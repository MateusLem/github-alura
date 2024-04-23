## Comandos

- ```git init``` - Inicializa o repositório local

- ```git clone <url>``` - Clona um repositório remoto para local

- ```git config --global <user.name | user.email>``` - Configura as informações do usuário

- ```git status``` - Verifica os arquivos modificados

- ```git add <./path | filename>``` - Adicionas as alterações para serem commitadas

- ```git restore <./path | filename>``` - Remove as alterações do *git add*

- ```git commit -m <mensagem>``` - Executa um commit com as informações adicionadas + breve descrição

- ```git log``` - Log de commits efetuados no projeto

- ```git push <remote_repository> <branch>``` - Envia as informações da branch do repositório local para o remoto

- ```git pull <remote_repository> <branch>``` - Recebe as informações da branch do repositório remoto para o local

- ```git restore <commit_hash>``` - Restaura o a branch local para seu estado em dado commit (alteração é apenas local)

- ```git reset --hard <commit_hash>``` - Exclui um commit desejado do log. O hash informado **DEVE** ser anterior ao que se deseja excluir. É ideal que seja executado apenas quando o commit não recebeu pull

- ```git commit --amend --no-edit``` - Altera o último commit sem a necessidade de alterar a mensagem

- ```git commit --amend -m <mensagem>``` - Altera a mensagem do último commit


## Commits

As mensagens dos commits devem ser simples e objetivas. 

- Mantenha a mensagem curta e concisa: 
A primeira linha da mensagem deve conter, no máximo, 72 caracteres. 
Caso seja necessário uma descrição adicional, você deve pular uma linha e adicionar os detalhes, como o contexto, da mudança realizada.

- Uso de verbo no infinitivo:
É comum que a mensagem do commit inicie com um verbo no infinitivo que descreva a alteração feita, como “adicionar”, “corrigir” ou “atualizar”. 
Em sequência, são adicionados detalhes concisos da mudança. Por exemplo: “Atualizar texto do título da página”.

- Evite detalhes técnicos: 
Não inclua detalhes técnicos complexos na mensagem de commit. 
Esses detalhes podem ser adicionados nos comentários de código ou na documentação.

Um commit deve ser realizado sempre que você finalizar uma tarefa específica ou resolver algum bug. 
Isso mantém o histórico de commits claro e rastreável, de modo que seja possível entender o que foi feito em cada commit.

Assim, é importante realizar commits frequentemente. 
Porém, evite realizar commits muito pequenos ou muito grandes, pois isso pode tornar difícil o seu entendimento.

**Lembre-se de nunca realizar um commit de um código que você sabe que contém bugs.**

O ideal é que o commit contenha somente código funcional.


### Co-authored
O Git oferece a possibilidade de adicionar mais de um autor a um commit. 
Para isso, após escrever a mensagem do commit, pulamos duas linhas e usamos a palavra-chave *Co-authored-by:*,
seguido do nome e e-mail associado ao GitHub de cada pessoa colaboradora.
```
$ git commit -m "Adicionar nova funcionalidade.<br><br><br>
Co-authored-by: USER1 <user1@email.com><br>
Co-authored-by: USER2 <user2@email.com>"
```


## Artigos Readme

[Artigo](https://www.alura.com.br/artigos/escrever-bom-readme?_gl=1*13y3hrp*_ga*MTc3MjU3NjE0Ny4xNzEzNjE1NzUz*_ga_1EPWSW3PCS*MTcxMzg5NTM1NS43LjEuMTcxMzg5NTc2OC4wLjAuMA..*_fplc*UjclMkZwSHc1TFltV1VBdDhrbldFYlZrWjJxZ1JzRW0lMkJ1WiUyQlpwT3NBcExJRkpMMlZFdlRFSUNpeWFqak1Jc2YwV0dSU21aWlRXMm91TlRCVTJ2T3lseFkxSFZ0SFNtR09WMHk5M3RKUWFsZDclMkJXVmozaVJVcUR6NkF3YmdhaGclM0QlM0Q)