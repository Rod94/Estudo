<p align="center">
  <img src="../img/git.svg" width="300">
</p>

## Git

- `git init` é usado para inicializar o repositório Git.

- `git status` vê o estado do repositório.

- `git add` vai guardar os itens selecionados que tem na pasta.

- `git add .` vai guardar todos os itens que tem na pasta.

- `git commit -m` é o parametro para passar uma mensagem.

- `git commit -a` parametro para seguir todos os arquivos modificados.

- `git log` lista os arquivos que foram guardados com o `commit`

- `git remote add origin + 'ssh' ou 'https'` serve pra adicionar o link junto ao repositório

- `git push -u origin master` serve para empurrar do repositório local(`master`) para o repositório remoto(`origin`), só precisa fazer isso pela primeira vez, depois podemos utilizar o `git push`.

- `git commit --amend` vai abrir seu editor com o conteúdo da mensagem do último commit e você pode editar da forma que quiser.

- `git rm -rf "nome do arquivo" --cached` remove do repositorio git mas não remove o arquivo.