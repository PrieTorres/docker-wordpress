# docker-wordpress

Este projeto define um ambiente Docker com quatro serviços principais:

- **nginx**: atua como proxy reverso expondo o WordPress em `/wordpress`.
- **mysql 5.7**: banco de dados utilizado pelo WordPress.
- **wordpress**: aplicação web WordPress.
- **phpmyadmin**: interface para administração do banco de dados.

## Como executar

1. Execute `docker compose up -d` para iniciar todos os serviços.
2. Acesse o WordPress em [http://localhost/wordpress](http://localhost/wordpress).
3. Para acessar o phpMyAdmin utilize [http://localhost:8080](http://localhost:8080).

O WordPress não ficará disponível diretamente em `http://localhost`, apenas por meio do nginx na rota `/wordpress`.
