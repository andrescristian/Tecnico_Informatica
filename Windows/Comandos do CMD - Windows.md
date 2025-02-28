Conteúdo deste arquivo<br>
1º_Desktop <br>
2º_Rede <br>
3º_Gerenciamento de Políticas de Grupo <br>


<h3>1º_Desktop</h3>

#_Faz o reparo de arquivos corrompidos ou ausentes do sistema

    sfc /scannow

<br>    

#_Verifica o status e dados estatísticos da bateria (No caso de notebook). Ao executar este comando, sua saída cria um arquivo de um relatório da bateria

    powercfg /batteryreport

<br>

#_Faz checagem do disco (reparo de endereçamento, configuração do Windows, ...)

    chkdsk /f

<br>

#_Faz a procura de setores defeituosos físicos no HDD/SSD, salvando recursos positivos e isolando os problemas encontrados

    chkdsk /r

<br>

#_Mostra os Processos/Tarefas em execução no sistema

    tasklist

<br>

#_Faz o encerramento de um Processo pelo PID

    taskkill /PID [nº do PID]

<br>

#_Força o encerramento de um Processo pelo PID

    taskkill /F /PID [nº do PID]

<br>

#_Verifica se os softwares instalados estão atualizados

    winget upgrade

<br>

#_Atualiza os softwares desatualizados

    winget upgrade --all

<br>

#_Redefine a pilha Winsock (Windows Sockets) para o estado original. A pilha Winsock é responsável pela comunicação de rede (internet) no Windows

    netsh winsock reset

<br>


<h3>2º_Rede</h3>

#_Verifica a conectividade com qualquer endereço IP. Essencial para teste de conexão de internet

    ping [IP ou Domínio]

<br>

#_Rastreia a rota do IP

    tracert [IP ou Domínio]

<br>

#_Mostra as conexões TCP/IP ativas

    netstat

<br>

#_Mostra os Endereços MAC de cada adaptador de rede (Placa de Rede Ethernet ou Adaptador Wi-fi)

    getmac

<br>

#_Mostra todas as informações das configurações de rede do computador

    ipconfig /all

<br>

#_Mostra o cache de DNS

    ipconfig /displaydns

<br>

#_Limpa o cache de DNS

    ipconfig /flushdns

<br>


<h3>3º_Gerenciamento de Políticas de Grupo</h3>

#_Força a atualização das Políticas de Grupo (GPOs, ou Group Policy Objects) no Windows, seja no meu computador ou na rede, políticas locais ou de um servidor de domínio

    gpupdate /force

<br>

#_Mostra as informações sobre as GPOs aplicadas, como nome do usuário, nome do computador, configurações de GPO aplicadas, etc

    gpresult /r
