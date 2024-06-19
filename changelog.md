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