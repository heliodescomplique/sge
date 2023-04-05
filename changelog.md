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