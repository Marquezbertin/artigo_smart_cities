# Estrutura Básica

* !DOCTYPE html: Define a versão do HTML sendo utilizada.
* html lang="pt-br": Abre a tag HTML e define o idioma da página como português brasileiro.

# Cabeçalho (Head)

* head: Início da seção de cabeçalho, onde informações sobre o documento são colocadas.
* meta charset="UTF-8": Define o conjunto de caracteres como UTF-8, que inclui a maioria dos caracteres utilizados globalmente.
* title: Define o título da página exibido na barra de título do navegador.

# Estilos (Style)

* style: Define o estilo da página utilizando CSS (Cascading Style Sheets).
* body: Estilos aplicados ao corpo da página.
* .container, .box, .news-container: Estilos aplicados a diferentes containers.
* h1, img, p, ul, li, footer a: Estilos aplicados a diferentes elementos HTML.
  
## Corpo (Body)

* body: Início da seção de corpo, onde o conteúdo visível da página é colocado.
* div class="container": Container principal que envolve a seção de notícias e a caixa de conteúdo principal.
* div class="news-container": Container para exibir as últimas notícias.
* ul id="news-list": Lista não ordenada onde as notícias serão inseridas dinamicamente usando JavaScript.
* div class="box": Caixa principal que contém o conteúdo relacionado às cidades digitais e smart cities.
* img src="...": Imagem relacionada às cidades digitais e smart cities.
* p: Vários parágrafos que explicam a relação entre cidades digitais e smart cities.
* footer: Rodapé que contém informações sobre a autoria do artigo, data de criação e um link para o LinkedIn.

# Script (JavaScript)

* script: Inclui o script JavaScript para buscar e exibir automaticamente as últimas notícias.
* const apiKey = '...';: Define uma chave de API para autenticar na NewsAPI (substitua pela sua própria chave).
* const newsList = document.getElementById('news-list');: Referência à lista de notícias no HTML.
* async function fetchNews() { ... }: Função assíncrona para buscar e exibir notícias.
* Chamada para a função fetchNews() para iniciar a busca automática de notícias quando a página é carregada.

# Teste Local da Página HTML

Este é um guia simples para realizar testes locais da sua página HTML utilizando um servidor local. Isso é útil especialmente quando há interações com APIs externas, como no caso de exibir notícias atualizadas em sua página.

## Pré-requisitos

- [Python](https://www.python.org/downloads/) (para a opção de servidor Python)
- [Node.js](https://nodejs.org/) (para a opção de servidor Node.js)

## Configurando e Executando o Servidor Local

### Opção 1: Usando o Python

1. Abra o terminal.
2. Navegue até o diretório onde seu arquivo HTML está localizado.
3. Execute o seguinte comando, dependendo da versão do Python:
    ```bash
    python -m http.server
    ```
    ou
    ```bash
    python -m SimpleHTTPServer
    ```
4. Acesse a página em seu navegador em `http://localhost:8000` ou `http://127.0.0.1:8000`.

### Opção 2: Usando o Node.js

1. Abra o terminal.
2. Instale o `http-server` globalmente usando o seguinte comando:
    ```bash
    npm install -g http-server
    ```
3. Navegue até o diretório onde seu arquivo HTML está localizado.
4. Execute o seguinte comando:
    ```bash
    http-server
    ```
5. Acesse a página em seu navegador em `http://localhost:8080`.

### Opção 3: Usando o Visual Studio Code

1. Instale a extensão "Live Server" no Visual Studio Code.
2. Clique com o botão direito no seu arquivo HTML.
3. Escolha "Open with Live Server".
4. A página será aberta automaticamente em seu navegador padrão.

## Notas Importantes

- Certifique-se de que o servidor local esteja em execução enquanto estiver testando a página.
- Verifique as instruções específicas fornecidas na seção de testes locais do seu projeto, especialmente se houver interações com APIs externas.


# Conclusão

Este código HTML cria uma página web interativa e informativa sobre a relação entre cidades digitais e smart cities, incluindo uma seção dinâmica de notícias. O código utiliza HTML para estrutura, CSS para estilos e JavaScript para interatividade. Certifique-se de substituir a chave da API e personalizar conforme necessário.