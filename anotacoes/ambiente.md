# Histórico de 28 de julho de 2017

## Assuntos abordados
* Variáveis de ambiente
* Copiar (`cp`), mover (`mv`), renomear (`mv`) e excluir (`rm`)
* Concatenação (`cat arq1.txt arq2.txt`) com redirecionamento de saída (`>` ou `>>`)

## Variáveis de ambiente

### Windows
1. Abrir `cmd`
2. Exibir todas as variáveis: `set`
    * `USERNAME`: Nome do usuário
    * `HOMEDRIVE`: Drive do usuário (`C:`, `D:` etc.)
    * `HOMEPATH`: Pasta base do usuário dentro do `HOMEDRIVE`
    * `COMPUTERNAME`: Nome do computador
    * `TEMP`: Pasta para arquivos temporários
    * `TMP`: Pasta para arquivos temporários
    * `PROMPT`: Aviso de comando (`$P$G`: $P -> Unidade e caminho atual; $G -> sinal de maior que. Digite `prompt /?` para saber mais)
    * `PATH`: Caminho de busca de comandos (O Windows usa `;` como separador.)
    * `PATHEXT`: Extensões que podem ser omitidas ao digitar um comando no `PATH`
    * `USERDOMAIN`: Domínio NETBIOS em que o usuário iniciou a sessão
    * `USERDNSDOMAIN`: Domínio DNS em que o usuário iniciou a sessão

3. Exibir valor de uma variável específica: `echo %VAR%` (Onde `VAR` é o identificador da variável):
    * `echo %USERNAME%`
    * `echo %COMPUTERNAME%`
    * `echo %APPDATA%`
    * `echo %PATH%`
    * `echo %PROMPT%`

### Linux
1. Abrir terminal Bash (No Ubuntu, `\<CTRL> + \<ALT> + <T>`)
2. Exibir todas as variáveis: `set`, `set | less` ou `env`
    * `USER` ou `LOGNAME` : Nome do usuário
    * `HOME`: Pasta base do usuário (Ex.: `/home/fulano` ou `/home/ifrn/fulano`)
    * `HOSTNAME`: Nome do computador
    * `PS1`: Aviso de comando (Experimente: `PS1=[\W]$ ')
    * `PATH`: Caminho de busca de comandos (O Linux usa `:` como separador)

3. Exibir valor de uma variável específica: `echo $VAR` (Onde `VAR` é o identificador da variável):
    * `echo $USER`
    * `echo $HOSTNAME`
    * `echo $PATH`
    * `echo $PS1`

## Comandos digitados no Linux
* set
* set | less
* echo $HOSTNAME
* echo $USER
* cd /var/www/html/
* ls -F1
* cd so2017/
* ls
* cd info4m
* ls
* ls -ld .
* ls 
* ls -F1
* cd ativ/
* ls
* mkdir 2017-07-28
* cd 2017-07-28/
* chmod a+rwxt .
* pwd
* echo $PS1
* PS1='bla'
* ls
* pwd
* PS1='$ '
* pwd
* PS1='[\W]$ '
* cd
* pwd
* mkdir cal
* cd cal/
* ls
* mkdir dia
* cd dia/
* ls
* mkdir manha tarde noite
* cat << FIM > index.md
# Dia
* [Manhã](./manha/)
* [Tarde](./tarde/)
* [Noite](./noite/)
FIM

* pwd
* cd /var/www/html/so2017/info4m/ativ/2017-07-28/$USER
* mkdir /var/www/html/so2017/info4m/ativ/2017-07-28/$USER
* cd /var/www/html/so2017/info4m/ativ/2017-07-28/$USER
* pwd
* mkdir diario
* cd diario/
* ls
* cd ..
* ls
* pwd
* mkdir -p diario/julho/
* cd diario/julho/
* pwd
* cd ~
* mv cal/dia/ .
* cd -
* pwd
* ls -F1
* cp -v /etc/passwd usuarios.txt
* cp /etc/group grupos.txt
* ls ~jurandy-soares/dia
* ls -d ~jurandy-soares/dia
* cat ~jurandy-soares/dia/index.md 
* cp ~jurandy-soares/dia/ 28
* ls -F1
* cp -rv  ~jurandy-soares/dia/  28
* cp -r 28 29
* cp -r 28 30
* cp -r 28 31
* ls -F1
* for ((i=0; i<30; i++)); do echo $i; done
* help for
* for ((dia=1; dia<=31; dia++)); do  cp -r 28 $dia; done
* ls
* ls -F1
* ls
* cd 28/
* ls
* rm -rf 28/
* ls
* ls -F1
* pandoc -o index.html index.md
* cat index.html 
* vim ~/dia/cabecalho.html
* vim ~/dia/rodape.html
* cat < index.html 
* cp ~jurandy-soares/dia/cabecalho.html .
* ls -F1
* cp ~jurandy-soares/dia/rodape.html .
* cat < cabecalho.html index.html rodape.html 
* cat cabecalho.html 
* cat  cabecalho.html index.html rodape.html 
* cat  cabecalho.html index.html rodape.html > pagina.html
* cat pagina.html 
* history 
* history > ../historico.txt
* mv ../historico.txt  ../../
* ls
* history 
* # Abra, no navegador Web a <pagina.html>
* # Firefox: http://oulu/so2017/[...]/nome-sobrenome/diario/julho/28/pagina.html
* pwd
* mv -i pagina.html index.html 
* cp
* ls
* pwd
* mkdir ~jurandy-soares/public_html/historico/
* history > ~jurandy-soares/public_html/historico/historico-jurandy-soares-2017-07-28-manha.txt
