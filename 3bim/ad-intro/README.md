# Introdução ao Active Directory (AD)

<a name="servidor">

## Descoberta do servidor de domínio
1. Quais são todas as variáveis de ambiente do Windows? R.: `set`
2. Qual o nome de seu usuário? R.: `echo %USERNAME%`
2. Qual o nome de sua máquina? R.: `echo %COMPUTERNAME%`
3. Qual o nome do servidor de autenticação? R.: `echo %LOGONSERVER%`

## Compreensão das siglas
* DN: Nome distinto 
* CN: Nome comum
* OU: Unidade Organizacional
* DC: Componente de domínio

## Navegação no diretório de objetos do AD

## Execução de consultas

### Via linha de comando (CLI)
* Recuperar todos os registros:
  * De usuário: `dsquery user`
  * De computador: `dsquery computer`
  * De grupo: `dsquery group`

* Recuperar registros específicos:
  * De usuário: `dsquery user -name %USERNAME%`
  * De computador: `dsquery computer %COMPUTERNAME%`
  * De grupo: `dsquery group -name G_PAR_*`

### Via interface gráfica (GUI) 
1. Baixe o [AD Explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/adexplorer);
2. Conecte-se ao servidor (Você já sabe o [nome dele](#servidor));
3. Use seu [usuário](#servidor);
4. E digite a senha, que só você deve saber.

### via interface de linguagem de programação (API)
Procure no Google por: `rosettacode ad search user`

E você encontrará: https://rosettacode.org/wiki/Active_Directory/Search_for_a_user

#### Python
https://github.com/jurandysoares/explorado

```
ssh nome-sobrenome@oulu
view $(which cria-meu-usuario)
   ESC:q!
   
explorado   
  Matrícula:
  Senha (do SUAP):
  
  # Consulta a seus dados
  consulta_dados('Sua matrícula')
  seu_nome = consulta_dados('Sua matrícula')
  seu_nome.keys()
  seu_nome['mail']
  seu_nome['extensionAttribute5']
  seu_nome['displayName']
  print(seu_nome['displayName'][0])
  
  # Consulta a dados de um colega
  consulta_dados('Matrícula de um colega')
  nome_colega = consulta_dados('Matrícula de um colega')
  nome_colega.keys()
  nome_colega['mail']
  nome_colega['extensionAttribute5']
  nome_colega['displayName']
  print(nome_colega['displayName'][0])
  
  # Consulta a dados do professor
  nome_professor = consulta_dados('Matrícula do professor')
  nome_professor['mail']
  nome_professor['mobile'] 
```
