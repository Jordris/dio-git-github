# Comandos Prompt git bash 
- **mkdir**: cria uma pasta.
- **touch *arquivo.extensão***: cria um arquivo.
- **ls ou dir**: lista os diretórios em uma pasta.
- **cat *arquivo***: mostra o que tem dentro do arquivo.
- **echo *texto* > *arquivo***: insere o texto no arquivo desejado, se não tiver o arquivo ele cria.
- **echo *texto* >> *arquivo***: adiciona uma quebra de linha e coloca o novo texto.
- **rm -rf *arquivo-ou-pasta***: exclui o arquivo ou a pasta.

# Comandos Git e GitHub

## Configurações Básicas 

- **git config --global user.name seu-nome-no-github**: definir nome de usuário padrão para os repositórios.

- **git config --global user.email seu-email-no-github**: definir email padrão para os repositórios.

- **git config init.defaultBranch**: Verfica o nome da Branch dos repositórios locais(o padrão geralmente é master).

- **git config --global init.defaultBranch novo-nome-branch**: definir o nome da Branch padrão para os repositórios(é recomendado colocar main).




## Criação e clonagem de repositórios

### Criação:

- **git init**: transforma o diretório em um repositório git.

### Clonagem:
- **git clone link-https**: clonar repositórios do github pelo https.

- **git clone link-ssh**: clonar repositórios do github pelo ssh(é necessário [configurar a chave ssh](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh)).


## Salvando alterações no repositório local

- **git status**: verifica dentro do repositório os arquivos não rastreados na árvore de trabalho. 

- **git add *arquivo***: adiciona arquivos não rastreados para o ambiente de preparação

- **git add .** : adiciona todos os arquivos 

- Depois de adicionar os arquivos no ambiente de preparação é necessário dar um commit, ou seja, salvar as alterações do repositório.

- **git commit -m "msg do motivo"**: salva as alterações e o repositório está pronto para ser enviado para o github. 

- **.gitignore**: arquivo que ignora uma pasta ou arquivo, é necessário escrever o caminho nesse arquivo.

- Pastas vazias são ignoradas automáticamente pelo git, com isso criou-se uma convenção que é: um arquivo **.gitkeep** dentro da pasta para representar que esta pasta é realmente vazia.

## Desfazendo alterações no repositório local

- **Excluir a pasta .git**: no repositório git x, se você excluir a pasta *.git*, x não será mais um repositório git.

- **git restore *arquivo***: restaura o arquivo conforme o último commit para caso houver alterações indesejadas.

### Desfazendo Commits

- **git commit --amend -m "nova msg"**: substitui a msg do último commit pela *"nova msg"*.

- **git reset --soft *"bash do commit"***: desfaz os commits posteriores ao especificado pelo *"bash do commit"*.

- **git reset --mixed *"bash do commit"***: além de desfazer os commits, retorna os arquivos relacionados a árvore de trabalho, sendo necessário dar um *git add* para commitar novamente.

- **git reset --hard *"bash do commit"***: além de desfazer os commits, apaga os diretórios e arquivos.

- **git reflog**: mostra operações de commits feitos no repositório.

- **git reset *arquivo* ou git restore --staged**: remove o arquivo da área de preparação para a árvore de trabalho. 

## Enviando e Baixando Alterações com o Repositório Remoto

- Ao criar um novo repositório no github sem o arquivo README, o github disponibiliza o que precisa ser feito tanto para criar um novo repositório pela linha de comando quanto para enviar um existente.

- Quando são feitas alterações nos arquivos do repositório pelo github no repositório local essas alterações ainda não foram realizadas, para "puxar" essas alterações existe o comando *git pull*.

- **git remote set-url origin *novo_url_do_repositorio***: para quando precisar mudar o url do repositório.


<p align="center">Feito por João 🚀</p>
