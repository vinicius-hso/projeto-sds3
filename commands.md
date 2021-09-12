# Comandos

## Front-end

__Criar projeto__
`npx create-react-app front-end --template typescript`

__Remover diretório .git__
`rm -rf .git`

__Iniciar o projeto__
`yarn start`

__Configurando Typescript__
`tsconfig.json`-> `compilerOptions` -> add `"baseUrl": "./src"`

__Adicionar Boostrap__
`yarn add bootstrap`

__Adicionar apexcharts__
`yarn add apexcharts react-apexcharts`

__Adicionar React-router-dom__
`yarn add react-router-dom`

__Adicionar tipos do TypeScript__
`yarn add @types/react-router-dom -D`

__Adicionar Axios__
`yarn add axios`

__Adicionar Date-FNS__
`yarn add date-fns`



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

## Deploy

__Heroku__

```
postgres://

dxtebsilednniw

:

77c7a292eaa8f48277acc9e3297b0820182882ce09a53f88bf7d8e89c0a451bc

@ec2-44-195-16-34.compute-1.amazonaws.com:

5432

/

dp82kglkvnujv
```

