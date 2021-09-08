# Comandos

## Front-end

Criar projeto
`npx create-react-app front-end --template typescript`

Remover diretório .git
`rm -rf .git`

Iniciar o projeto
`yarn start`

Configurando Typescript
`tsconfig.json`-> `compilerOptions` -> add `"baseUrl": "./src"`

Adicionar Boostrap
`yarn add bootstrap`

Adicionar apexcharts
`yarn add apexcharts react-apexcharts`

## Back-end

Criar projeto com Spring Initializer

Dependências: Web, JPA, H2, Postgres, Security

### Mapeamento Objeto Relacional

Mapeamento e conversão dos dados que estão no paradigma Orientado a Objeto para o paradigma Relacional.

__Mapeando__:

Mapeamento do Objeto Seller

* Definindo como tabela:

  ```java
  @Entity
  @Table(name = "<table_name>")
  ```

* Definindo o Id:

  ```java
  @Id 
  @GeneratedValue(strategy = GenerationType.IDENTITY)
  ```

* Definindo a FK:

  ```java
  @ManyToOne
  @JoinColumn(name = "<db_column_name>")
  
  // o objeto que será FK deverá receber o seguinte mapeamento
  
  /* definição como tabela */
  /* definição de id */
  
  //
  @OneToMany(mappedBy = "seller")
  ```

