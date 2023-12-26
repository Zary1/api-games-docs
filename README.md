# Api de games
Esta API é utilizado para tal e tal....
## Endpoints
### Get/ games
Esse endpoint é responsavel por retornar a listagem de todos cadastrados no banco de dados
#### Parametros
Nenhum

##### Respostas
######Ok ! 200

Caso essa resposta aconteça voçe vai recever a listagem de todos os games.
Exemplo de respostas:
```
[
        {
            "id": 1,
            "title": "call of dudi",
            "year": 2000,
            "price": 12
        },
        {
            "id": 2,
            "title": "call of mum",
            "year": 2030,
            "price": 19
        },
        {
            "id": 3,
            "title": "baby bom",
            "year": 2010,
            "price": 62
        }
    ]
```
### Post/ games
Esse endpoint é responsavel por retornar a listagem de todos  os games cadastrados no banco de dados
#### Parametros
email:E-email do usuário cadastrado no sistema
password : senha do usuário cadastrado no sistema ,com aquele determinado email

Exemplo de respostas:
```
{
  "eamil":"Ratinha meu amor",
  "password":"ratinha@zary",


}
```
#### Falga na autenticação ! 401

Caso essa resposta aconteça,isso sognifica que aconteceu alguma falha durante o processo de autencicação. Motivos: token iválido, token expirado
Exemplo de respostas:
```
{
"error" :'Token inválido'


}
```
