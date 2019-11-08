# Comandos-Git
Aqui vai alguns comandos básicos do <a href="https://git-scm.com/book/pt-br/v1/Primeiros-passos-No%C3%A7%C3%B5es-B%C3%A1sicas-de-Git" target="_blank">GIT</a> para iniciantes: ❤️

* **git init** - INICIALIZA UM REPOSITÓRIO GIT NO SEU PC

* **git clone https://isabelamazeto@bitbucket.org/isabelamazeto/teste.git** - COPIA UM REPOSITÓRIO GIT NO SEU PC - MASTER

* **git remote add origin https://github.com/IsabelaMazeto/Comandos-Git.git** - REFERENCIA UM REPOSITÓRIO GIT NO SEU PC - MASTER

* **git status** - MOSTRA O QUE TEM DE ALTERAÇÃO NA SUA BRANCH

* **git add caminho/nomeArquivo.html** - ADICIONAR ARQUIVOS ESPECÍFICOS ALTERADOS PARA O COMMIT

* **git add .** - ADICIONAR TODOS OS ARQUIVOS ALTERADOS PARA O COMMIT

* **git commit -m "Descrição"** -PARA FAZER O COMMIT DOS ARQUIVOS ALTERADOS

* **git log** - MOSTRA INFORMAÇÕES DETALHADAS DA BRANCH

* **git reset numero_do_commit_informado_no_gitlog** - PARA DESFAZER UM COMMIT

* **git push -u origin master** - SOBE SEU PROJETO PRO REPOSITÓRIO MASTER

* **git branch** - MOSTRA TODAS AS BRANCHs

* **git branch nomebranch** - PARA CRIAR UMA NOVA BRANCH

* **git checkout nomebranch** - MUDA PARA A BRANCH ESCOLHIDA

* **git branch -t nomebranch origin/nomebranch** - PARA ACESSAR UMA BRANCH JÁ EXISTENTE

* **git push -u origin nomebranch** - SOBE SEU PROJETO PRA UMA BRANCH ESPECÍFICA

* **git pull** - BAIXA AS ALTERAÇÕES DO DIRETÓRIO PRA SUA BRANCH

* **git merge master** - MERGE (fazendo o merge entre o feature atual e a master, significa juntar alterações feitas de locais diferentes)

* **git checkout -b nomebranch** - PARA EXCLUIR UMA BRANCH

## GIT FLOW:

O <a href="https://medium.com/trainingcenter/utilizando-o-fluxo-git-flow-e63d5e0d5e04" target="_blank">Git Flow</a> é uma forma organizada de fazermos o versionamento dos nossos projetos.

* **git flow init** (para iniciar o Git Flow)
* **git flow feature start NomeBranch** (para criar uma nova branch)
* **git flow feature finish NomeBranch** (para finalizar a branch e fazer o merge com a develop)
* **git flow release start 1.0.0** (para lançar uma versão)
* **git flow release finish "1.0.0"** (para finalizar a release)

Temos a master que é a branch principal, ao dar o "git flow init", ele irá criar a branch Develop que é uma cópia da Master, para podermos trabalhar nela com mais tranquilidade caso ocorra algum erro. Ao dar o comando "git flow feature start NomeBranch", este irá criar uma cópia da Develop e nesta branch você irá uma etapa do projeto, ao terminar esta etapa você finaliza essa branch, e ele irá juntar ela com a Develop, depois é só inicar outra branch de outra etapa do projeto que irá fazer. E assim vai até terminar todo o projeto e subir tudo para a Develop, depois que a Develop estiver pronta fazemos a junção com a Master que é a principal, lançando uma release (versão).
