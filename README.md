# Principais Comandos do Git

## Configuração Inicial
- `git config --global user.name "Seu Nome"`: Define o nome do usuário que será associado aos commits.
- `git config --global user.email "seu.email@example.com"`: Define o email do usuário.

## Criação e Clonagem de Repositórios
- `git init`: Inicializa um novo repositório Git no diretório atual.
- `git clone <url-do-repositorio>`: Clona um repositório existente de uma URL.

## Comandos Básicos de Arquivos
- `git add <arquivo>`: Adiciona um arquivo específico para a área de staging.
- `git add .`: Adiciona todos os arquivos modificados para a área de staging.
- `git commit -m "mensagem do commit"`: Cria um commit com os arquivos que estão na área de staging.
- `git rm <arquivo>`: Remove um arquivo do repositório e da área de staging.

## Inspeção do Histórico
- `git status`: Mostra o estado dos arquivos no diretório de trabalho e na área de staging.
- `git log`: Exibe o histórico de commits.
- `git log --oneline`: Exibe o histórico de commits em uma linha por commit.
- `git diff`: Mostra as diferenças entre arquivos no diretório de trabalho e a área de staging.
- `git diff <branch1>..<branch2>`: Mostra as diferenças entre duas branches.

## Branching e Merging
- `git branch`: Lista todas as branches locais no repositório.
- `git branch <nome-da-branch>`: Cria uma nova branch.
- `git checkout <nome-da-branch>`: Muda para uma branch específica.
- `git checkout -b <nome-da-branch>`: Cria e muda para uma nova branch.
- `git merge <nome-da-branch>`: Mescla a branch especificada na branch atual.
- `git branch -d <nome-da-branch>`: Deleta uma branch que já foi mesclada.

## Remotos
- `git remote`: Lista os repositórios remotos configurados.
- `git remote add <nome> <url>`: Adiciona um novo repositório remoto.
- `git fetch <remote>`: Busca as atualizações do repositório remoto.
- `git pull <remote> <branch>`: Busca e mescla as atualizações do repositório remoto na branch atual.
- `git push <remote> <branch>`: Envia os commits da branch local para o repositório remoto.

## Rebasing
- `git rebase <branch>`: Rebase a branch atual no topo da branch especificada.
- `git rebase --continue`: Continua o processo de rebase após resolver conflitos.
- `git rebase --abort`: Aborta o processo de rebase e volta para o estado anterior.

## Stashing
- `git stash`: Armazena temporariamente as modificações no diretório de trabalho.
- `git stash apply`: Aplica as modificações armazenadas.
- `git stash pop`: Aplica as modificações armazenadas e as remove do stash.
