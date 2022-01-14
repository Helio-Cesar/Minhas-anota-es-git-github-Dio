#Minhas anotações - Curso Git+Github (Diginal Inovation One)
#Arquivo markdown do resuo do curso - Desafio de projeto
#Autor: Helio Silva

##Git: Repositório local(uso em seu equipamento)
###URL do site para download: http://git-scm.com
###Há versões para Windows, Linux e Mach

##Github: Repositório na nuvem (Cloud) 
###Site para cadastro de usuário e repositórios: http://gitgub.com
###Por convenção utilizar mesmo e-mail e user.name para ambos

##Gerar Chave SSH no Gitbash
###Comandos:
###SSH --keygen -t ed25519 -C <e-mail>
###Obs: Na tela será exibido caminho para chave privada e pública
###A URL apresentada deve ser copiada para o Github em campo próprio durante a criação do repositório lá

###Importante: Há equivalência de comandos windows/dos e unix/linux:
###Windows/DOS     Unix/Linux
###   dir           ls
###   cd            cd
###   type          cat
###   mkdir         mkdir
###   de/rmdir      rm -rf

##Ativar SSH Agent
###Comando1: eval $(ssh-agent -S)
###Observação: Aqui será exibido agente PID

###Comando2: ssh-add id-ed25519(chave pública)


###Nota: Caso queira efetuar um teste pode ser clonado  um repositório existente no github


##Gerando Chave Token no Github

###1-Utilizar o caminho a partir de sua foto:
###settings>developers settings>personal acess tokens

###2-Clicar em generate new token
###Digitar:nome, expiração e repo

###3-Clicar em generate token

###4-Copiar em arquivo .txt o conteúdo da chave gerada e guardar

###O github não mostrará mais a chave. Inclusive avisa isto na tela


##Configurando e-mail e user.name no git bash
###Para ajustar estes campos, execute os comandos abaixo:

####1)Indicar E-mail
####git config --global <e-mail>
####Exemplo: heliocesarosai@yahoo.com.br

####2)Retirar indicação do E-mail
####git config --global --unset <e-mail>

####3)Indicar user.name
####git config --global <user.name>
####Exemplo:helio-cesar

####4)Retirar indicação user.name
####git config --global --unset <user.name>

####Importante: Tanto o e-mail quanto o user.name devem ser os mesmos informados no github
####Isto facilita pois evita que a todo instante os informemos durante o trabalho com git github

##Após a gravação do e-mail e user.name devemos inicializar o respositório com o comando:
###git init

##Após a criação do arquivo markdown ou mesmo arquivos de código, utilize:
###1)Movimentar arquivos para a área de stage:
####git add *

###2)Realizar commit(transferir para respositório local):
####git commit -m "<mensagem de histórico>"

###3)Verificar status
####git status

###4)Indicar para o git a URL do repositório no github:
####git remote add origin <URL do github>

###5)Mostrar a URL do repositório atual
####git remote -V
####Nota: são exibidas duas linhas uma terminando com fetch e a outra com push

###6)Empurrar arquivos para o github
####git push origin master

###7)Puxar arquivos  para o git bash ou seu equipamento
####git pull origin master

###8)Clonar repositório em seu equipamento
####git clone <URL do repositório a ser clonado>



