
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


