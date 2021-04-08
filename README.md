# Visão Geral

Você pode construir aplicações integrando-se com seu backend e também pode construir backends no módulo Integration do Oracle Integration Cloud (OIC). Quando você constrói seu próprio backend dentro do Oracle Integration, você consegue ainda compartilhar e reusar estas funcionalidades com o mundo externo.
Dentro do Oracle Integration é possível desenhar processos através de notação BPMN 2.0 e automatizar as etapas integrando com backends e aplicações, implementando chamadas a telas e enviando mensagens; tornando o processo rastreável através de dashboard.

Abaixo, uma série de links úteis disponíveis na Internet para ajudar na construção de aplicações LOW-CODE.

# Visual Builder (LOWCODE Web / Mobile)
Este é o módulo de construção das aplicações Web e Mobile (iOS/Android) do Oracle Integration.

### Video Series Tutorials
Esta série de vídeos permite 
- Ter uma visão geral da estrutura do Visual Builder
- Construir uma aplicação simples para entender como customizar uma aplicação LOWCODE
- Entender como implementar vários componentes disponíveis 
https://www.youtube.com/playlist?app=desktop&list=PLSKf-atSzZeiB4mTN8163D5Ohx3DzuHcd&itct=CBEQojAYBCITCJ2k_vnmv-QCFcWjkAodiGcKUDIHcmVsbGlzdA%3D%3D&csn=GTV0XY26KczHwAT-oqqwAw&wlfg=true

### Trabalhando com temas no Visual Builder
- Look and feel da aplicação
- HTML e CSS
https://docs.oracle.com/en/cloud/paas/app-builder-cloud/tutorial-create-theme/

### Criando uma aplicação Web Simples
https://apexapps.oracle.com/pls/apex/f?p=44785:50:0:::50:P50_EVENT_ID,P50_COURSE_ID:5817,206

### Criando uma aplicação Mobile Simples
https://apexapps.oracle.com/pls/apex/f?p=44785:50:0:::50:P50_EVENT_ID,P50_COURSE_ID:5819,208

### Aplicações Multi-Lingua no Visual Builder
https://docs.oracle.com/en/cloud/paas/app-builder-cloud/tutorial-translate-app/index.html

### Criando o módulo de seleção de Línguas no Visual Builder
https://docs.oracle.com/en/cloud/paas/app-builder-cloud/tutorial-language-switcher/index.html

### Dashboards
- O tutorial para mobile para a construção de dashboards também pode ser feito para uma aplicação Web
- https://docs.oracle.com/cd/E83857_01/paas/app-builder-cloud/csapb/dashboards.html#GUID-5FA5C6B0-038E-48E3-A081-EA6A5D9AFA1C

### Incluindo Bluetooth e outras APIs de dispositivos móveis no Visual Builder Studio (iOS/Android)
- É possível implementar Bluetooth bem como outras APIs essenciais do dispositivo utilizando Cordova
- Existem várias APIs Cordova disponíveis como bibliotecas, porém sem o suporte da Oracle
- O tutorial para implementar está neste link:
	- https://docs.oracle.com/en/cloud/paas/integration-cloud/visual-developer/create-web-and-mobile-applications.html#GUID-E558B9DF-AA52-4DF4-867C-7BDEDD689C1D
- Esta é a biblioteca Bluetooth em Cordova que atende iOS e Android
	- https://github.com/don/cordova-plugin-ble-central
- Tutorial para criar um reconhecimento facial (foto) no Visual Builder 
	- https://medium.com/@vijaykumar.yenne/media-capture-using-oracle-visual-builder-for-facial-recognition-app-f5049ea2564a
	- Utilizar estes procedimentos também como fonte de informação para implementar Bluetooth

# Integração
Entende-se por integração todas as conexões para backends ou tecnologias como banco de dados, aplicações ou outras; das quais o Visual Builder necessita para a construção de aplicações Web ou Mobile.
Portanto, o passo-a-passo para conectar a um banco de dados é:
- Ter uma visão geral da estrutura do Visual Builder
	- https://www.youtube.com/watch?v=FUTU6UNPeHE&list=PLSKf-atSzZeiB4mTN8163D5Ohx3DzuHcd&index=2
- Ter uma visão geral de como implementar uma integração
	- Você pode chamar uma integração com seu backend para utilizar dentro do Visual Builder de 2 formas:
		- Configurando uma chamada direto no Visual Builder
			- https://www.youtube.com/watch?v=9VhDCQsK_SY&list=PLSKf-atSzZeiB4mTN8163D5Ohx3DzuHcd&index=18
			- https://www.youtube.com/watch?v=ohcDgAmbKL8
		- Criando uma integração (normalmente quando necessita conectar a uma tecnologia que NÃO seja REST; por exemplo, banco de dados, aplicações como SAP, trabalhar com arquivos CSV, entre outras). Esta integração é feita com o módulo de Integração descrito mais abaixo.
			- https://apexapps.oracle.com/pls/apex/f?p=44785:50:11196675345906:::50:P50_COURSE_ID,P50_EVENT_ID:344,6079
- Usar a integração implementada dentro do Visual Builder

### Construa sua primeira integração
https://apexapps.oracle.com/pls/apex/f?p=44785:50:106332613417553:::50:P50_COURSE_ID,P50_EVENT_ID:344,6079

### Integração com Bancos de Dados Oracle (similar com outros bancos, como SQL Server, DB2, MySQL)
https://www.youtube.com/watch?v=FW3WGB8z2sg
https://niallcblogs.blogspot.com/2018/12/674-oic-db-adapter-for-oracle-database.html

### Integração com aplicações on-prem (exemplo: SAP)
- É necessário a instalação de um AGENT em uma máquina na estrutura do on-prem que tenha acesso à aplicação via rede e também que esteja disponível para a Internet
- O AGENT permite acesso somente ao OIC configurado, portanto, é totalmente seguro liberar a máquina do AGENT para a Internet
- Porém, se por questões de compliance, for necessário proteger esta máquina por Firewall, basta identificar o IP do OIC e implementar o firewall

### Primeiros passos para Configurar o AGENT OIC:
https://docs.oracle.com/en/cloud/paas/integration-cloud/integrations-user/create-integration-exchange-messages-oracle-integration-and-local-host.html#GUID-F92564A0-8C6F-4C35-A5EE-B3F19571B616

### Integrando com SAP:
- Primeiro entenda como funciona uma integração
	- 
- Entenda como funcionam os adapters
	- Adapters de Integração disponíveis
		- https://docs.oracle.com/en/cloud/paas/integration-cloud/find-adapters.html
- Entenda como funciona o adapter do SAP
	- https://docs.oracle.com/en/cloud/paas/integration-cloud/sap-adapter/jco-properties-files.html

### Tipos de Autenticação
https://docs.oracle.com/en/cloud/paas/integration-cloud/rest-adapter/authentication-types.html

### OAuth 2
https://docs.oracle.com/en/cloud/paas/integration-cloud/rest-api/OAuth_useincalls.html

### Usando Funções Pré-Programadas para tratamento de Strings, Datas, Números, etc
https://docs.oracle.com/en/cloud/paas/integration-cloud/mapper-user/working-functions-operators-and-xslt-statements.html

### Customizando Funções Javascript para a Integração
- Normalmente você possui várias funções pré-programadas dentro do OIC para tratamento de strings, datas, números, etc
- Porém, algumas vezes se faz necessária alguma função muito específica, como tratamento de CPF
- Nestes casos, é possível criar funções em Javascript
- https://oracle-integration.cloud/2017/05/22/custom-functions-ics-definitive-guide-2/

# Process

### Start in Process
https://docs.oracle.com/en/cloud/paas/integration-cloud/user-processes/ready-create-web-form.html#GUID-4C894CB1-C8B8-4699-BDE4-4CBE83003AE2

### Process Tutorial
https://apexapps.oracle.com/pls/apex/f?p=44785:50:102871161032883:::50:P50_COURSE_ID,P50_EVENT_ID:142,5718

### Work with Integrations in Processes: Creating a REST Integration in a Process Application
https://apexapps.oracle.com/pls/apex/f?p=44785:52:6271126425428:::52:P52_CONTENT_ID,P52_MODULE_ID,P52_ACTIVITY_ID,P52_EVENT_ID:23452,2324,11833,5913

### Usando Processos em sua aplicação Visual Builder
https://apexapps.oracle.com/pls/apex/f?p=44785:50:0:::50:P50_EVENT_ID,P50_COURSE_ID:5995,279

# APIs

- Características de APIs na plataforma Oracle Cloud:
	- A Oracle disponibiliza o API Gateway como o gateway de APIs com os seguintes objetivos:
		- Expor os serviços de integração sob o formato REST e Open API para o mundo externo (Internet)
		- Necessidade de estabelecer mecanismos de throtling, timeouts e custom authentication
		- Necessidade de monitoramento de consumo de APIs
		- Necessidade de integrar com mecanismos de billing das APIs
	- Neste caso, é possível expor os serviços REST do Oracle Integration através do API Gateway
	- https://www.ateam-oracle.com/a-simple-guide-to-setup-api-gateway-with-oracle-integration-cloud

# Lifecycle Management - DEVOPS
https://docs.oracle.com/en/cloud/paas/visual-builder/visualbuilder-administration/set-vb-studio-developing-visual-applications.html#GUID-8317BDD9-409E-4999-87AF-503114954050
