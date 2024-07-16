# Exemplo de Chamada HTTP Assíncrona

Este é um exemplo simples de uma função assíncrona em Django que faz uma chamada HTTP não bloqueante usando a biblioteca `httpx`. Essa abordagem permite que o código continue executando outras tarefas enquanto aguarda a resposta da chamada HTTP.

## Pré-requisitos

Certifique-se de ter o Python e o Django instalados no seu ambiente de desenvolvimento.

## Instalação

1. Clone este repositório para sua máquina local.

2. Navegue até o diretório do projeto.

3. Instale a biblioteca `httpx`:
    ```bash
    pip install httpx
    ```

## Uso

1. Execute o servidor de desenvolvimento do Django:
    ```bash
    python manage.py runserver
    ```

2. Abra o seu navegador e vá para `http://localhost:8000`.

3. Você verá a mensagem "Non-blocking HTTP request!" no navegador.

## Explicação do Código

O código consiste em duas funções principais:

- A função `http_call_async` é uma função assíncrona que faz uma chamada HTTP não bloqueante. Ela itera de 1 a 5, aguardando 1 segundo em cada iteração e exibindo o número correspondente. Em seguida, faz uma solicitação GET assíncrona para a URL "https://httpbin.org/" usando o cliente HTTP da biblioteca `httpx`.

- A função `async_view` é uma view assíncrona do Django que inicia a chamada HTTP assíncrona em segundo plano e retorna uma resposta HTTP imediata.

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões, melhorias ou correções, sinta-se à vontade para abrir uma issue ou enviar um pull request.
