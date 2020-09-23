#Basics comands
Create a file whitout any content

    touch <file>
New empty directory

    mkdir some-directory

Remove files

    rm <file> or rm -rf <file>
    
Remove directory empty

    rmdi

Move files or directories

    mv <file/folder> <directory>
    
   

# GIT

# Los tres estados de Git
Working Directory

    En este estado los archivos se encuentran en el repositorio, pero aún no han sido incluidos en el mismo.
Staging Area

    Se preparan los archivos para ser incluidos al repositorio.

Git Directory (repository)

    Los archivos son incluidos al repositorio con el uso de commits


Para borrar del listado de Git

    git rm <file> or git rm -f <file>
    
Agregar archivos a Staging area
    
    git add .

Retirar archivos de Staging area

    git rm --cached <file>

Add separte files

    git add <file>
   
Add messaje

    -m “Mensaje” Se le asignara un mensaje al commit. El mensaje es obligatorio para realizar el commit.

Add change to ultimate commit
    
    git commit --amend


# Proyect version Git tag

  Annotated Tags
  
    $ git tag -a v1.4 -m "my version 1.4"
    $ git tag
    v0.1
    v1.3
    v1.4
  Lightweight Tags
  
    $ git tag v1.4-lw
    $ git tag
    v0.1
    v1.3
    v1.4
    v1.4-lw
    v1.5
    
List tag

    $ git tag l
    
    
Clear tag
    
    $git tag -d <version>
   
rename tag
    $git tag -f -a 0.1 or other name version
    
View log

    $git log --oneline
    
    $git log --oneline --graph // For bifurcation, Alternate version
    or branches
    
    $git log -1 or -2 for view last commit   

View Changes

    $git log
    $git diff <numbers qfist commit second commit>
    version 1 vs version 2
    
#Back to past DANGER
Soft
 
 
    1 - $git reset --soft <sha-1>
    this only clear commit but not delete files
    this files are in staging
    
    2 - Create new commit

Mixed

    1- $git reset --mixed <sha-1>
    this clear commit and send files to work area
    2- add and commit
    
    
#Branch
 Create branch   
 
    $git branch <new name branch>
    $git branch -l
            
Delete branch

    $git branch -d <name branch>
    $git branch -D <name branch> //Force delete

Rename branch

    $git branch -m <originalName finalName>

Change branch for commits

    $git checkout <name branch>

Travel in the time commit

    1- $git checkout <sha>
    This not delete files. 
    Create virtual branch
    2- Returm
       $git checkout <branch>
    
Create branch and move it
    
    
    $git checkout -b <nameBranch>

#Merge or Blend branch to master
    
    1. Select Main branch $git checkout Master
    2. $git merge <branch name>
fast-forward message
    The changes makes in time line 
recursive. 
    Detect new changes from before Merge
  
  
#git Rebase 

#Cabeza separada

    $ git checkout -b test-branch 56a4e5c08

    ...do your thing...

    $ git checkout master
    $ git branch -d test-branch
