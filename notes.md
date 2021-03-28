# Angular - CRUD

## passos...

### Criando o Backend

- criar pasta backend;
- rodar o comando **npm init -y**;
- instalar pacote **npm i json-server**;
- Criar arquivo **db.json** dentro da pasta backend;
- colocar o seguinte array de objetos no db.json:

```json
    {
        "products": [
        {
            "id": 1,
            "name": "Caneta BIC Preta",
            "price": 5.89
        },
        {
            "id": 2,
            "name": "Notebook Mac Pro",
            "price": 12000.89
        },
        {
            "id": 3,
            "name": "Sansung S20+",
            "price": "5000.89"
        }
        ]
    }
```
- no arquivo package.json vamos criar um script **"start": "json-server --watch db.json --port 3001"**;
- podemos testar rodando na pasta backend o comando - **npm start**;
- esse comando roda o servidor na porta 3001 - simulando uma api com o recurso **/produtos**;

---

### O que é o Angular?

- Framework js criado pelo Google para a criação de SPAs;
- Baseada em componentes;
- Trabalhamos com TS - superset do JS;
- Versão 2 até as mais recentes não existem tantas quebras;
- Usamos muito o CLI;

---

### Conceitos...

- Main.ts -> AppModule -> AppComponent (que chama os outros componentes);
- O que é um componente? Algo que represena algo na tela;
- Um componente tem um Arquivo html, css e ts;
- Um componente quando criado é gerado uma tag (estilo html);
- No arquivo Ts é onde referenciamos o html e css;
- Na classe do TS existe um decorator @Component;
- Os componentes estão dentro de algum **módulo**;
- Podemos ter mais de um módulo por aplicação;
- Um componente pode ser definido como visivel apenas para o seu módulo ou não;
- Um módulo possui: Declarations, Imports, Exports, Providers e Bootstrap;
- Declarations - ficam os componentes, diretivas e pipes que pertencem ao modulo;
- Exports - ficam os componentes, diretivas e pipes que pertencem ao modulo (que serão exportados);
- Imports - importa outros módulos;
- Providers - declaramos os services;
- Bootstrap - componente que será carregado - no módulo inicial.

---

### Criando App com Angular CLI

- Na pasta do projeto instalar a CLI -> **npm i -g @angular/cli**;
- Instalado a CLI, rodamos o comando para criar um novo projeto -> **ng new frontend --minimal**;
- Criado o projeto, entramos na pasta e digitamos o comando **npm start**;
- Esse comando compila o programa e serve na porta 4200;

---

### Conhecendo os arquivo do projeto

- **angular.json**: Arquivo de configuração
 - Alterar o template inline e style inline para false;
- Dentro da pasta **src**:
 - Temos o **main.ts**: chama o AppMoule (módulo principal);
 - O AppModule esta dentro da pasta **app**;
    - Dentro da pasta temos o arquivo de rota, componente e módulo;
 - Existe a pasta **assets** - Arquivos estáticos - colocaremos uma imagem, por exemplo;
 - **environments** - que define as variáveis de ambiente;
 - **index.html** - página da aplicação - que chama o <app-root>, que é o componente que foi criado com esse seletor;

 ---

 ### Html do AppComponent


