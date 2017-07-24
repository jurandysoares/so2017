# Interpretador de comandos
Muitos sistemas computacionais possuem um interpretador de comandos por meio do qual você pode interagir. 
A principal vantagem de se utilizar um interpretador de comandos, também conhecido como Shell, esta na interatividade.
A cada comando que você digita, você obtem uma resposta. Isto facilita o aprendizado de novos comandos.

Independentemente de qual Shell você esteja utilizando, lembre-se sempre de pedir ajuda. Preferencialmente em Inglês (`help`).

## Cmd
Se você é um usuário do Sistema Operacional Windows, a maneira mais simples e mais antiga de interagir com o sistema é por meio da execução de comandos, que pode ser feita por meio do *Prompt do DOS*, também conhecido como CMD (Abreviação de COMMAND.COM). Para os mais novos, o DOS (Disk Operating System), foi o primeiro Sistema Operacional da Microsoft, 
sendo quase um avô do Windows.

Para abrir o *Prompt do DOS*, digite: 
* `<Windows> + <R>`
* `cmd`
* `<ENTER>`

**Observação:** O que está circundado por *\<>* é uma *\<Tecla>* que deve ser digitada.

Para obter uma ajuda resumida de alguns comandos básicos:
* `help`

Para obter ajuda mais detalhada de um comando: `<COMANDO> /?`
* `dir /?`

Criação, listagem e exclusão de diretórios em *Documentos* (Documents)
* `cd`
* `cd Documents`
* `dir`
* `dir /?`
* `mkdir Abra Cadabra`
* `mkdir Calendario`
* `dir`
* `rmdir Cadabra`
* `dir`

Para aprender mais, visite:
* [Command-Line Reference](https://technet.microsoft.com/en-us/library/cc754340(v=ws.11).aspx)


## Bash
Bash é o Shell padrão dos Mac OS e das principais distribuições do Sistema Operacional Linux. 
No Windows, há várias maneiras de se obter o Bash. A mais simples delas é instalando o [Git para Windows](https://git-scm.com/download/win). 

Uma vez instalado o *Git for Windows*, procure por *Git Bash*:
* `\<Windows>`
* `bash`
* `\<ENTER>`

Para obter uma ajuda resumida de alguns comandos básicos:
* `help`

Para obter ajuda mais detalhada de um comando: `<COMANDO> --help`
* `ls --help`

Criação, listagem e exclusão de diretórios em *Documentos* (Documents)
* `pwd`
* `cd Documents`
* `dir`
* `dir /?`
* `mkdir Abra Cadabra`
* `mkdir Calendario`
* `dir`
* `rmdir Cadabra`
* `dir`

Para aprender mais, visite:
* [Bash | Wikipedia](https://pt.wikipedia.org/wiki/Bash)
* [Utilitários Unix | Wikipedia](https://pt.wikipedia.org/wiki/Utilit%C3%A1rios_Unix)
 

## PowerShell
PowerShell é o interpretador de comandos mais recente para o Windows. Ele oferece várias funcionalidades que superam o 
*Prompt do DOS* e o *Bash*. Ele já vem incluso no Windows desde o Windows 7. Enquanto os comandos do Bash e do CMD são, em 
sua maioria, abreviações ou acrônimos, no PowerShell os comandos costumam ter o formato `<Verbo>-<Nome>`.

Uma executar o *PowerShell*, digite:
* `\<Windows>`
* `PowerShell`
* `\<ENTER>`

Para obter uma ajuda resumida de alguns comandos básicos:
* `help`
* `Get-Help`

Para obter ajuda mais detalhada de um comando: `Get-Help <COMANDO>`
* `Get-Help `

Criação, listagem e exclusão de diretórios em *Documentos* (Documents)
* `Get-Location`
* `Get-ChildItem Documents`
* :point_down: [...] A-FAZER [...]
* `dir`
* `dir /?`
* `mkdir Abra Cadabra`
* `mkdir Calendario`
* `dir`
* `rmdir Cadabra`
* `dir`
