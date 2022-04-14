# Projeto Cardápio Online (Back-end)



## Configurações utilizadas

### Instalação AdonisJS

```bash
npm i -g @adonisjs/cli
```
#### Criando uma nova aplicação

```bash
adonis new "menu" --api-only
cd "menu"
```

### Iniciando o Servidor

```bash
adonis serve --dev
```

### Instalação do banco de dados

```bash
npm install pg
```



## Migrations

### Criando Migrations

```bash
adonis make:migration product
```
`Choose an action Create table`

### Rodando as Migrations

```
adonis migration:run
```

### Status das Migrations

```
adonis migration:status
```

### Reverter todas as Migrations

```
adonis migration:reset
```



## Models

### Criando Models

```
adonis make:model Product
```



## Validator

### Setup

Primeiro, execute o comando adonis para baixar o validator provider:
```
adonis install @adonisjs/validator
```
Em seguida, registre o validator provider dentro do arquivo start/app.js:
```js
const providers = [
  '@adonisjs/validator/providers/ValidatorProvider'
]
```

### Criando Validator

Validators ficam dentro do diretório `app/Validators`:
```
adonis make:validator ValidacaoUsuario
```