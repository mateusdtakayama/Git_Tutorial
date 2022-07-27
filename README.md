
# Git/Github - Do Básico ao Avançado

### Comandos Básicos

| Comando | Descrição |
| --- | --- |
| `git version` | Aponta a versão do git instalada no computador |
| `git config –global user.name “Nome”` | Serve para registrar o nome do usuário que está fazendo as commits  |
| `git config –global user.email “E-mail”` | Serve para registrar o email do usuário que está fazendo as commits  |
| `git init` | Inicia o .git na pasta desejada |
| `git add *` | Adiciona todos os arquivos da pasta ao índice |
| `git commit -m “Nome da commit”` | Faz o controle de versionamento dos arquivos adicionados ao índice |
| `git diff` | Mostra a diferença entre o que foi alterado em relação a última commit |
| `git log` | Mostra os históricos das alterações |
| `git log --oneline` | Mostra os históricos das alterações em apenas uma linha |
| `git diff` | Mostra a diferença entre o que foi alterado em relação a última commit |
| `git log` | Mostra os históricos das alterações |
| `git log --oneline` | Mostra os históricos das alterações em apenas uma linha |
| `git checkout “Número da commit` | Volta a commit desejada |
| `git checkout “Arquivo` | Desfaz as alterações realizadas naquele arquivo em relação a última commit |
| `git status` | Mostra o status dos arquivos alterados/adicionados/deletados |
| `git reset --hard` | Deleta todas as alterações em relação a última commit da branch atual |
| `git clean -f` | Deleta arquivos não rastreados (não adicionados ao índice) |

### Ignorando Arquivos
`echo > .gitingore`


Este comando cria um arquivo de texto e dentro deste arquivo será escritos os arquivos que serão ignorados

#### Como ignorar os arquivos?

Caso queira ignorar os arquivos .txt na pasta com .git, escreva dentro do .gitignore `*.txt`, por exemplo.
`Teste/*.txt` para ignorar todos os txts dentro da paste “Teste”

O site abaixo pode ajudar a ignorar arquivos irrelevantes:
https://www.toptal.com/developers/gitignore

***Lembrando que o gitignore ignora apenas arquivos que não foram adicionados ao índice!!***


### Github

Para conectar o repositório local com o remoto é necessário criar uma chave SSH, para criar ela basta usar o comando abaixo no cmd:

`$ ssh-keygen -t ed25519 -C "your_email@example.com"`

Após isso entre na pasta Users > Seu usuário > .ssh > pegue a chave escrita no arquivo de texto .pub e envie no github em Settings > SSH and GPG Keys.

Agora crie um repositório no Github com o nome desejado.

Upando o repositório local no repositório remoto.

Agora que você já possui um repositório remoto criado, para upar ele no remoto basta usar os comandos abaixo na ordem:

| Comando | Descrição |
| --- | --- |
| `git init` | Inicia o .git em sua pasta |
| `git add` | Adiciona todos os arquivos da pasta ao índice  |
| `git commit -m "nome da commit"` | Faz o controle de versionamento dos arquivos adicionados ao índice  |
| `git branch -m main` | Muda o nome da branhc para main |
| `git remote add origin “link do repositorio” | Vincula o repositório local com o repositório remoto |
| `git push -u origin main` | Empurra os arquivos do repositório local para o repositório remoto |

Caso seja feita alguma alteração no repositório remoto e que não há no local, basta utilizar `git pull -u origin main`

Agora caso seja feita alguma alteração no repositório local e deseje upar no remoto, faça um `git add`, `git commit -m "nome da commit"` e `git pull -u origin main`.



