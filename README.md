# # LoginAuth com Django_rest_framework e Knox

Uma Simples api rest com login, logout e signup, segura e prática feita com Knox e autenticação por Token

# Instalação
Após baixar o arquivo .zip ou clonar, abra o com cmd e rode: **pip install** -r **requirements**.**txt**, depois de instalar todas as depedências rode: **py manage.py runserver** 

# Register

 Para fazer o SignUp acesse a rota **_**http://localhost:8000/api/register/**_ no seu navegador ou client rest
 {
    "username": "seu_username",
    "email": "exemplo@gmail.com",
    "password": "exemplosenha12345"
}
após feito o registro você irá ter seu access Token

## Login

Para Fazer o login acesse: **_**http://localhost:8000/api/login/**_ 
digite seu email e senha criados 
{
    "username": "seu_username",
    "password": "exemplosenha12345"
}
a função te retornará, e você já estará logado
{
    "expiry": "2020-06-29T02:56:44.924698Z",
    "token": "99a27b2ebe718a2f0db6224e55b622a59ccdae9cf66861c60979a25ffb4f133e"
}

## Logout

para fazer o logout acesse: **http://localhost:8000/api/logout/**
nos headers 
Authorization: Token {o seu token de acesso}
Pronto estará deslogado




