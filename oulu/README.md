# Oulu
A máquina oulu é um servidor virtual onde você poderá fazer seus experimentos de SO (Sistemas Operacionais). Para utilizá-la, 
primeiro você precisa criar sua conta a partir de sua conta pre-existente na rede do IFRN.

Onde você vir **nome-sobrenome**, substitua pelo nome de sua conta. Em meu caso, minha conta é **jurandy-soares**.

## Criação de conta
1. Início de sessão como estudante: `ssh estudante@oulu.ifrn.local`
2. Criação da conta: `sudo cria-minha-conta`  (Experimente: `sudo cria-TAB`)
3. Troca da senha: `sudo troca-minha-senha` (Experimente: `sudo troca-TAB`)
4. Encerramento da sessão de estudante: `exit`

## Acesso à conta
* Início de sessão com seu usuário: `ssh nome-sobrenome@oulu.ifrn.local`

## Publicação de páginas na Intranet
* Criação de diretório *public_html*: `mkdir ~/public_html`
* Verificação da criação: `ls -F1`
* Entrada no diretório: `cd public_html`
* Publicação de conteúdo qualquer: ```
touch bla.txt ble.jpg bli.png blo.html blu.css
ls -F1
mkdir -v lorem ipsum
ls -F1
```

## Visualização de suas páginas
* Acesse, no navegador Web, o endereço http://oulu.ifrn.local/~nome-sobrenome
