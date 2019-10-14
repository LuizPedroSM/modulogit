# Modulo GIT
> Comandos GIT

## Configurando o GIT

```sh
git config --global user.name "Luiz Pedro"
git config --global user.email "email@gmail.com"
git config --global core.editor vscode

git config user.name
git config user.email
git config --list
```

## Iniciando um repositório

```sh
cd pasta do projeto
git init
```

## Branch, README e Commit

```sh
git status
git add README.md
git add -A
git commit -m "Primeiro Commit"
git log
```

## Revertendo Modificações

```sh
git log
git branch
git commit -am "Commit junto com as modificações"
git reset --soft codigo_do_commit // volta com as alterações.
git reset --mixed codigo_do_commit // volta sem as alterações.
git reset --hard codigo_do_commit // volta para o commit escolhido perde todos os commits posteriores ao escolhido.
```

## Trabalhando com diferentes Branches

```sh
git branch
git branch nome
git checkout nome
```

## Diferença entre arquivos

```sh
git status
git diff
git diff --name-only
git diff style.css
git checkout HEAD -- style.css
```

## Conectando repositório local ao remoto

```sh
git remote add origin https://github.com/LuizPedroSM/modulogit.git
git remote
git remote -v
git push -u origin master
```

## Fazendo alterações no repositório remoto

```sh
git push origin master
```

## Ignorando arquivos do repositório (gitignore)

Crie o arquivo .gitignore e adicione o nome do arquivo que deseja ser ignorado e diretorio.

```sh
banco.sql
*.sql
*.txt
pasta/*
```

## Revertendo sem perder o código (Revert)

```sh
git revert --no-edit codigo_do_commit
```

## Deletando branches locais e remotos

#### Local

```sh
git branch -D nome
```

#### Remoto

```sh
git push origin :teste
```

## Puxando alterações de outras pessoas (pull)

```sh
git pull origin master
```

## Clonando repositórios remotos

```sh
git clone https://github.com/LuizPedroSM/modulogit

```
