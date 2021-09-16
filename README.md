# API do Dead By Daylight - NodeJs

<img src="https://1hitgames.com/wp-content/uploads/2019/08/Dead-by-Daylight-1-1.jpg" alt="DarkSouls Logo" style="zoom:98%;" />

> API criada para estudar conceitos de back-end, utilizando a linguagem de programação JavaScript e o banco de dados MongoDB. Nessa API eu crio um CRUD completo de personagens do DbD.

Para utilizar o projeto faça o dowload do arquivo zip, ou faça o clone em seu computador utilizando o Git. Execute o comando `npm i` dentro da pasta do projeto em seu computador(a pasta que contém o arquivo package.json), para baixar as dependencias do projeto.

## Executando o projeto

*Essa API utiliza o mongodb como banco de dados e o mongoose como ODM, então antes de testar a API certifique se você possui o MongoDb instalado em seu computador(https://www.mongodb.com/try/download/community).*

Além disso, você precisa criar o arquivo .env com a url do seu banco, *utilize o arquivo .env.exemple para criar o seu*. Esse é um exemplo de string de conexão com o banco de dados: mongodb://localhost:27017/db_darksouls.

Agora você pode executar o projeto: 
* Para executar o projeto com o nodemon, digite no terminal: 
```bash
npm run dev
```
* Para executar o projeto com o node, digite no terminal: 
```bash
npm start
```
## Testando a API

Você pode utilizar as ferramentas:

* Postman
* Insomnia
* Thunder Client (plugin no vsCode)

Exemplos de URLs: 
* Essa é a URL de teste padrão: http://localhost:3000/personagens
* Para buscar por ID, Editar ou Apagar, insira o ID na URL: http://localhost:3000/personagens/5
* Para fazer uma busca com query string, esse é um exemplo de URL: http://localhost:3000/personagens/filter?identidade=Steve


Essa é a estrutura JSON para fazer o POST e o PUT:

```json
{
    "nome": "Joe Keery",
    "identidade": "Steve Harrington",
    "genero": "Masculino",
    "imagem": "https://static.wikia.nocookie.net/deadbydaylight_gamepedia_en/images/7/75/S19_charSelect_portrait.png/revision/latest/scale-to-width-down/150?cb=20200721164551"
}
```
<img src= "https://i.redd.it/1f3eobeziq271.png" style="zoom:30%;"> 

> *"No One Touches My Kids."* -
**Steve**

```json
{
    "nome": "Michael Audrey Myers",
    "identidade": "Michael Mayers",
    "genero": "Masculino",
    "imagem": "https://static.wikia.nocookie.net/villains/images/4/44/Michael_Myers-0.jpg/revision/latest/scale-to-width-down/350?cb=20190204001554"
}
```
<img src= "https://steamuserimages-a.akamaihd.net/ugc/920296549072323619/8A6FE0A28177AA9AAE54EAABE3D188FE5F662B86/?imw=512&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false" style="zoom:30%;">

> *"I met him fifteen years ago. I was told there was nothing left; no reason, no conscience, no understanding in even the most rudimentary sense of life or death, of good or evil, right or wrong. I met this... six year old child with this blank, pale, emotionless face, and... the blackest eyes - the devil's eyes. I spent eight years trying to reach him, and then another seven trying to keep him locked up because I realized that what was living behind that boy's eyes was purely and simply... evil."*
― **Samuel Loomis**

Obrigado por testar e utilizar minha API, volte sempre!