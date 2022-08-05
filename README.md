# 42_school_Net_Pratice
A system administration related exercises

### Network Protocol Layers [ TCP/IP]

	- Network communication is split into layers.
	- Each layer has different protocols that operate at that layer.
	- Each layer is self-contained and only needs to know to interface with the layer above and below it.

	1) Application	[protocols: HTTP, HTTPS, DNS, SMTP, IMAP, POP]
	2) Transport	[protocols: TCP, UDP, SPX]
	3) Network		[protocols: IPv4, IPv6, ICMP]
	4) Link			[protocols: Ethernet, MAC address, network card, device drivres, WIFI standards, switches, etc...]
	5) Physical		[ethernet cables, ...]

## TCP/IP
	TCP significa "Transmission Control Protocol" e IP "Internet Protocol".
	Por mais que duas máquinas estejam conectadas à mesma rede, se não “falarem” a mesma língua, não há como estabelecer uma comunicação. Então, o TCP/IP é uma espécie de idioma que permite às aplicações conversarem entre si.

### Pilha de Protocolos
	TCP/IP é um conjunto de protocolos dividido em quato camadas que são processadas na seguinte ordem:
#### Aplicação
	Essa camada é utilizada pelos programas para enviar e receber informações de outros programas através da rede. Nela, você encontra protocolos como SMTP (para email), FTP (transferência de arquivos) e o
	famoso HTTP (para navegar na internet). 
#### Transporte e Rede
	A camada de transporte é responsável por receber os dados enviados pelo grupo acima, verificar a integridade deles e dividi-los em pacotes. Feito isso, as
	informações são encaminhadas para a camada internet, logo abaixo dela.
	Na Rede, os dados empacotados são recebidos e anexados ao endereço virtual
	(IP) do computador remetente e do destinatário. Agora é a vez dos pacotes serem, enfim, enviados pela internet. Para isso, são passados para a camada Interface.
#### Interface
	A tarefa da Interface é receber e enviar pacotes pela rede. Os protocolos utilizados nessa camada dependem do tipo de rede que está sendo utilizado. Atualmente, o mais comum é o Ethernet, disponível em diferentes velocidades.

#### Então o que é o TCP/IP
	É o conjunto de tdas a etapas citadas acima: primeiro há o recebimento das informações (camada de aplicação), depois elas são empacotadas para o formato da rede (transporte).Por fim, os dados são endereçados (rede) e enviados (interface).