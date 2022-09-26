# Bootcamp Database Experience :rocket:

Modelagem de um contexto reduzido de e-commerce, utilizando variação de modelo entidade relacional.

## Projeto - E-commerce [MER]

### DESCRIÇÃO

Refinamento do modelo apresentado acrescentando os seguintes pontos:

* **Cliente PJ e PF**
  > Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
  * [X] Implementado como duas entidades independentes
    * **`Cliente_pf`**
    * **`Cliente_pj`**

* **Forma Pagamento**
  > Pode ter cadastrado mais de uma forma de pagamento;
  * [X] Implementado uma entidade **`Wallet`**
    * contém os dados de pagamento do cliente
    * Associados por `idWallet`

* **Entrega**
  > Possui status e código de rastreio;
  * [X] Implementado como uma entidade **`Entrega`**
    * Entidade se relaciona com `Pedido`
    * FK `idCliente`, `idPedido`, `IdWallet`

| **SQL** |
