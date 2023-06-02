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

- ignora um arquivo já rastreado (antes mesmo de adicionar uma regra para ignorá-lo no arquivo .gitignore)  
$ git rm --cached NOME_ARQ   

- cadastra variáveis globais do 'git', tais como user.name e user.email
git config --global user.name "kaw19"  
git config --global user.email "eng.claudio.fleury@gmail.com"   

* Exemplo de Erro Clássico: nome do remoto errado, faltou a extensão '.git' no URL da 'origin'
<span style="color:blue">
    PS C:\Users\profc\Desktop\disPET> git remote -v
    origin  github.com/kaw19/disPET (fetch)
    origin  github.com/kaw19/disPET (push)
    PS C:\Users\profc\Desktop\disPET> git remote add origin https://github.com/disPET.git
    error: remote origin already exists.
    PS C:\Users\profc\Desktop\disPET> git push origin master
    fatal: 'github.com/kaw19/disPET' does not appear to be a git repository
    fatal: Could not read from remote repository.

    Please make sure you have the correct access rights
    and the repository exists.
    PS C:\Users\profc\Desktop\disPET> git push origin main
    error: src refspec main does not match any
    error: failed to push some refs to 'github.com/kaw19/disPET'
    PS C:\Users\profc\Desktop\disPET> git remote add origin https://github.com/kaw19/disPET.git
    error: remote origin already exists.
    PS C:\Users\profc\Desktop\disPET> git remote remove origin
    PS C:\Users\profc\Desktop\disPET> git remote add origin https://github.com/kaw19/disPET.git
    PS C:\Users\profc\Desktop\disPET> git remote -v
    origin  https://github.com/kaw19/disPET.git (fetch)
    origin  https://github.com/kaw19/disPET.git (push)
    PS C:\Users\profc\Desktop\disPET>
  </span>

