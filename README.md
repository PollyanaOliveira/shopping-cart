<h1 align="center">🛒🛒Shopping Cart🛒🛒</h1>  </p>


## Desenvolvido por

@PollyanaOliveira

## Objetivos do Projeto

- Fazer requisições a uma API *(Application Programming Interface)* do Mercado Livre;
- Utilizar os seus conhecimentos sobre JavaScript, CSS e HTML;
- Trabalhar com funções assíncronas;

## Requisitos do projeto

## Documentação da API do Mercado Livre

A página _web_ consome os dados da API do _Mercado Livre_ para realizar a busca de itens da loja online. As buscas podem ser consultadas nos seguintes _endpoints_:

- "https://api.mercadolibre.com/sites/MLB/search?q=$QUERY"
- "https://api.mercadolibre.com/items/$ItemID"

### Lista de requisitos

### 1 - Crie uma listagem de produtos

Você deve criar uma listagem de produtos que devem ser consultados através da API do Mercado Livre.

Adicione o elemento retornado da função `createProductItemElement(product)` como filho do elemento `<section class="items">`.

**Obs:** as variáveis `sku`, no código fornecido, se referem aos campos `id` retornados pela API.

### 2 - Adicione o produto ao carrinho de compras

Cada produto na página _HTML_ possui um botão com o nome `Adicionar ao carrinho!`.

Adicione o elemento retornado da função `createCartItemElement(product)` como filho do elemento `<ol class="cart__items">`.

### 3 - Remova o item do carrinho de compras ao clicar nele

Ao clicar no **produto no carrinho de compra**, ele deve ser removido da lista.
Para isso, uma função (já existente) chamada `cartItemClickListener(event)` deve ser implementada com a lógica necessária para realizar a remoção.

### 4 - Carregue o carrinho de compras através do **LocalStorage** ao iniciar a página

Ao carregar a página, o estado atual do carrinho de compras deve ser carregado do **LocalStorage**.
Para que isso funcione, o carrinho de compras deve ser salvo no **LocalStorage**, ou seja, todas as **adições** e **remoções** devem ser abordadas para que a lista atual seja salva.

### 5 - Some o valor total dos itens do carrinho de compras de forma assíncrona

Cada vez que se adicionar um item ao carrinho de compras, será necessário somar seus valores e apresentá-los na página principal do projeto. Não queremos que essa soma, no entanto, impacte no carregamento da página. Devemos, portanto, fazer essa soma de forma *assíncrona*. Use `async/await` para fazer isso. O elemento que tem como filho o preço total dos itens do carrinho deve ter, **obrigatóriamente**, a classe `total-price`.

### 6 - Crie um botão para limpar carrinho de compras

Crie um botão para remover todos os itens do carrinho de compras. Ele deve, **obrigatóriamente**, ter a classe `empty-cart`.

### 7 - Adicione um texto de "loading" durante uma requisição à API

Uma requisição à API gasta um tempo e durante ele, ficamos sem saber se está tudo certo ou se algo deu errado.
Normalmente é utilizada alguma forma para mostrar que a requisição está em andamento.
Mostre a palavra "loading..." em algum lugar da página **apenas durante** a requisição à API. O elemento mostrado durante o carregamento da página deve, **obrigatóriamente**, ter a classe `loading`.

---
