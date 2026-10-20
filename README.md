# alura_space

Galeria de imagens do espaço feita em Django, durante o curso "Django: templates e boas práticas" da Alura (2024).

O que o projeto pratica: templates com herança, arquivos estáticos, rotas (`/` e `/imagem/`) e a `SECRET_KEY` lida de variável de ambiente, fora do código.

## Como rodar

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
echo "SECRET_KEY=$(python3 -c 'import secrets; print(secrets.token_urlsafe(50))')" > .env
python manage.py migrate
python manage.py runserver
```

Abra http://127.0.0.1:8000.

Projeto de estudo: `DEBUG = True` e sem configuração de produção.
