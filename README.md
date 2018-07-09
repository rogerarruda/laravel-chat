# Laravel chat com Pusher

Criação de um aplicativo de bate-papo com o Laravel e o Pusher

## Getting Started

Clone o repositório do projeto

```bash
git clone https://github.com/rogerarruda/laravel-chat
```

Depois de clonar, entre na pasta e execute o comando (você deve ter o composer instalado):

```bash
composer install
```

Copie o arquivo `.env.example` and rename it `.env`

Depois execute:

```bash
php artisan key:generate
```

### Configurando o Pusher

Se você não tiver um, crie uma conta gratuita no Pusher em [https://pusher.com/signup](https://pusher.com/signup) então faça o login no seu painel e crie um aplicativo.

Coloque `BROADCAST_DRIVER` em seu arquivo `.env` **pusher**:

```txt
BROADCAST_DRIVER=pusher
```

Em seguida, preencha suas credenciais do aplicativo Pusher no seu `.env`:

```txt
PUSHER_APP_ID=xxxxxx
PUSHER_APP_KEY=xxxxxxxxxxxxxxxxxxxx
PUSHER_APP_SECRET=xxxxxxxxxxxxxxxxxxxx
PUSHER_APP_CLUSTER=
```

### Migração do banco de dados

Certifique-se de preencher os detalhes do banco de dados em seu `.env` depois execute o comando:

```bash
php artisan migrate
```

E finalmente, inicie o aplicativo:


```bash
php artisan serve
```

visite [http://localhost:8000/](http://localhost:8000/) veja a aplicação em ação.
