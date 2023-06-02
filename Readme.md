Olá, esse arquivo exibe informações sobre o projeto Git que tem por objetivo ensinar o uso do software de controle de versões, **git**.
A extensão '.md' significa que o arquivo usa a linguagem de marcação **Markdown** na sua composição.
O nome 'Readme.md' é um padrão usado pelo **git** na exibição da página inicial do site **github**.

**Comandos:**  
- mostra a versão instalada em seu sistema  
$ git --version           

- inicia um repositório git vazio em sua máquina local  
$ git init                

- coloca arquivo(s) no *staging* (ante-sala do palco)  
$ git add                 

- mostra o status do *branch* com os arquivos a serem enviados ao repositório (*commit*)  
$ git status              

- faz a conexão com o repositório remoto no github  
$ git remote add origin https://github.com/kaw19/proj_git.git  

- para ignorar um arquivo já rastreado (antes mesmo de adicionar uma regra para ignorá-lo no arquivo .gitignore)
$ git rm --cached NOME_ARQ
