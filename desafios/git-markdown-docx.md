# Git, Markdown e Docx

## Material necessário:
* [Git for Windows](https://git-scm.com/download/win)
* [Pandoc](https://github.com/jgm/pandoc/releases/)

Por questão de simplicidade, já deixei estas ferramentas disponíveis em https://mange.ifrn.edu.br/so/win/

## Sumário
* [Gerar um arquivo Markdown no Gitlab](#gitlab)
* [Copiá-lo no Windows via linha de comando](#git-clone)
* [Gerar o Docx a partir do arquivo Markdown](#md2docx)
* [Gerar o Html a partir do arquivo Docx](#md2html)
* [Registrar os arquivos](#git-commit)
* [Enviar os arquivos gerados para o Gitlab](#git-push)

<a name="gitlab">
## Gerar um arquivo Markdown no Gitlab
* Crie um novo projeto no [Gitlab](https://gitlab.devops.ifrn.edu.br), e dentro deste projeto, crie um arquivo `README.md` usando a sintaxe 
da linguagem [Markdown](http://commonmark.org/help/).

<a name="git-clone">
## Copiá-lo no Windows via linha de comando
* Inicie o *Git Bash*
* `cd ~/Documents`
* `mkdir Projetos`
* `cd Projetos`
* `pwd`
* `git clone URL`
* `ls -F1`
* `cd nome-do-projeto`

<a name="md2docx">
## Gerar o Docx a partir do arquivo Markdown
* `pandoc -o README.docx README.md`

<a name="#md2html">
## Gerar o Html a partir do arquivo Markdown
* `pandoc -o README.html README.md`

Caso seu arquivo tenha emojis, experimente:
* `pandoc -o README.html -f markdown_github README.md`

<a name="git-commit">
## Registrar os arquivos no Git
* `git status`
* `git add README.html`
* `git status`
* `git add README.docx`
* `git status`
* `git diff README.md`
* `git commit -m "Geração de DOCX e HTML a partir do MD"`

<a name="git-push">
## Enviar os arquivos gerados para o Gitlab
* `git status`
* `git push`
