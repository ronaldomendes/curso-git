Comandos no Git Bash 

git init
Iniciar o diretório

git status
Mostrar o status dos arquivos

git add .
Adicionar todos os arquivos para envio

git commit -m "Inserir comentário"
Inserindo comentários

=============================================================

*Entrar no Github e criar um repositório

git clone "link_do_repositório" "nome_do_repositório"
Clonar um repositório

git push -u origin master
Enviando o projeto para o Github

=============================================================

git config --global user.name "Seu nome"
Configurando o nome no Git

git config --global user.email "Seu e-mail"
Configurando o e-mail no Git

git config --global core.editor "nomeEditor"
Configurando o editor

git config user.name
Mostrar o username

git config --list
Mostrar toda a configuração do Git

vim "nomeDoArquivo"
Utilizando o editor do Git.Bash --> tecle (i) para editar, (esc) para finalizar, e em seguida (:wq)

git log ou git log --decorate
Mostra quem fez as alterações

git log --author="nomeAutor"
Mostra todos os arquivos editados por uma pessoa

git shortlog
Mostra o nome e arquivos editados, em ordem alfabética

git shortlog -sn
Mostra o nome do(s) autor(es) em ordem alfabética

git log --graph
Mostra em forma gráfica

git show "códigoHash"
Mostra as edições realizadas

git diff
Mostra a modificação realizada

git diff --name-only
Mostra os arquivos modificados

git checkout "nomeArquivo"
Retorna as mudanças realizadas

git reset HEAD "nomeArquivo"
Retorna status do arquivo inserido no "git add"

git reset "(--soft, --mixed  ou --hard)" "códigoHash"

=============================================================

Adicionando uma chave SSH
https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

--> em seguida, é necessário acessar o local da chave .ssh e fazer o comando
cat id_rsa.pub

--> copiar a chave contida no arquivo e adicionar ao Github no acesso:
Settings/ SSH and GPG keys

=============================================================

git checkout -b "nome"
Cria um branch (ramificação)

git branch
Lista os branches e mostra o branch que está sendo utilizado

git checkout "nome_do_branch"
Seleciona o branch

git branch -D "nome_do_branch"
Deleta um branch

git checkout -- .
Recupera os arquivos do repositório até o último commit realizado

=============================================================

git merge "nome_do_branch"
Une um branch ao master

=============================================================

git stash
Salva as alterações de um arquivo

git stash apply 
Retornas as alterações de um arquivo

git stash list
Lista os arquivos salvos pelo stash

git stash clear
Limpa a lista de arquivos salvos
