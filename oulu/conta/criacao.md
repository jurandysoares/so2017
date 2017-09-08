# Criação de sua própria conta
Onde você vir **nome-sobrenome**, substitua pelo nome de sua conta. Em meu caso, minha conta é **jurandy-soares**.

## Criação de conta
1. Início de sessão como estudante: `ssh estudante@oulu.ifrn.local`
2. Criação da conta: `sudo cria-meu-usuario`  (Experimente: `sudo cria-TAB`)
3. Troca da senha: `sudo troca-minha-senha` (Experimente: `sudo troca-TAB`)
4. Encerramento da sessão de estudante: `exit`

## Acesso à conta
* Início de sessão com seu usuário: 
```
ssh -XY nome-sobrenome@oulu.ifrn.local
    \_/ \____________/ \_____________/
     1         2              3
     
1: Habilita a execução de aplicações gráficas remotas
2: Substitua pelo nome de seu usuário
3: No laboratório de rede, utilize somente *oulu* ou *oulu.ifrn.lab*
```
