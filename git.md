# My Tips
## Git
#### 1. Listando arquivos e diretórios existenes no diretório corrente (luciolemos):
    luciolemos@dev:~/luciolemos$ ls -l
    total 4
    -rw-rw-r-- 1 luciolemos luciolemos 3024 abr 26 21:38 README.md

#### 2. Criando o arquivo _markdow_ git.md:

    luciolemos@dev:~/luciolemos$ touch git.md

#### 3. Adicionando git.md:
    luciolemos@dev:~/luciolemos$ git add git.md

#### 4. Realizando o commit:
    luciolemos@dev:~/luciolemos$ git commit -m"Commit"
    [main 41712ff] Commit
    1 file changed, 0 insertions(+), 0 deletions(-)
    create mode 100644 git.md

#### 5. Realizando o _push_ das alteraçãoe feitas no projeto:
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

#### 6. Carregando o diretório do projeto no VSCode:
    luciolemos@dev:~/luciolemos$ code .
