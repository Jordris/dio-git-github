# Trabalhando com Branches

Criar novas branches tem vários objetivos e benefícios, incluindo:

- **Desenvolvimento Paralelo**: Branches permitem que diferentes pessoas trabalhem em partes diferentes do projeto ao mesmo tempo, sem atrapalhar umas às outras.

- **Testes e Experimentação**: Você pode usar branches para testar novas ideias ou funcionalidades sem arriscar danificar o código principal do projeto.

- **Isolamento de Recursos**: Cada branch pode conter um conjunto específico de alterações, o que facilita a revisão e a organização do trabalho em partes separadas.

- **Múltiplas Versões**: Com branches, é possível manter diferentes versões do projeto, como uma versão estável em produção e uma versão em desenvolvimento com novos recursos.

- **Revisões de Código e Colaboração**: As branches facilitam a colaboração entre membros da equipe, permitindo revisões de código antes de mesclar as alterações de volta ao código principal.

----

## Criando, Mesclando, Deletando e Tratando Conflitos das Branches

- **git checkout -b *nome-da-branch***: cria uma nova branch e já altera para essa nova branch.

- **git checkout *nome-da-branch***: Altera para a branch especificada em *"nome-da-branch"*.

- Branches trabalham de forma independente, por exemplo, no repositório existem a branch main e a teste, se você criar um arquivo novo na teste e der o commit esse arquivo não irá aparecer na branch main, é necessário mesclar as duas.

- **git merge *nome-da-branch***: mescla as branches, por precaução esteja na branch main, nesse caso seria *git merge teste*. 

- **git branch**: mostra as branches existentes no repositório.

- **git branch -v**: mostra os últimos commits  de todas as branches que existem no repositório.

- **git branch -d *nome-da-branch***: exclui a branch selecionada.

----

## Comandos úteis no dia a dia

- **git fetch origin main**: baixa as alterações do repositório remoto no repositório local sem mesclar os dois.

- **git diff *branch-1* *branch-2***: mostra as diferenças entre as branches.

- **git clone *"https"* *--branch nome-da-branch --single-branch***: clona somente a branch especificada em *"nome-da-branch"* de todo o repositório.

---

## 📚 Documentação

- Parte de Branching and Merging na referência da [documenteção git](https://git-scm.com/docs).

- Tópico 3 no livro da [documenteção git](https://git-scm.com/docs).


<p align="center">Feito por João 🚀</p>