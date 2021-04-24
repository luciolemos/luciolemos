# RESTFUL
## Olá!

[![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/luciolemos)](https://github.com/luciolemos)
[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/lucio-lemos-a550441a1/)](https://www.linkedin.com/in/lucio-lemos-a550441a1/)
[![Twitter Badge](https://img.shields.io/badge/-Twitter-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/lucciolemos)](https://twitter.com/lucciolemos)
[![Youtube Badge](https://img.shields.io/badge/-YouTube-ff0000?style=flat-square&labelColor=ff0000&logo=youtube&logoColor=white&link=https://studio.youtube.com/channel/UCrNM1nr2nw0lSqMD10m6rLw)](https://studio.youtube.com/channel/UCrNM1nr2nw0lSqMD10m6rLw)

### About me
I'm a frontend developer [www.luciolemos.com](https://www.luciolemos.com).

- [Courses](https://www.treinaweb.com.br/cursos-online?q=fagner+pinheiro) 👨🏼‍🏫 - It's are technical courses on many technologies, such as Django, Flask, Python, Kotlin, Flutter, Dart, Git and more
- [Blog](https://www.treinaweb.com.br/blog/author/fagner-pinheiro/) ✍🏼 - I'm write about many things.
- [Website](https://fagnerpsantos.dev/) 💻 - Working on it.

## 1. INICIANDO COM O yarn
    luciolemos@dev:~/nextlevelweek/restful$ yarn init -y
obs: nesse momento é gerado o arquivo "_package.json_", com o seguinte conteúdo: 
    
    {
    "name": "restful",
    "version": "1.0.0",
    "main": "index.js",
    "license": "MIT",                             
    }


## 2. ADICIONANDO O express

    luciolemos@dev:~/nextlevelweek/restful$ yarn add express
Obs; o comando acima adicionará ao arquivo "_package.json_", a seguintes dependência:

    ...
    "dependencies": {
    "express": "^4.17.1"
    }
    ...
essa dependência criará na esrutura de diretórios do projeto o diretório "_node_modules_".

## 3. ESTRUTURA FINAL DO ARQUIVO "_package.json_".
    {
    "name": "restful",
    "version": "1.0.0",
    "main": "index.js",
    "license": "MIT",
    "dependencies": {
        "express": "^4.17.1"
    }
    }

## CRIAÇÃO DO ARQUIVO "data.json" NA RAIZ DO PROJETO
Importa dados de exemplo de https://jsonplaceholder.typicode.com/users.

[Dados de exemplo](https://jsonplaceholder.typicode.com/users).


### CONSTRAINSTS (Necessidades) para ser RESTFUL
- _Cliente-server_:
- _Stateless_:
- _Cacheable_:
- _Layered System_:
- _Code om demand_:

**Exemplo de negrito**
1. Lemos
2. Flavio
3. Lucio

**Outras features**
- Lemos
- Lucio
- Flavio

**Task**

- [x]  Lucio

- [x]  Lemos


**Exemplo de Code** (inserindo "tab" à frente do paragráfo).

    function testando( ) 
    {
    var x="exelente";
    console.log;
    }
    

### Exemplo de tabela em ".md"
| A | B | C | D | E |
|:-:|:-:|:-:|:-:|:-:|
| 1 |   |   |   |   |
| 2 |   |   |   |   |
| 3 |   |   |   |   |




