# My Tips 📌:
## Git CLI 💻
[Git](https://git-scm.com/) é um sistema de controle de versão distribuído gratuito e de código aberto projetado para lidar com tudo, desde projetos pequenos a muito grandes com velocidade e eficiência.

#### ✔️ Listando arquivos e diretórios existenes no diretório corrente (luciolemos):
    luciolemos@dev:~/luciolemos$ ls -l
    total 4
    -rw-rw-r-- 1 luciolemos luciolemos 3024 abr 26 21:38 README.md

#### ✔️ Criando o arquivo _markdow_ git.md: 

    luciolemos@dev:~/luciolemos$ touch git.md

#### ✔️ Adicionando (stage changes) git.md: 
Este comando irá adicionar um ou mais arquivos ao controle de versionamento do git, fazendo com que todas as alterações deste arquivo sejam monitoradas posteriormente.
    
    luciolemos@dev:~/luciolemos$ git add git.md

#### ✔️ Realizando o commit:
    luciolemos@dev:~/luciolemos$ git commit -m"Commit"
    [main 41712ff] Commit
    1 file changed, 0 insertions(+), 0 deletions(-)
    create mode 100644 git.md

#### ✔️ Realizando o _push_ das alteraçãoe feitas no projeto:
    luciolemos@dev:~/luciolemos$ git push
    Username for 'https://github.com': luciolemos
    Password for 'https://luciolemos@github.com': 
    Enumerating objects: 13, done.
    Counting objects: 100% (13/13), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (8/8), done.
    Writing objects: 100% (11/11), 979 bytes | 326.00 KiB/s, done.
    Total 11 (delta 4), reused 0 (delta 0), pack-reused 0
    remote: Resolving deltas: 100% (4/4), completed with 1 local object.
    To https://github.com/luciolemos/luciolemos.git
    6133587..41712ff  main -> main

#### ✔️ Carregando o diretório do projeto no VSCode:
    luciolemos@dev:~/luciolemos$ code .

#### ✔️ Empurrando o projeto a partir de liha de comando:
    git remote add origin https://github.com/luciolemos/restful_project.git
    git branch -M main 
    git push -u origin main