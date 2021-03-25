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