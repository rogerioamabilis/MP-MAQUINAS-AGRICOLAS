# MP-MAQUINAS-AGRICOLAS

MP MAQUINAS AGRICOLAS
Índice
1 Dados Do Cliente
1.1 Observações Importantes
1.2 Dados do Cliente
1.3 Padrinhos (Principal e Secundário)
2 Produtos e Serviços
2.1 FIREWALL FORTIGATE
3 UNIDADE 03 - Area de testes
3.1 Firewall
3.2 Rede Interna
3.3 LINK
4 ACESSOS VPN - IPSEC
4.1 Internet
4.2 ANTIVIRUS
4.2.1 WATCHGUARD AD360
4.3 WATCHGUARD
4.4 DHCP
4.4.1 Rede Corporativa
4.4.2 Rede Câmeras
4.4.3 Rede Visitantes
4.5 Servidor
4.6 ACESSOS EXTERNOS
4.7 WIFI
4.7.1 CONTROLADORA UBIQUITI
4.7.2 REDES WIFI
4.8 SWITCHS GERENCIÁVEIS
4.8.1 DOCUMENTOS ONEDRIVE
Dados Do Cliente
Observações Importantes
Descrever particularidades sobre o atendimento ao Cliente
Dados do Cliente
Nome: MP MAQUINAS AGRICOLAS
CNPJ: 11.331.727/0001-78
Cliente da Cidade de IBATÉ / SP (PROXIMO A SÃO CARLOS)
OBS.: Demais dados temos no SankhyaW
Padrinhos (Principal e Secundário)
Central de Serviço
Produtos e Serviços
FIREWALL FORTIGATE
MODELO DE CONTRATO = LOCAÇÃO
FIREWALL FORTIGATE 40F


Acessos: https://mpagro.fortiddns.com:4443/
Acessos: https://201.63.216.187:4443


UNIDADE 03 - Area de testes
Firewall
Fortigate 40F: https://mpagrounid03.fortiddns.com:4443
Rede LAN da unidade: 192.168.15.0/255.255.255.0
Colaboradores: 172.16.20.1/255.255.254.0
Visitantes: 10.10.30.1/255.255.255.0
Rede Interna
Switch Cisco 24 portas: https://192.168.15.100
Ubiquiti: 192.168.15.103 (Gerenciado pela controladora)
Chave pré-compartilhada do tunel IPSEC S2S com a matriz: IDtUpADk6R741m0
LINK
AguiaNet

PPPoE
300MB
Usuário de configuração do link: mpagro2
Senha:113317
IP da WAN: 170.254.212.19
OBS: A unidade conta com um tunel IPSEC entre o firewall principal 60F pelo link da vivo onde todas as redes se enxergam

ACESSOS VPN - IPSEC
mpagro.fortiddns.com

Chave Pré-Compartilhada: nMBtaJ48G90e



Endereço: IP ESTÁTICO, 2 LINKS, UM DEDICADO E UM PPPoE
Acesso Externo: Somente a partir dos endereços da Panice ou via VPN
Internet
LINK: VIVO
201.63.216.187 / 29
LINK DEDICADO


LINK: CELIG
PPPoE
Usuário = mp.eireli1236642
Senha = 113317


LINK: AguiaNet
PPPoE
LINK DEDICADO
500MB
Usuários: mpagro
Senha:113317
ip do mikrotik: 192.168. 88.1
ANTIVIRUS
WATCHGUARD AD360
Link: https: https://wg.managedprotection.pandasecurity.com/
Usuario: ti@mpagro.com.br
Senha: Enviado e-mail para criação
Senha de desinstalação e gerenciamento: kuY#@13221$%434
85 Licenças
WATCHGUARD
  Nome: Mp Maquinas Agricola
  Usuario: mp.agricolas
  Senha: Popotinho@9724
  e-mail: infraestrutura@mpagro.com.br
  Numero: 16997967597
DHCP
Rede Corporativa
VLAN: 1

Item	Descrição
Escopo	Distribuição Ips de 192.168.168.xx à 192.168.168.xx
Exclusões	192.168.168.xxx
Opções	003 Roteador (192.168.168.1)
006 Servidores DNS (192.168.168.240)
015 Nome do Domínio DNS (mpagro.local)
Rede Câmeras
VLAN: 253
Item	Descrição
Escopo	Distribuição Ips de 192.168.253.xx à 192.168.253.xx
Exclusões	192.168.253.xxx
Opções	003 Roteador (192.168.253.1)
006 Servidores DNS (8.8.8.8)
015 Nome do Domínio DNS (mpagro.local)

Rede Visitantes
VLAN: 20
Item	Descrição
Escopo	Distribuição Ips de 192.168.20.xx à 192.168.20.xx
Exclusões	192.168.20.xxx
Opções	003 Roteador (192.168.20.1)
006 Servidores DNS (8.8.8.8)
015 Nome do Domínio DNS (mpagro.local)
Servidor
Nome da Maquina	IP	Serviços	Acesso Remoto	Observação	Sistema Operacional
SERVER2019	192.168.168.240 (Físico)	Servidor que possui o controlador de domínio (AD), DNS, Servidor de Licenças SOLIDWORKS, Servidor antigo MEGA	fechar VPN com a MP AGRO ou via porta 1000	Servidor ! tomar muito cuidado, principalmente com o serviço do SOLID WORKS	Windows Server 2019 STD
FABRICANTE = HP
MODELO SERVIDOR = HP DL380 GEN10
SERIAL NUMBER = BRL919041R
PRODUCT NUMBER = P06421-B21
PROCESSADOR = INTEL XEON SILVER 4114
MEMÓRIA = 32GB
DISCO EM RAID
ARRAY 1 = 02 DISCOS SAS 600GB DE 10K EM RAID 1 (PARTIÇÃO C:\)
ARRAY 2 = 02 DISCOS SATA 1.2 TB DE 7.2K EM RAID 1 (PARTIÇÃO D:\)

"ILO"
URL = https://192.168.168.244/
Usuário = administrator
Senha = TYQBZEVW

Domínio .: mpagro.local
Usuário .: Administrador
Senha .: Mpagro##2019
Usuário = backup
Senha = P3amdemc2

ACESSOS EXTERNOS
ACESSO TS
mpagro.fortiddns.com:1000 > 192.168.168.240
WIFI
CONTROLADORA UBIQUITI
ACESSO: https://192.168.168.240:8443/
SERVIDOR: 192.168.168.240
Perfil usuário Backup
USUÁRIO CONTROLADORA = admin
SENHA CONTROLADORA = 87If93m7KPmY

REDES WIFI
SSID = MP AGRO
Senha = #Mp@gro#
VLAN = DEFAULT
DHCP DESTA REDE NO FIREWALL FORTIGATE

SSID = MP AGRO COLABORADORES
Senha = #CelMp@agro#
VLAN = 10
DHCP DESTA REDE NO FIREWALL FORTIGATE

SSID = MP AGRO VISITANTES
Senha = #VisMp@gro#
VLAN = 20
DHCP DESTA REDE NO FIREWALL FORTIGATE
ESTA REDE ESTÁ ABERTA PORÉM PEDE SENHA ATRAVÉS DE VOUCHER UBIQUITI

SWITCHS GERENCIÁVEIS
CISCO CLOUD
URL: https://id.cisco.com/ui/v1.0/profile-ui
USUÁRIO = ti@mpagro.com.br
SENHA = 6Z0fFc6Zy1rV

SWITCHS CISCO, ACESSO VIA NAVEGADOR PARA GERÊNCIA.

Switches Cisco de IP's: 192.168.168.4, 5, 6, 238, 239, 242, 243, 245, 246, 247, 248, 249, 251, 252, 253, 254
VLANS: 1 (Corporativa), VLAN 10 (Colaboradores) e VLAN 20 (Visitantes)

Senhas antigas
Usuário: suporte
Senhas: 6Z0fFc6Zy1rV ou 6Z0fFc6Zy1rV1 ou 6Z0fFc6Zy1rV10# ou 2MAuLum4gM78

Senha nova
Usuário: suporte
Senha: 9Zw,H%X\hJDN

Nome do Switch	IP	Localização	Acesso	Observação
SWITCHCORE	192.168.168.245	DATACENTER SWITCH 1	https://192.168.168.245/	SWITCH CORE DA REDE, TODAS AS CASCATAS PASSAM POR ELE, O FIREWALL ESTÁ LIGADO NELE, E A FIBRA DA UNIDADE 2 ESTÁ NELE
SWITCH2	192.168.168.246	DATACENTER SWITCH 2	https://192.168.168.246/	
SWITCH3	192.168.168.247	DATACENTER SWITCH 2	https://192.168.168.247/	
SWITCH2	192.168.168.246	DATACENTER SWITCH 2	https://192.168.168.248/	
SWITCHENGENHARIA1	192.168.168.249	ENGENHARIA PASSAGEM	https://192.168.168.249/	
SWITCHENGENHARIA2	192.168.168.250	ENGENHARIA PASSAGEM	https://192.168.168.250/	
SWITCH GALPÃO	192.168.168.253	GALPÃO PREDIO NOVO	https://192.168.168.253/	
SWITCH 1 SEGUNDO ANDAR	192.168.168.252	SWITCH FIBRA SEGUNDO ANDAR	https://192.168.168.252/	
SWITCH 2 SEGUNDO ANDAR	192.168.168.251	SWITCH FIBRA SEGUNDO ANDAR	https://192.168.168.251/	
SWITCH 2 SEGUNDO ANDAR	192.168.168.6	SWITCH FIBRA SEGUNDO ANDAR	https://192.168.168.6/	
SWITCH 1 FUNDO GALPÃO	192.168.168.5	SWITCH 1 FUNDO GALPÃO FIBRA	https://192.168.168.5/	
SWITCH 2 FUNDO GALPÃO	192.168.168.4	SWITCH 2 FUNDO GALPÃO	https://192.168.168.4/	
SWITCH 1 PRIMEIRO ANDAR	192.168.168.250	SWITCH 1 PRIMEIRO ANDAR	https://192.168.168.250/	
SWITCH 2 PRIMEIRO ANDAR	192.168.168.254	SWITCH 2 PRIMEIRO ANDAR	https://192.168.168.254/	

DOCUMENTOS ONEDRIVE
Baixar arquivos documentações [[1]]

Baixar documentação de backup [[2]]
