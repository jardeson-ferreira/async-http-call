# Exemplo de Chamada HTTP não bloqueante em Django

Este é um exemplo simples de uma função assíncrona em Django que realiza uma chamada HTTP não bloqueante usando a biblioteca `httpx`. Essa abordagem permite que o código continue executando outras tarefas enquanto aguarda a resposta da chamada HTTP.

## Pré-requisitos

Certifique-se de ter instalado o Python e o Django em seu ambiente de desenvolvimento.

## Instalação

1. Clone este repositório em sua máquina local.

2. Navegue até o diretório do projeto.

## Uso

1. Execute o servidor de desenvolvimento do Django.


2. Abra o navegador e acesse `http://localhost:8000`.

3. Você verá a mensagem "Non-blocking HTTP request!" no navegador.

## Explicação do Código

O código consiste em duas funções principais:

- A função `http_call_async` é uma função assíncrona que realiza uma chamada HTTP não bloqueante. Ela itera de 1 a 5, aguardando 1 segundo em cada iteração e exibindo o número correspondente. Em seguida, realiza uma chamada GET assíncrona para a URL "https://httpbin.org/" usando o cliente HTTP da biblioteca `httpx`.

- A função `async_view` é uma view assíncrona do Django que inicia a chamada HTTP assíncrona em segundo plano e retorna uma resposta HTTP imediata.

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões, melhorias ou correções, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Desenvolvedores

| [<img src="https://avatars.githubusercontent.com/jose-uchoa" width=115><br><sub>Jose Uchoa</sub>](https://github.com/jose-uchoa) |
| :----------------------------------------------------------: |
