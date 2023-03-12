


## Comandos básicos
- [Definindo suas credenciais](#definindo-suas-credenciais)
- [Criando um projeto com Git](#criando-um-projeto-com-git)
- [Clone um diretório que já existe](#clone-um-diretório-que-já-existe)
- [Veja quais arquivos precisam de commit](#veja-quais-arquivos-precisam-de-commit )
- [Adicionar arquivos ao commit](#adicionar-arquivos-ao-commit)
- [Fazer commit de uma alteração](#fazer-commit-de-uma-alteração)
- [Ver se existe servidor sincronizando projeto](#ver-se-existe-servidor-sincronizando-projeto)
- [Sincronizar projeto com servidor remoto](#sincronizar-projeto-com-servidor-remoto)
- [Subir projeto para servidor](#subir-projeto-para-servidor)
- [Salvar etiquetas de versionamento do código](#salvar-etiquetas-de-versionamento-do-código)
- [Subir release para servidor](#subir-release-para-servidor) 

### Definindo suas credenciais

1. Defina o nome de usuário: git config --global user.name "Nome Sobrenome" 
2. Defina seu endereço de email: git config --global user.email "email@dominio" 

### Criando um projeto com Git 

1. Navegue até a pasta do projeto
2. Inicie o git  
```markdown
git init 
```

### Clone um diretório que já existe 
```markdown
git clone <url>
```

### Veja quais arquivos precisam de commit 
```markdown
git status  
```
 
### Adicionar arquivos ao commit 
```markdown
git add <nome-do-arquivo> 
git add * [Adiciona todos os arquivos] 
```
 
### Fazer commit de uma alteração 
```markdown
git commit -m "Descrição da alteração feita" 
```

### Ver se existe servidor sincronizando projeto 
```markdown
git remote -v 
```
 
### Sincronizar projeto com servidor remoto 
```markdown
git remote add <nome-do-servidor> local-do-servidor 
```

**Exemplo**
```markdown
git remote add origin https://github.com/kerleysousa/<nome-do-repositorio>.git 
```

### Subir projeto para servidor 
```markdown
git push <servidor> <nome-brunch> 
```

**Exemplo**
```markdown
git push origin master 
```

### Salvar etiquetas de versionamento do código 
```markdown
git tag -a v0.1.0 -m "Mensagem da release"  
```

### Subir release para servidor 
```markdown
git push <servidor> v0.1.0 
```
 
