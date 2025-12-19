# v1.0.1
- Adicionado o módulo _electron-squirrel-startup_ para gerar atalho na área de trabalho
- Adicionada janela de splash, permitindo ao usuário selecionar entre exibir os dados do computador ou abrir um chamado
- Se a aplicação está rodando, abre a janela de splash ao tentar abrir uma nova instância. Isso impede que a aplicação rode várias vezes
- Caso usuário selecione a opção **salvar meus dados** ao gerar um chamado, traz a opção selecionada na abertura de chamado seguinte
- Deixa de exibir tabelas vazias nas informações do computador

# v1.0.2
- Implementação de novo layout (conforme desenhado pela equipe de UX)

# v1.0.3
- Mensagens de processamento, erro e sucesso passam a ser exibidas em modal
- Correções diversas de layout
- Inserida propriedade CSS para impedir a seleção de textos

# v1.0.4
- Modo escuro

# v1.0.5
- Oculta as bordas e o menu das janelas (**ALT + M** para reexibir ou ocultar o menu)
- Insere botões para alternar entre modo escuro e modo claro e fechar a janela
- Cria uma janela minimizada que permite fechar todas as janelas visíveis sem parar a execução do programa

# v1.0.6
- Correção de erro que ocorria ao pressionar **ALT + M** (janela fechava e não reabria)
- Permite exibir a janela de ferramentas do desenvolvedor (DevTools) ao pressionar **CTRL + SHIFT + I**
- Passa a buscar o ID de conexão dos programas RustDesk, Team Viewer e AnyDesk
- Insere validação da última atualização enviada para o SGC e efetua nova atualização após 10 dias

# v1.0.7
- Correção de erro que ocorria ao cadastrar novo equipamento, indicando que o UUID e número de série devem ser informados

# v1.0.8
- Alteração do retorno ao obter JSON inválido (ex.: mensagem HTML retornada pelo servidor) ou erro de conexão (ex.: site indisponível)
- Deixa de chamar a função para atualização do token caso o usuário ou token não estejam salvos nos dados da aplicação
- Passa a enviar a informação da versão ao efetuar a atualizar os dados do equipamento via tela

# v1.0.9
- Alteração da validação de aplicação configurada, efetuada ao clicar no botão Abrir Chamado na tela principal

# v1.0.10
- Passa a chamar a função para atualização de token a cada três horas e meia.

# v1.0.11
- Passa a utilizar função --get-id para obter id do RustDesk (requer privilégios administrativos)
- Correção do intervalo de atualização do token

# v1.0.12
- Ao abrir a aplicação, aguarda dois minutos antes de validar o token.
- Durante a validação, o menu listará apenas o item "Validando dados da aplicação"

# v1.1.0
- Remoção do repositório testegfo
- Caso o UUID ou número de série não sejam informados, passa a exibir a mensagem de erro retornada pelo SGC
- Versão do testegfo (1.0.43) é maior que a do SGE (1.0.12). Essa mudança de versão (para 1.1.0) possibilitará a atualização automática.

# v1.1.1
- Aplicação passa a gravar logs. O caminho e tamanho atual do log serão exibidos na tabela "Arquivo de log" na tela "Meu PC".

# v1.1.2
- Incluídas informações de placas de vídeo, monitores, impressoras e dispositivos USB

# v1.1.3
- Correção de erro [Object Object] ao abrir chamado

# v1.1.4
- Alteração na função que obtém o UUID
- Correção da informação exibida em vRAM
- Ajuste na requisição para refresh do token

# v1.1.5
- Ajuste no envio de informações para as janelas (ex.: Dark mode)
- Validação dos campos ao cadastrar um novo chamado
- Remoção da funcionalidade de exibir ou ocultar o menu (**ALT + M**)
- Ajustes na tela de configuração

# v1.1.6
- Ajustes no tratamento ao obter erro de conexão (equipamento sem Internet, SGC indisponível, etc)
- Exibição do hostname e modelo do equipamento na tela de abertura de chamado
- Tela de chamado passa a ser fechada automaticamente após a abertura do chamado
- Exibição da informação FQDN na tela de configuração
- Correção ao clicar em **usar ID** na tela de configuração

# v1.1.7
- Passa a salvar e enviar para o SGC a informação FQDN (anteriormente, era necessário efetuar a configuração do equipamento para salvar a informação)
- Personalização do texto do botão em determinadas mensagens para o usuário

# v1.1.8
- Correção de erro que impedia o cadastro de novo equipamento (o botão **Novo cadastro** não era exibido quando o equipamento não era localizado no SGC)
- Exibição de informações básicas do equipamento (UUID, Número de Série, Modelo e FQDN) na tela "Meu PC". É indicada uma mensagem caso a aplicação não esteja configurada
- Ajuste no comportamento no modal de aviso quando ação for "fechar_janela"

# v1.1.9
- Ajuste no tempo de obtenção de token quando ocorre falha na atualização
- Alteração da validação de aplicação configurada e de token obtido
- Exibição de mensagem para o usuário quando não é possível conectar ao servidor, com opção de abertura de chamado via site

# v1.1.10
- Inclusão de campo para envio de anexos na abertura do chamado
- Passa a validar parâmetros informados na inicialização, permitindo alteração da URL da API e ativar/desativar o modo debug (informações adicionais no log)
- Cria uma área para mostrar as configurações alteradas (modo debug e URL da API, indisponível se não ocorrer alterações via inicialização com parâmetros)

# v1.1.11
- Inclusão de função para efetuar testes de conexão com a Internet e SGC
- Alteração no processo de validação de aplicação configurada
- Alteração no envio de erros para a janela do usuário (passa a mandar o tipo de erro, que pode ser conexão ou credenciais)
- Passa a gravar os IDs de pré-chamados cadastrados
- Passa a enviar o log e arquivo de configuração para o SGC em determinados erros
- Passa a permitir a abertura de chamados quando a aplicação está configurada, mas não foi possível obter ou atualizar o token (deixa de exibir aplicação não configurada, erro comum quando um usuário de funcionário é desativado)
- Ajuste na função de exibição de mensagens
- Ajustes nas mensagens exibidas ao usuário

# v1.1.12
- Inclusão da tela (janela) Acompanhar Chamados, onde será possível obter o status de atendimento dos chamados abertos e também inserir comentários ou indicar que o chamado deve ser finalizado
- Se não existir atalho para o SGE na Área de Trabalho, cria o atalho automaticamente
- Tela de informações do sistema passa a exibir modal durante o carregamento
- Ao abrir uma nova instância, é verificado se uma janela já está aberta, evitando que ela seja fechada
- Ajustes na função de atualização / obtenção de token. Verificado nos logs recebidos pelo servidor que, em alguns casos, o usuário não é obtido para o processo de login
- Ajustes em mensagens salvas no log ou exibidas para o usuário

# v1.1.13
- Se o usuário estiver logado e a aplicação configurada, substitui o botão "Meu PC" por "Acompanhar Chamados" na tela principal
- Passa a solicitar o envio do log ao SGE após atualização automática dos dados
- Ao enviar os logs, remove eventual arquivo de log antigo (.old.log) existente na pasta de logs

# v1.1.14
- Remove o método alternativo utilizado na obtenção de usuário
- Limpa o intervalo de obtenção de token quando o erro recebido for relacionado às credenciais
- Ajustes nas mensagens salvas no log

# v1.1.15
- Passa a buscar o código do equipamento e código do cliente quando uma ou ambas as informações estão ausentes na configuração
- Passa a buscar dados do equipamento diariamente, a fim de verificar eventual atualização do cliente no SGC. 
- Correção de erro na montagem da URL (em alguns casos, o número de série retornado possuía espaços)