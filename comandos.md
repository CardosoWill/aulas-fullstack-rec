Configurando - SSH

SSH - GitBash

1 - Verificar se existe chave ssh.
ls -al ~/.ssh

2 - Adicionar uma nova chave.
ssh-keygen -t ed25519 -C "seUemail@example.com"

3 - Inicializar agente-ssh
eval "$(ssh-agent -s)"

4 - Adicionar chave ssh ao agente
ssh-add ~/.ssh/id_ed25519

5 - Copiar chave ssh
clip < ~/.ssh/id_ed25519.pub

6 - Para sdicionar a chave no github
Github - Settings - SSH and GPG keys - New SSH key - Colar - adicionar um titulo - salvar

7 - Testar conexão
ssh -T git@github.com


git rm --cached = Remove arquivos do índice, os arquivos são removidos da, mas não do diretório de trabalho.

git branch = Lista todas as branchs locais existentes

git init = Inicializa um novo repositório Git em um diretório existente e cria um subdiretório .git.

git status = Exibe o estado atual do repositório.

git add = Adiciona arquivos ao índice e prepara os arquivos específicos para o próximo commit.

git commit -m "" = Faz um commit das mudanças no índice com uma mensagem descritiva.

git merge = Realiza o merge da branch ATUAL na Branch informada

git push = Envia commits do repositório local para o repositório remoto.

git branch -D = Exclui a branch especificada.

git fetch = Baixa objetos e referências do repositório remoto.

git pull = Baixa objetos e referências do repositório remoto e mescla com a branch atual.

git checkout = Muda para a branch especificada.

git checkout -b = Cria uma nova branch e muda para ela.