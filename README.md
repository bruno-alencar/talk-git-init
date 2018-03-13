# Git init

## O que é git?
 *"Git é um sistema de controle de versão de arquivos. Através deles podemos desenvolver projetos na qual diversas pessoas podem contribuir simultaneamente no mesmo, editando e criando novos arquivos e permitindo que os mesmos possam existir sem o risco de suas alterações serem sobrescritas"*
 [Tableless](https://tableless.com.br/tudo-que-voce-queria-saber-sobre-git-e-github-mas-tinha-vergonha-de-perguntar/)

## git init 
Comando utilizado para iniciar um projeto git
> `git init`

## git remote add < NOME > < LINK >
Quando estamos referenciando uma origem de código de um projecto já existente na máquina
> `git remote add origin git@github.com:bruno-alencar/talk-git-init.git`

## git add < ARQUIVO >
Podemos adicionar nossos arquivos a serem comitados separadamente ou não
> `git add README.md`

ou para adicionar todos os arquivos:
> `git add .` / `git add *`

## git commit -m ""
Commits são utilizados para "gravar" um comentário para as modificações que foram feitas
> `git commit -m "First commit"`

## git branch
Criamos novas ramificações quando estamos em outra funcionalidade

![Branch](./branch.jpg "Branch example")

### listar todas as branches
> `git branch`

### criar nova branch 
> `git branch bruno`

### excluir branch
> `git branch -d bruno`

### renomear
> `git branch -m bruno brunoalencar`

## git checkout < BRANCH-NAME >
Para navegar/trocar as branches

> `git checkout bruno`

> `git checkout master`

## git push
Enviar os arquivos commitados (registrados) para o seu repositório remoto

git push origin < BRANCH-NAME >

> `git push origin dev`

## PULL REQUEST
Realizamos pull request, mais conhecido como "*PR*" quando nosso fluxo de projeto necessita de uma aprovação e revisão de código

git pull-request [-f] [TITLE|-i ISSUE|ISSUE-URL] [-b BASE] [-h HEAD]

> `git request-pull v1.0 http:.. master`

## git pull  < REPOSITORIO > < BRANCH >
Atualizar a branch local com as modificações do repositório

> `git pull origin dev`

## git merge (vai dar m#&$*@) 
Juntar/misturar as ramificações do seu repositório 

> `git merge dev`

## git ignore
Não enviar arquivos determinados para o git

Ex: arquivos de configuração com senhas

[Criador](https://www.gitignore.io)
