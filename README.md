# Script que substitui o CCleaner
Criado por Aurélio "Baboo"

Leia a matéria completa clicando [aqui](https://www.baboo.com.br/windows-10/conteudo-essencial-windows/script-que-substitui-o-ccleaner/%3famp)

**Executar o Script como administrador.**

Se você acompanha o meu trabalho e assiste os meus vídeos, você sabe que um dos motivos do Windows ficar lento com o tempo é o excesso de arquivos temporários que aumentam a fragmentação de arquivos no disco rígido ou SSD.

Para piorar, como esses arquivos são salvos aleatoriamente em diversos setores do disco rígido, eles também impedem que arquivos grandes consigam ser salvos sequencialmente, obrigando-os a serem salvos em partes menores, fragmentando também esses arquivos.

O resultado disso é que em pouco tempo a partição fica cheia de arquivos distribuídos em dezenas ou centenas de partes, que levam muito mais tempo para serem lidos e salvos, e com isso o Windows fica mais lento.

Embora você possa diminuir bastante esse problema usando algum programa decente de desfragmentação como o PerfectDisk, que tem a opção StealthPatrol que previne a fragmentação excessiva de arquivos, o ideal é apagar esses arquivos temporários a cada uma ou duas semanas.

Embora a Limpeza de Disco do próprio Windows ajude nisso apagando arquivos temporários do sistema operacional, arquivos do Windows Update que não são mais necessários, arquivos da Lixeira, etc., ela não apaga arquivos temporários de programas que não foram criados pela Microsoft, além dela também não apagar os arquivos temporários do navegador Edge da própria Microsoft.

O pior é que a Limpeza de Disco também não apaga arquivos temporários de navegadores de terceiros como Chrome, Firefox, Vivaldi e Brave,

sendo que esses navegadores podem manter centenas de milhares de arquivos desnecessários no computador do usuário, resultando em uma notável perda de desempenho do Windows.

Se você quer entender fragmentação mais a fundo, eu sugiro você assistir o meu vídeo aonde eu abordo isso em detalhe.

Eu já vivenciei casos aonde o usuário tinha quase meio milhão de arquivos fragmentados do Chrome, totalizando mais de 20 GB, porque nem o usuário nem o próprio Chrome apagaram esses arquivos nos últimos dois anos.

Para resolver isso, há anos eu sugiro o uso da versão gratuita do CCleaner somente para apagar arquivos temporários, algo que ele faz muito bem.

Infelizmente nos últimos anos o CCleaner se tornou cada vez mais invasivo, incluindo aí a opção de manter ele rodando na memória RAM, que é algo totalmente desnecessário e pode criar problemas de segurança e de privacidade, e por isso eu SEMPRE sugiro desabilitar a opção Limpeza Inteligente,

embora ultimamente o CCleaner é carregado automaticamente na inicialização do Windows mesmo que o usuário não tenha configurado ele para fazer isso.

Para piorar, a empresa responsável pelo CCleaner, a Avast, foi pega pela segunda vez vendendo informações dos usuários para empresas de publicidade e anunciantes.

Embora ela tenha feito isso através do conhecido antivírus dela, que fica constantemente monitorando tudo que acontece no Windows e por isso ele consegue obter todas as informações que ele quiser sem nenhuma interferência nem conhecimento do usuário, na prática a remoção dos arquivos temporários dos navegadores é algo bastante simples e não exige o uso de qualquer programa para isso, porque isso pode ser feito através do próprio navegador, embora quase ninguém faça isso.

Então a solução mais simples para isso é o usuário executar um script que apague os arquivos temporários dos navegadores bastando um duplo-clique para isso – e é exatamente isso que eu abordo nesse vídeo.

Há algum tempo eu criei um script simples que apaga apenas os arquivos de cache dos navegadores Edge Chromium, Firefox, Vivaldi, Brave e do Chrome,

além dos arquivos temporários do Windows.

Eu não incluí o navegador Opera porque eu não recomendo ele desde 2016 quando ele foi comprado por um pool de empresas chinesas que incluem a Qihoo, comprometendo a credibilidade que ele tinha antes disso.

Esse meu script não apaga cookies, histórico e senhas, porque eles são importantes e podem ser removidos através do próprio navegador, sendo que ele é um arquivo .bat com pouco mais de 150 linhas.

Script que substitui o CCleaner: Eu decidi criar um script .bat ao invés de PowerShell porque o .bat funciona em todas as versões do Windows e os comandos dele são simples de serem compreendidos.

Esse script é muito útil pois ele ajuda quem quer manter o Windows otimizado com o menor número de programas instalados. O meu script pode ser baixado nesse link, aonde você pode baixar ele completo (para os 5 navegadores), além de um script individual para cada navegador, permitindo que você baixe e execute somente aquele que te interessa.

Não existe problema algum em você baixar o script completo e executá-lo no seu computador mesmo que você utilize apenas um navegador

porque isso não vai causar nenhum problema.

Aliás, eu sempre sugeri o uso de vários navegadores ao invés de um único porque dessa maneira o seu trabalho pode ser mais organizado (aonde cada navegador acessa algum tipo de site), além de você poder se manter logado simultaneamente em várias contas do Outlook ou Gmail, por exemplo.

Qualquer um desses scripts deve ser executado via Prompt de Comando (Admin), porque se ele for executado via Prompt de Comando comum alguns comandos não funcionarão e a eliminação dos arquivos será limitada.

Você também pode executá-lo via Agendador de Tarefas caso você queira que ele seja executado automaticamente sem intervenção do usuário, como eu vou mostrar daqui a pouco.

Script que substitui CCleaner Esse é o script completo, aonde no início ele fecha o CCleaner e depois ele executa os comandos para apagar os arquivos temporários do Windows e dos cinco navegadores que eu citei agora há pouco.

Ao executar qualquer um dos scripts, os comandos dele aparecerão na janela do Prompt de Comando enquanto o script estiver em funcionamento, e essa janela se fechará automaticamente assim que o script for finalizado.

Eu não me preocupei com o visual dele porque eu me foquei no que realmente interessa, que é apagar os arquivos desnecessários, embora agora que ele se tornou público eu posso implementar algumas melhorias nas próximas versões se isso for necessário.

E nada melhor que mostrar ele funcionando na prática, aonde inicialmente eu executei o CCleaner e ele mostrou que o Edge Chromium tem 1,2 GB de arquivos de cache que podem ser apagados, o próprio Windows tem quase 3 GB, o Firefox tem 132MB, o Chrome tem 29 MB, o Brave tem 142MB e o Vivaldi tem 105 MB para serem apagados.

Script que substitui o CCleaner: no total são mais de 21 mil arquivos que podem ser apagados sem problema algum e com isso serão recuperados quase 5 GB de espaço em disco.

Daí eu clico com o botão da direita do mouse no script e escolho a opção Executar como Administrador. Feito isso o script fecha o CCleaner e começa a apagar os arquivos. Se algum dos 5 navegadores estiver aberto, ele será automaticamente fechado porque não é possível apagar todos os arquivos necessários com ele aberto.

Depois que o script foi finalizado, eu abro novamente o CCleaner e executo uma análise, aonde ele mostra que foram removidos mais de 4,7 GB de dados,

sobrando apenas 109 MB que são basicamente os cookies e histórico dos navegadores, além dos arquivos de dump do Windows – que eu sugiro não apagar pois eles são importantes para analisar eventuais problemas com o sistema operacional.

Esses arquivos que sobraram não influenciam no desempenho do Windows, porque os principais arquivos responsáveis pela alta fragmentação são os arquivos de cache que foram apagados.

Esse script funciona por usuário, ou seja, ele apaga os arquivos temporários do usuário que executou ele, mas ele não apaga os arquivos temporários de outros usuários que eventualmente também utilizem o mesmo computador fazendo login com outro usuário e senha.

O ideal é que esse script seja utilizado uma vez por semana ou a cada 15 dias, sendo que não existe NENHUMA necessidade de executá-lo diariamente porque isso não vai deixar o seu computador mais rápido.

Se você quiser executar o script e logo em seguida fazer com que ele desligue automaticamente o computador depois dele ser finalizado, sendo uma boa opção para você executar toda sexta-feira no final do dia, por exemplo, daí basta adicionar essa linha antes da última linha dele, e com isso o computador vai ser desligado 30 segundos após a finalização dele.

Outra opção é agendar o script para ser executado via Agendador de Tarefas. Então se eu quiser que ele seja executado toda sexta-feira às 17h, por exemplo, a gente abre o Agendador de Tarefas e clica em Criar Tarefa. Eu coloco o nome da tarefa “Apagar Arquivos Temporários dos Navegadores” e clico na opção de executar com privilégios mais altos, que indica que ele vai ser executado como Administrador.

Daí eu clico em Disparadores e Novo e informo quando o script vai ser executado, que é uma vez a cada duas semanas na sexta-feira às 17h, pois se fosse uma vez por semana eu colocaria UM aqui e depois clico em OK. Em Ações a gente informa o que vai ser executado, e nesse caso vai ser “iniciar um programa”

e aqui eu procuro ele e escolho o script da pasta Documentos.

Por fim eu clico em OK e pronto. A partir de agora ele vai ser executado toda 6ª feira às 17h, semana sim semana não.

Esse meu script que substitui o CCleaner pode ser atualizado e melhorado a qualquer momento, aonde ele pode ganhar novas funcionalidades, ter uma versão em PowerShell e também uma versão executável.

Com isso, os alunos dos meus cursos podem postar no Fórum do BABOO suas ideias, sugestões e mudanças para melhorar ele, porque quanto mais completo e eficiente ele for, melhor para todos.
