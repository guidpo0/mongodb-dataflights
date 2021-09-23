### Informações Gerais

Projeto desenvolvido durante formação em desenvolvedor Web Full Stack pela Trybe.

---

# Boas vindas ao repositório do projeto DataFlights!!

Neste projeto foi praticado os conceitos básicos de **MongoDB** utilizando o banco de dados `dataFlights`.

Lembrando que esta aplicação corresponde aos meus esforços para melhorar minhas hard skills e soft skills, sinta-se à vontade para explorá-la! Feedbacks construtivos são sempre bem vindos!

Abaixo você poderá encontrar mais informações técnicas sobre este projeto.

---

# Sumário

- [Habilidades](#habilidades)
- [Intruções para fazer o fork do repositório](#intruções-para-fazer-o-fork-do-repositório)
- [Informações do projeto](#informações-do-projeto)
  - [Linter](#linter)
  - [Instruções para restaurar o banco de dados dataFlights](#instruções-para-restaurar-o-banco-de-dados-dataFlights)
  - [Implementações técnicas](#implementações-técnicas)
- [Desafios](#desafios)
  - [Desafio 1](#desafio-1)
  - [Desafio 2](#desafio-2)
  - [Desafio 3](#desafio-3)
  - [Desafio 4](#desafio-4)
  - [Desafio 5](#desafio-5)
  - [Desafio 6](#desafio-6)
  - [Desafio 7](#desafio-7)
  - [Desafio 8](#desafio-8)
  - [Desafio 9](#desafio-9)
  - [Desafio 10](#desafio-10)
  - [Desafio 11](#desafio-11)
  - [Desafio 12](#desafio-12)
  - [Desafio 13](#desafio-13)
  - [Desafio 14](#desafio-14)
  - [Desafio 15](#desafio-15)
  - [Desafio 16](#desafio-16)
  - [Desafio 17](#desafio-17)
  - [Desafio 18](#desafio-18)
  - [Desafio 19](#desafio-19)
  - [Desafio 20](#desafio-20)
  - [Desafio 21](#desafio-21)
  - [Desafio 22](#desafio-22)
  - [Desafio 23](#desafio-23)
  - [Desafio 24](#desafio-24)
  - [Desafio 25](#desafio-25)
  - [Desafio 26](#desafio-26)
  - [Desafio 27](#desafio-27)
  - [Desafio 28](#desafio-28)

---

# Habilidades

Nesse projeto, fui capaz de:

- Buscar documentos no banco
- Usar filtros na busca
- Deletar documentos conforme filtro
- Contar documentos compreendidos nos filtros pedidos
- Inserir documentos no banco

---

# Instruções para fazer o fork do repositório

1. Faça o fork do repositório

2. Instale as dependências do projeto
  * Instale as dependências:
    * `npm install`

---

# Informações do projeto

### Linter

Para garantir a qualidade do código de forma a tê-lo mais legível, de mais fácil manutenção e seguindo as boas práticas de desenvolvimento foi utilizado neste projeto o linter `ESLint`.

### Instruções para restaurar o banco de dados `dataFlights`

1. Abra o terminal e conecte-se à sua instância local do **MongoDB**.

2. Agora que você tem certeza de que a sua instância está no ar e que você está conectado a ela, digite `exit`. Você voltará ao terminal para iniciar a importação dos dados.

3. Na raiz do diretório do projeto, execute o seguinte comando que fará a restauração da base de dados `dataFlights`:
    ```sh
    DBNAME=dataFlights ./scripts/resetdb.sh assets
    ```

  * A execução desse script criará um banco de dados chamado `dataFlights` e importará os dados para a coleção `voos`.

### Implementações técnicas

Para executar localmente os testes, é preciso escrever o seguinte no seu terminal, estando na raiz do diretório do projeto:
```sh
./scripts/evaluate.sh
```

Esse script passará por **todos os desafios** e imprimirá um relatório indicando se passou ou não para cada desafio. Como a execução do script **envolve restauração da base de dados `dataFlights`** de um teste para outro, recomenda-se esperar pela sua execução completa.

Para executar somente o teste de um desafio, execute o comando abaixo, substituindo N pelo númedo do desafio

```sh
./scripts/evaluate.sh desafioN
```

---

# Desafios

#### Desafio 1

Retorne a quantidade de documentos inseridos na coleção `voos`.

#### Desafio 2

Retorne os 10 primeiros documentos com voos da empresa `AZUL`.

#### Desafio 3

Retorne a quantidade de voos da empresa `AZUL`.

#### Desafio 4

Retorne a quantidade de voos da empresa `GOL`.

#### Desafio 5

Retorne o `vooId` do décimo ao décimo segundo documento da coleção `voos`.

#### Desafio 6

Retorne apenas os campos `empresa.sigla`, `empresa.nome` e `passageiros` do voo com o campo `vooId` igual a `756807`.

#### Desafio 7

Retorne a quantidade de voos em que o ano seja menor do que `2017`.

#### Desafio 8

Retorne a quantidade de voos em que o ano seja maior do que `2016`.

#### Desafio 9

Retorne a quantidade de voos entre os anos de `2017` e `2018`.

#### Desafio 10

Retorne apenas os **10** primeiros documentos com voos da empresa `GOL` do ano de `2017`. Exiba apenas os campos `vooId`, `empresa.nome`, `aeroportoOrigem.nome`, `aeroportoDestino.nome`, `mes` e `ano`.

#### Desafio 11

Retorne a quantidade de documentos em que o campo `aeroportoDestino.pais` não seja igual a `ESTADOS UNIDOS`.

#### Desafio 12

Retorne a quantidade de documentos em que o campo `aeroportoDestino.pais` seja igual a `BRASIL`, `ARGENTINA` ou `CHILE`.

#### Desafio 13

Retorne a quantidade de documentos em que o campo `aeroportoDestino.continente` não seja igual a `EUROPA`, `ÁSIA` e `OCEANIA`.

#### Desafio 14

Retorne o total de voos em que o país de origem não seja `BRASIL`.

#### Desafio 15

Retorne o total de voos com mais de 20 `decolagens`.

#### Desafio 16

Retorne o total de voos em que o campo `natureza` possui o valor `Internacional`.

#### Desafio 17

Retorne o total de voos em que o campo `natureza` possui o valor `Doméstica`.

#### Desafio 18

Retorne o `vooId`, `mes` e `ano` do primeiro voo com mais de `7000` passageiros pagos.

#### Desafio 19

Retorne o `vooId` do primeiro voo em que o campo `litrosCombustivel` exista.

#### Desafio 20

Retorne o `vooId` do primeiro voo em que o campo `rtk` não exista.

#### Desafio 21

Retorne o `vooId` do primeiro voo em que o campo `litrosCombustivel` seja maior ou igual a `1000`.

#### Desafio 22

Retorne o `vooId` do primeiro voo em que a empresa seja `DELTA AIRLINES` ou `AMERICAN AIRLINES`, a sigla do aeroporto de origem seja `SBGR` e a sigla do aeroporto de destino seja `KJFK`.

#### Desafio 23

Retorne o `vooId` e `litrosCombustivel` do primeiro voo em que o campo `litrosCombustivel` **não seja maior do que** `1000` e o campo `litrosCombustivel` exista.

#### Desafio 24

Retorne o `vooId`, `empresa.nome` e `litrosCombustivel` do primeiro voo em que `litrosCombustivel` **não seja maior do que** `600` **e** a empresa **não seja** `GOL` **ou** `AZUL`, **e** o campo `litrosCombustivel` exista.

#### Desafio 25

Remova todos os voos da empresa `AZUL` em que a quantidade de combustível seja menor do que `400`. Informe a quantidade de documentos removidos.

#### Desafio 26

Remova todos os voos da empresa `GOL` em que a quantidade de passageiros pagos esteja entre `5` e `10`, incluindo os casos em que a quantidade é `5` e `10`. Informe a quantidade de documentos removidos.

#### Desafio 27

Retorne a quantidade total de voos de natureza `Doméstica` que a empresa `PASSAREDO` possui, via uso de uma nova coleção chamada `resumoVoos`.

Ou seja, a coleção `resumoVoos` conterá documentos onde cada um indica para cada empresa a quantidade total de voos que ela possui de natureza `Doméstica`.

Para isso, escreva no arquivo `desafio27.js` duas queries, **nesta ordem**:

1. Conte quantos voos da empresa `PASSAREDO` cujo campo `natureza` possua valor igual a `Doméstica` e crie uma query que insira na coleção `resumoVoos` um documento com os campos: `empresa` (nome da empresa) e `totalVoosDomesticos` (o total retornado anteriormente).

2. Em uma segunda query, retorne a `empresa` e o `totalVoosDomesticos` do primeiro documento presente na coleção `resumoVoos` em que a empresa seja `PASSAREDO`.

#### Desafio 28

Retorne a quantidade total de voos de natureza `Doméstica` que a empresa `LATAM AIRLINES BRASIL` possui, via uso de uma nova coleção chamada `resumoVoos`.

Para isso, escreva no arquivo `desafio28.js` duas queries, **nesta ordem**:

1. Conte quantos voos da empresa `LATAM AIRLINES BRASIL` cujo campo `natureza` possua valor igual a `Doméstica` e crie uma query que insira na coleção `resumoVoos` um documento com os campos: `empresa` (nome da empresa) e `totalVoosDomesticos` (o total retornado anteriormente).

2. Em uma segunda query, retorne a `empresa` e o `totalVoosDomesticos` do primeiro documento presente na coleção `resumoVoos` em que a empresa seja `LATAM AIRLINES BRASIL`.

---