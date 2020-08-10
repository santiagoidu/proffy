<h1 align="center">
    <img alt="Proffy" src=".github/logo.svg" height="100px" />
    <br>Next Level Week #2<br/>
    Node.js | ReactJS | React Native
</h1>

<p align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/HigorSnt/proffy?style=flat-square">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/HigorSnt/proffy?style=flat-square">
  <img alt="GitHub" src="https://img.shields.io/github/license/HigorSnt/proffy?style=flat-square"> 
  <img alt="Made by Rocketseat" src="https://img.shields.io/badge/made%20by-Rocketseat-%237519C1?style=flat-square"><br/>
  <a href="https://insomnia.rest/run/?label=Proffy&uri=https%3A%2F%2Fraw.githubusercontent.com%2FHigorSnt%2Fproffy%2Fmaster%2F.github%2FInsomnia.json" target="_blank"><img src="https://insomnia.rest/images/run.svg" alt="Run in Insomnia"></a>
</p>
<p align="center">
  <a href="#bookmark-sobre">Sobre</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#rocket-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#winer_glass-como-executar">Como Ultilizar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#octocat-como-contribuir">Como Contribuir</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<p align="center">
  <img alt="design do projeto" width="650px" src="./.github/design.png" />
<p>

## :bookmark: Sobre

O **Proffy** é uma aplicação Web e Mobile feita para auxiliar na conexão entre os alunos e os professores. Logo, esta aplicação oferece aos professores a possibilidade de registrar aulas, podendo adicionar informações como a disciplina, o custo e horário e aos alunos a possibilidade de buscar pelas aulas cadastradas.
  
Este projeto foi idealizado pensando no **6 de agosto**, onde se comemora o **Dia Nacional dos Profissionais da Educação**.
  
Essa aplicação foi realizada durante a Next **Level Week #2**, projeto da [Rocketseat](https://rocketseat.com.br/).

## :rocket: Tecnologias

-  [Typescript](https://www.typescriptlang.org/)
-  [Node.js](https://nodejs.org/en/)
-  [ReactJS](https://reactjs.org/)
-  [React Native](http://facebook.github.io/react-native/)
-  [Expo](https://expo.io/)
-  [Express](https://expressjs.com/)
-  [axios](https://github.com/axios/axios)

## **:wine_glass:  COMO UTILIZAR**

### Configurações Iniciais

Primeiro, você precisa ter o <kbd>[NodeJS](https://nodejs.org/en/download/)</kbd> instalado na sua máquina. 

Se você estiver utilizando o **Linux**, você pode optar por instalar o **Node** através do gerênciador de versões <kbd>[asdf]</kbd> para facilitar o processo de mudança da versão do **Node**, quando for necessário.

Você pode optar também por utilizar o **yarn** no lugar do **npm**. Você pode instalar clicando nesse <kbd>[link][yarn]</kbd>, ou através do <kbd>[asdf]</kbd>.

Após ter o **Node** instalado, instale as dependências do **React e React Native (Expo)** de forma global, utilizando os comandos:

```sh
# React:
$ npm install create-react-app -g

# Expo (React Native):
$ npm install -g expo-cli 
```

Você precisa renomear o arquivo `.env-example` para `.env` e inserir as informações que condizem com o seu **host**:

```sh
$ mv .env-example .env
```

Instale as dependências contidas nos arquivos `package.json` que se encontram na raíz do repositório (para o gerenciamento de commits), no diretório do **server**, no diretório do **website** e no diretório **mobile**. Para instalar as dependências, basta abrir o terminal no diretório e digitar o comando:

```sh
$ npm install

# ou
$ yarn
```

1. Faça um clone do repositório:

```sh
  $ git clone https://github.com/santiagoidu/proffy.git
```

```sh
  # Instalando as dependências do commitlint:
  $ cd server
  $ yarn # ou npm install
  # Configurando o banco de dados e criando as tabelas.
  $ yarn knex:migrate # ou npm run knex:migrate

  # Instalando as dependências do website:
  $ cd web
  $ yarn # ou npm install

  # Instalando as dependências do mobile:
  $ cd mobile
  $ yarn # ou npm install
```
### Utilizando o Server

```sh
# Abrindo o terminal no diretório do servidor:
$ cd ./sources/server

# Executando a aplicação em modo de desenvolvimento:
$ npm run dev

# Instanciando o banco de dados:
$ npm run knex:migrate

# Povoando o banco de dados (seeds):
$ npm run knex:seed
```

> Veja a parte de **scripts {}** do arquivo <kbd>[package.json](./sources/server/package.json)</kbd> para saber quais scripts estão disponíveis.

### Utilizando o Website

```sh
# Abrindo o terminal no diretório do website:
$ cd ./sources/website

# Executando o website no modo de desenvolvimento:
$ npm run start
```

> Se o browser não abrir automaticamente, acesse: http://localhost:3000.

### Utilizando o Mobile

Instale o aplicativo <kbd>[Expo](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en)</kbd> no seu smartphone.

```sh
# Abrindo o terminal no diretório do mobile:
$ cd ./sources/mobile

# Executando o mobile no modo de desenvolvimento:
$ npm run start
```

Agora, abra o aplicativo do expo e no modo **LAN** faça o scan do QRCode.

> Se tiver algum problema para executar o aplicativo nesse modo, tente desabilitar o firewall da sua máquina.

**\* Lembre de inserir no arquivo `.env` o IP exato que foi gerado pelo seu mobile após utilizar o comando `npm run start`.**

Veja os arquivos **`package.json`** do <kbd>[commitlint](./package.json)</kbd>, <kbd>[server](./sources/server/package.json)</kbd>, <kbd>[website](./sources/website/package.json)</kbd> e <kbd>[mobile](./sources/mobile/package.json)</kbd>.

## **:octocat:  COMO CONTRIBUIR**
  
  - Verifique as **[Issues](https://github.com/santiagoidu/proffy/projects/1)** que estão abertas e se já não existe alguma com a sua feature;
  - Abra uma **Issue** com o nome e descrição da sua feature e assine com o seu usuário informando que irá fazê-la;
  - Faça um **[fork](https://help.github.com/pt/github/getting-started-with-github/fork-a-repo)** do repositório;
  - Entre no sua página do GitHub e faça um **clone** do seu **fork**;
  - Crie uma *branch* com o nome da sua feature: `git chechout -b feat/minhaFeature`;
  - Faça as alterações necessárias no código ou na documentação;
  - Instale as dependências do *commitlint* na raíz do projeto para a verificação dos commits: `npm install` ou `yarn`;
  - Faça o *commit* das suas alterações seguindo as [convenções de commit](https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/), adicione na descrição o id da sua Issue em parênteses e lembre de fechar a sua Issue com o id no rodapé do commit:

  ```
    <tipo>(escopo opcional): <descrição> (#x)

    [corpo do commit]

    Close #x
  ```
  Exemplo:
  ```sh
    feat: adicionado componente para tal coisa (#52)

    Foi adicionado um componente para tal coisa com o objetivo de melhorar tal coisa, deixando o projeto de tal maneira.

    Close #52
  ```
  - Faça um *push* para a sua *branch*: `git push origin feat/minhaFeature`;
  - Agora é só abrir um *pull request* no repositório que você fez o *fork* e assim que acontecer o *merge* sua Issue será fechada e suas alterações irão fazer parte do projeto;
  - Depois que o *merge* da sua pull request for feito, você pode deletar a sua *branch*.

  \* **Obrigado por contribuir!** ❤️ :facepunch: :blush:

## **:page_with_curl:  LICENÇA**

Esse repositório está licenciado pela **MIT LICENSE**. Para mais informações detalhadas, leia o arquivo [LICENSE](./LICENSE) contido nesse repositório. 

<h2 align="center">Feito com ❤️ por <a href="http://github.com/santiagoidu">Marco Tulio Santiago</a></h2>

<!-- Website Links -->

[rocketseat_site]: https://rocketseat.com.br/

<!-- Badges -->

[github_issues_badge]: https://img.shields.io/github/issues/x0n4d0/ecoleta?color=green

[repository_license_badge]: https://img.shields.io/github/license/x0n4d0/ecoleta

[node_version_badge]: https://img.shields.io/badge/node-12.17.0-green

[npm_version_badge]: https://img.shields.io/badge/npm-6.14.4-red

[web_react_badge]: https://img.shields.io/badge/web-react-blue

[mobile_react-native_badge]: https://img.shields.io/badge/mobile-react%20native-blueviolet

[server_nodejs_badge]: https://img.shields.io/badge/server-nodejs-important

<!-- Techs -->

[react]: https://reactjs.org/

[typescript]: https://www.typescriptlang.org/

[node]: https://nodejs.org/en/

[leaflet]: https://react-leaflet.js.org/en/

[ibge_api]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1

[ibge_api_ufs]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1#api-UFs-estadosGet

[ibge_api_municipios]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1#api-Municipios-estadosUFMunicipiosGet

[vscode]: https://code.visualstudio.com/

[react_native]: http://www.reactnative.com/

[stackedit]: https://stackedit.io

[vscode_sqlite_extension]: https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite

[markdown_emoji]: https://gist.github.com/rxaviers/7360908

[commitlint]: https://github.com/conventional-changelog/commitlint

[express]: https://expressjs.com/

[cors]: https://expressjs.com/en/resources/middleware/cors.html

[knex]: http://knexjs.org/

[sqlite3]: https://github.com/mapbox/node-sqlite3

[tsnode]: https://github.com/TypeStrong/ts-node

[feather_icons]: https://feathericons.com/

[insomnia]: https://insomnia.rest/

[react_leaflet]: https://react-leaflet.js.org/

[react_router_dom]: https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom

[react_icons]: https://react-icons.github.io/react-icons/

[axios]: https://github.com/axios/axios

[dotenv]: https://github.com/motdotla/dotenv

[expo]: https://expo.io/

[expo_google_fonts]: https://github.com/expo/google-fonts

[react_navigation]: https://reactnavigation.org/

[react_native_maps]: https://github.com/react-native-community/react-native-maps

[expo_constants]: https://docs.expo.io/versions/latest/sdk/constants/

[react_native_svg]: https://github.com/react-native-community/react-native-svg

[expo_location]: https://docs.expo.io/versions/latest/sdk/location/

[expo_mail_composer]: https://docs.expo.io/versions/latest/sdk/mail-composer/

[font_roboto]: https://fonts.google.com/specimen/Roboto

[font_ubuntu]: https://fonts.google.com/specimen/Ubuntu

[font_awesome]: https://fontawesome.com/

[multer]: https://github.com/expressjs/multer

[celebrate]: https://github.com/arb/celebrate

[joi]: https://github.com/hapijs/joi

[react_dropzone]: https://github.com/react-dropzone/react-dropzone

[asdf]: https://github.com/asdf-vm/asdf

[yarn]: https://classic.yarnpkg.com/en/docs/install/#debian-stable
