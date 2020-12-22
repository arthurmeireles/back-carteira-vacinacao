# Back-end Carteira de Vacinação Digital

Link para Servidor https://lais-api-carteira-vacinacao.herokuapp.com/

## Pre-requisito

### Configuração do Banco de Dados

Crie um novo banco de dados:

```sh
sudo -u postgres psql -U postgres -c "CREATE DATABASE nomedobanco;"
```

Ajuste nas settings o username e senha do seu database

```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'nomedobanco',
        'USER': "seu_user",
        'PASSWORD': "sua_senha",
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```


## Configuração do Ambiente

1. Clonar o repositório com ˋˋˋhttps://github.com/arthurmeireles/back-carteira-vacinacao.git ˋˋˋ
2. Instalar dependências com ˋˋˋpip install -r requirements.txtˋˋˋ
3. Gerar as migrações com ˋˋˋpython manage.py makemigrationsˋˋˋ
4. Rodar as migrações com  ˋˋˋpython manage.py migrateˋˋˋ
5. Rodar o servidor com ˋˋˋpython manage.py runserverˋˋˋ

