#### 1. Listando
    luciolemos@dev:~/vscode$ ls -l
#### 1. Listando
    luciolemos@dev:~/vscode$ npx create-react-app react_project
#### 1. Listando
    luciolemos@dev:~/vscode$ cd react_project
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ ls -l
    total 548
    drwxrwxr-x 1047 luciolemos luciolemos  36864 abr 27 21:22 node_modules
    -rw-rw-r--    1 luciolemos luciolemos    817 abr 27 21:21 package.json
    drwxrwxr-x    2 luciolemos luciolemos   4096 abr 27 21:21 public
    -rw-r--r--    1 luciolemos luciolemos   3362 abr 27 21:21 README.md
    drwxrwxr-x    2 luciolemos luciolemos   4096 abr 27 21:21 src
    -rw-rw-r--    1 luciolemos luciolemos 507735 abr 27 21:22 yarn.lock
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ ls -la
    total 560
    drwxrwxr-x    5 luciolemos luciolemos   4096 abr 27 21:21 .
    drwxrwxr-x    6 luciolemos luciolemos   4096 abr 27 21:18 ..
    -rw-r--r--    1 luciolemos luciolemos    310 abr 27 21:21 .gitignore
    drwxrwxr-x 1047 luciolemos luciolemos  36864 abr 27 21:22 node_modules
    -rw-rw-r--    1 luciolemos luciolemos    817 abr 27 21:21 package.json
    drwxrwxr-x    2 luciolemos luciolemos   4096 abr 27 21:21 public
    -rw-r--r--    1 luciolemos luciolemos   3362 abr 27 21:21 README.md
    drwxrwxr-x    2 luciolemos luciolemos   4096 abr 27 21:21 src
    -rw-rw-r--    1 luciolemos luciolemos 507735 abr 27 21:22 yarn.lock
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git init
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ ls -la
    total 564
    drwxrwxr-x    6 luciolemos luciolemos   4096 abr 27 21:34 .
    drwxrwxr-x    6 luciolemos luciolemos   4096 abr 27 21:18 ..
    drwxrwxr-x    7 luciolemos luciolemos   4096 abr 27 21:34 .git
    -rw-r--r--    1 luciolemos luciolemos    310 abr 27 21:21 .gitignore
    drwxrwxr-x 1047 luciolemos luciolemos  36864 abr 27 21:22 node_modules
    -rw-rw-r--    1 luciolemos luciolemos    817 abr 27 21:21 package.json
    drwxrwxr-x    2 luciolemos luciolemos   4096 abr 27 21:21 public
    -rw-r--r--    1 luciolemos luciolemos   3362 abr 27 21:21 README.md
    drwxrwxr-x    2 luciolemos luciolemos   4096 abr 27 21:21 src
    -rw-rw-r--    1 luciolemos luciolemos 507735 abr 27 21:22 yarn.lock
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git status
    No ramo master
    No commits yet
    Arquivos n??o monitorados:
    (utilize "git add <arquivo>..." para incluir o que ser?? submetido)
        .gitignore
        README.md
        package.json
        public/
        src/
        yarn.lock

    nada adicionado ao envio mas arquivos n??o registrados est??o presentes (use "git add" to registrar)
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git add .
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git status
    No ramo master
    No commits yet
    Mudan??as a serem submetidas:
    (utilize "git rm --cached <arquivo>..." para n??o apresentar)
        new file:   .gitignore
        new file:   README.md
        new file:   package.json
        new file:   public/favicon.ico
        new file:   public/index.html
        new file:   public/logo192.png
        new file:   public/logo512.png
        new file:   public/manifest.json
        new file:   public/robots.txt
        new file:   src/App.css
        new file:   src/App.js
        new file:   src/App.test.js
        new file:   src/index.css
        new file:   src/index.js
        new file:   src/logo.svg
        new file:   src/reportWebVitals.js
        new file:   src/setupTests.js
        new file:   yarn.lock

#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git commit -m "Commit_one"
    [master (root-commit) 77046b2] Commit_one
    18 files changed, 11728 insertions(+)
    create mode 100644 .gitignore
    create mode 100644 README.md
    create mode 100644 package.json
    create mode 100644 public/favicon.ico
    create mode 100644 public/index.html
    create mode 100644 public/logo192.png
    create mode 100644 public/logo512.png
    create mode 100644 public/manifest.json
    create mode 100644 public/robots.txt
    create mode 100644 src/App.css
    create mode 100644 src/App.js
    create mode 100644 src/App.test.js
    create mode 100644 src/index.css
    create mode 100644 src/index.js
    create mode 100644 src/logo.svg
    create mode 100644 src/reportWebVitals.js
    create mode 100644 src/setupTests.js
    create mode 100644 yarn.lock
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git status
    No ramo master
    nothing to commit, working tree clean
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git branch
    * master
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ ls -l
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git remote add origin https://github.com/luciolemos/react_project.git
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git branch -M main
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ git push -u origin main
    Username for 'https://github.com': luciolemos
    Password for 'https://luciolemos@github.com': 
    Enumerating objects: 22, done.
    Counting objects: 100% (22/22), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (22/22), done.
    Writing objects: 100% (22/22), 211.62 KiB | 3.25 MiB/s, done.
    Total 22 (delta 0), reused 0 (delta 0), pack-reused 0
    To https://github.com/luciolemos/react_project.git
    * [new branch]      main -> main
    Branch 'main' set up to track remote branch 'main' from 'origin'.
#### 1. Listando
    luciolemos@dev:~/vscode/react_project$ code .

