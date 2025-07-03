<h1 align="center">PHP Code Coverage Dark mode</h1>

## Descrição
- Repositório com estilos CSS para sobrescrever os estilos padrão das paginas HTML geradas pela lib [php-code-coverage](https://github.com/sebastianbergmann/php-code-coverage) com tema escuro
- Para projetos com Laravel

## Como aplicar no seu projeto Laravel
- Sobrescreva o script "test" com os comandos a seguir no composer.json
  ```json
    "scripts": {
      "test": [
        "@php artisan config:clear --ansi",
        "@php artisan test --coverage-html coverage ; curl https://raw.githubusercontent.com/henrqueDev/php-code-coverage-dark/main/style.css -o coverage/_css/style.css"
      ]
    }
  ```
- Para rodar o script com as alterações
  ```shell
    composer run-script test
  ```
