aca voy a poner todos lo codigos con su nombre y para que se utilizan 
registrar cambios y consultar historial 
todo x consola terminal se escribe  para manejo opertivo o uso crear o moverno listar 
git init .  iniciar el estado repositoriao para parame en la carpeta o se crea para armar el repositoriao
git status para ver nosotros como va cmabiando todo el tiempo 
cambiaos o comits vemos hoy working directory > area o estado donde se crea archivos no queda guardado nada aca  se lo para a la area de preparacion 

stagins area esta es la area de preparacion x que capas que quieres dejarlo para almacenar o no  de aca podemos paras a area de trabajo y volver despues en el repositorio no  
repository
si mandas en el comit y le das que si en este ya si lo guardas 
git add . mandas a area intermedia sacar del directorio de trabajo al area intermedia  si pones el punto pones el nombre del archivo lo mandas al area intermedia y ya estaria para el proximo comit 
para confirmar los cambio se usa  git commit .  cuanto lo pones a esto ya queda guardado y no puedes volver de eso ahi uno 
se pone commit -m "mensaje claro y espesifico son aca x ejemplo se cambio tal cosa  "
git log .  se ve los comit con estos que cambiamos los commit de letras y numeros cambiados 
git reset . este se lo usa para el area intermedia para volver del aarea intermedia al directorio de trabajo para que pase al commit o no  con el nombre del archivo.   

untraked files todas los archivos que no estan preparados para el commits 
[master (root-commit) be4f8c0] creacion del archivo llamado.txt
tambien puedes usara para agregar en esto si lo agregar a un  git log --oneline en una linea en ingles se lo ve 
pwd se vre aca los documento del arcrhivo ahi dentro de todso ls - l es la lista git status veo y se ve como estan ahi los commits se lo agrega con git add . de ahi git status . git log 
andreacampos@MacBook-Air-de-ANDREA clase3 % pwd
/Users/andreacampos/Documents/git aprender/clase3
andreacampos@MacBook-Air-de-ANDREA clase3 % git init . 
hint: Using 'master' as the name for the initial branch. This default branch name
hint: will change to "main" in Git 3.0. To configure the initial branch name
hint: to use in all of your new repositories, which will suppress this warning,
hint: call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
hint:
hint: Disable this message with "git config set advice.defaultBranchName false"
Initialized empty Git repository in /Users/andreacampos/Documents/git aprender/clase3/.git/
andreacampos@MacBook-Air-de-ANDREA clase3 % git init
Reinitialized existing Git repository in /Users/andreacampos/Documents/git aprender/clase3/.git/
andreacampos@MacBook-Air-de-ANDREA clase3 % ls -l
total 8
-rw-r--r--@ 1 andreacampos  staff  1440 Oct 13 14:54 readme.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % git status 
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
andreacampos@MacBook-Air-de-ANDREA clase3 % git add .
andreacampos@MacBook-Air-de-ANDREA clase3 % git starus
git: 'starus' is not a git command. See 'git --help'.

The most similar command is
        status
andreacampos@MacBook-Air-de-ANDREA clase3 % git log 
fatal: your current branch 'master' does not have any commits yet
andreacampos@MacBook-Air-de-ANDREA clase3 % git commit -m "creacion del archivo llamado.txt " 
[master (root-commit) be4f8c0] creacion del archivo llamado.txt
 1 file changed, 17 insertions(+)
 create mode 100644 readme.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % git log
commit be4f8c089da656c60e918600462d50aa5df986b4 (HEAD -> master)
Author: Andrea Campos <jacano1010@gmail.com>
Date:   Tue Oct 13 15:00:37 2026 -0300

    creacion del archivo llamado.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % ls -l
total 16
-rw-r--r--@ 1 andreacampos  staff     1 Oct 13 15:05 README.md
-rw-r--r--@ 1 andreacampos  staff  1579 Oct 13 15:01 readme.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

no changes added to commit (use "git add" and/or "git commit -a")
andreacampos@MacBook-Air-de-ANDREA clase3 % git add .
andreacampos@MacBook-Air-de-ANDREA clase3 % git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   README.md
        modified:   readme.txt

andreacampos@MacBook-Air-de-ANDREA clase3 % git commit -m "se cambio el nombre archvo y agregue una "
[master 44cb3e6] se cambio el nombre archvo y agregue una
 2 files changed, 3 insertions(+), 1 deletion(-)
 create mode 100644 README.md
andreacampos@MacBook-Air-de-ANDREA clase3 % git log
commit 44cb3e69cb2885c467b75fe8cb315de7bbe34a13 (HEAD -> master)
Author: Andrea Campos <jacano1010@gmail.com>
Date:   Tue Oct 13 15:10:04 2026 -0300

    se cambio el nombre archvo y agregue una

commit be4f8c089da656c60e918600462d50aa5df986b4
Author: Andrea Campos <jacano1010@gmail.com>
Date:   Tue Oct 13 15:00:37 2026 -0300

    creacion del archivo llamado.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % git log --
commit 44cb3e69cb2885c467b75fe8cb315de7bbe34a13 (HEAD -> master)
Author: Andrea Campos <jacano1010@gmail.com>
Date:   Tue Oct 13 15:10:04 2026 -0300

    se cambio el nombre archvo y agregue una

commit be4f8c089da656c60e918600462d50aa5df986b4
Author: Andrea Campos <jacano1010@gmail.com>
Date:   Tue Oct 13 15:00:37 2026 -0300

    creacion del archivo llamado.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % git log --oneline
44cb3e6 (HEAD -> master) se cambio el nombre archvo y agregue una
be4f8c0 creacion del archivo llamado.txt
andreacampos@MacBook-Air-de-ANDREA clase3 % 