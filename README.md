# AprendendoGit

##### Setar usuário
```bash
$ git config --global user.name + "nome"
```	
##### Setar email
```bash
$ git config --global user.email  + email
```	
##### Listar configurações
```bash
$ git config --list
```
### Inicialize um repositório Git no diretório escolhido:
```bash
$ git init
```
### Conecte o repositório local com o repositório remoto:
```bash
$ git remote add origin + link repositorio
```
### Clonar repositorio
```bash
$ git clone link do repositorio
```
### Clonar uma branch especifica do repositorio
```bash
$ git clone link do repositorio --branch + nome da branch --single-branch
```
### Verificar estado dos arquivos/diretórios
```bash
$ git status
```
- Untracked files: arquivos que não subiram para o git

### Adicionar arquivo/diretório na area de preparacao

##### Adicionar um arquivo em específico
```bash
$ git add meu_arquivo.txt
```
##### Adicionar um diretório em específico
```bash
$ git add meu_diretorio
```
##### Adicionar todos os arquivos/diretórios
```bash
$ git add .
```	
### Comitar arquivo/diretório

##### Comitar um arquivo
```bash
$ git commit meu_arquivo.txt
```	
##### Comitar vários arquivos
```bash
$ git commit meu_arquivo.txt meu_outro_arquivo.txt
```
##### Comitar informando mensagem
```bash
$ git commit meuarquivo.txt -m "minha mensagem de commit"
```
### Remover arquivo/diretório

##### Remover arquivo
```bash
$ git rm meu_arquivo.txt
```
##### Remover diretório
```bash
$ git rm -r diretorio
```
### Visualizar histórico

##### Exibir histórico
	
```bash
$ git log
```    
### Desfazendo Alterações no Repositório Local

#### Como alterar a mensagem do último commit
```bash
$ git commit --amend
```
Alterando a mensagem sem abrir o editor:  
```bash
$ git commit --amend –m"nova mensagem"
```

#### Como desfazer um commit
```bash
$ git reset
```
##### Os arquivos dos commits posteriores a esse voltam para a area de preparacao
```bash
$ git reset --soft + codigo hash
```
##### Os arquivos dos commits posteriores a esse voltam para o estado de untracked files, nao foram subido para o repositorio local
```bash
$ git reset --mixed + codigo hash
```
##### Os arquivos dos commits posteriores a esse sao totalmente excluidos
```bash
$ git reset --hard + codigo hash
```

### Commitando o repositorio ao gitHub

```bash
$ git push -u origin main
```

### Atualizando o repositório local com as informações do github

```bash
$ git pull
```

### Criando uma branch

```bash
$ git checkout -b + "nome da branch"
```

### Alternando entre branchs

```bash
$ git checkout + "nome da branch ex main, teste, funcionalidade nova"
```

### Listar branchs existentes
```bash
$ git branch
```

### Listar o último commit de cada branch 
```bash
$ git branch -v
```

### Mesclando branchs (merge)
```bash
$ git merge + "nome da branch que queira mesclar a branch main/principal"
```

### Excluindo branchs
```bash
$ git branch -d + "nome da branch"
```