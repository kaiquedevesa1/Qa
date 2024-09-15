Requisitos Funcionais (RF)

 RF001- Adicionar nova tarefa
 ● Cenário 1: Adicionar uma tarefa com sucesso
   ○ #Funcionalidade: Adicionar tarefa
   ○ #Cenário: O usuário adiciona uma nova tarefa
   ○ #Dado#:Ousuário está na página de tarefas e o campo de entrada
   da tarefa está vazio
   ○ Quando: Ousuário insere o nome da tarefa e clicar no botão
   "Adicionar"
   ○ Então: A nova tarefa deve ser exibida na lista de tarefas abaixo
   da última tarefa
 ● Cenário 2: Tentativa de adicionar uma tarefa sem nome
   ○ Funcionalidade: Adicionar tarefa
   ○ Cenário: O usuário tenta adicionar uma tarefa sem nome
   ○ Dado:Ocampodeentrada da tarefa está vazio
   ○ Quando: Ousuário tenta clicar no botão "Adicionar"
   ○ Então: O sistema deve exibir uma mensagem de erro informando
   que o nome da tarefa é obrigatório
   RF002- Remover tarefa
 ● Cenário 1: Remover uma tarefa existente
   ○ Funcionalidade: Remover tarefa
   ○ Cenário: O usuário remove uma tarefa existente
   ○ Dado:Ousuário está visualizando a lista de tarefas e a lista
   contém ao menos uma tarefa
   ○ Quando: Ousuário clica no ícone de remoção de uma tarefa
   específica
   ○ Então: A tarefa deve ser removida da lista
 ● Cenário 2: Tentativa de remover uma tarefa inexistente
   ○ Funcionalidade: Remover tarefa
   ○ Cenário: O usuário tenta remover uma tarefa que não existe
   ○ Dado:Alista de tarefas está vazia
   ○ Quando: Ousuário tenta clicar no botão de remover
   ○ Então: O sistema não deve permitir a remoção e deve exibir uma
   mensagem informando que não há tarefas para remover
   RF003- Editar tarefa
 ● Cenário 1: Editar uma tarefa existente com sucesso
   ○ Funcionalidade: Editar tarefa
   ○ Cenário: O usuário edita o nome de uma tarefa existente
   ○ Dado:Ousuário está visualizando a lista de tarefas e há uma
   tarefa selecionada para edição
   ○ Quando: Ousuário clica no botão de edição e insere um novo
   nome
   ○ Então: O nome da tarefa deve ser atualizado na lista de tarefas
 ● Cenário 2: Tentativa de editar uma tarefa sem alterar o nome
   ○ Funcionalidade: Editar tarefa
   ○ Cenário: O usuário tenta editar uma tarefa sem alterar o nome
   ○ Dado:Onomedatarefa selecionada está visível para edição
   ○ Quando: Ousuário não altera o nome e tenta salvar
   ○ Então: O sistema deve exibir uma mensagem de erro informando
   que o nome da tarefa precisa ser alterado
   RF004- Marcar tarefa como concluída
 ● Cenário 1: Marcar uma tarefa como concluída
 ○ Funcionalidade: Marcar tarefa como concluída
 ○ Cenário: O usuário marca uma tarefa como concluída
 ○ Dado:Ousuário está visualizando a lista de tarefas
 ○ Quando: Ousuário clicar no checkbox ao lado de uma tarefa
 específica
 ○ Então: A tarefa deve ser movida para a seção de tarefas
 concluídas
 ● Cenário 2: Desmarcar uma tarefa concluída
 ○ Funcionalidade: Marcar tarefa como concluída
 ○ Cenário: O usuário desmarca uma tarefa que já foi concluída
 ○ Dado:Atarefa está na seção de tarefas concluídas
 ○ Quando: Ousuário desmarcar o checkbox
 ○ Então: A tarefa deve ser movida de volta para a lista de tarefas
 ativas
 RF005- Visualizar detalhes da tarefa
 ● Cenário 1: Visualizar os detalhes de uma tarefa existente
 ○ Funcionalidade: Visualizar detalhes da tarefa
 ○ Cenário: O usuário visualiza os detalhes de uma tarefa
○ Dado:Ousuário está visualizando a lista de tarefas
 ○ Quando: Ousuário clica no nome de uma tarefa específica
 ○ Então: Os detalhes da tarefa devem ser exibidos em uma nova
 janela ou modal
 ● Cenário 2: Tentativa de visualizar uma tarefa inexistente
 ○ Funcionalidade: Visualizar detalhes da tarefa
 ○ Cenário: O usuário tenta visualizar os detalhes de uma tarefa
 que não existe
 ○ Dado:Alista de tarefas está vazia
 ○ Quando: Ousuário tenta clicar em uma tarefa
 ○ Então: O sistema deve exibir uma mensagem informando que
 não há detalhes para exibir
 Requisitos Não Funcionais (RNF)
 RNF001- Desempenho do sistema de login
 ● Cenário 1: Tempo de resposta aceitável
 ○ Funcionalidade: Sistema de Login
 ○ Cenário: Tempo de resposta do sistema de login
 ○ Dado:Ousuário insere credenciais de login válidas
 ○ Quando: Ousuário clica no botão "Entrar"
○ Então: O sistema deve autenticar o usuário e conceder acesso
 emmenos de 2 segundos
 ● Cenário 2: Tempo de resposta fora do aceitável
 ○ Funcionalidade: Sistema de Login
 ○ Cenário: Tempo de resposta lento no login
 ○ Dado:Ousuário insere credenciais válidas
 ○ Quando: Osistema demora mais de 2 segundos para autenticar
 ○ Então: O sistema deve exibir uma mensagem de erro ou aviso
 sobre o tempo de resposta excedido
 RNF002- Responsividade do sistema
 ● Cenário 1: Interface ajustada para dispositivos móveis
 ○ Funcionalidade: Interface responsiva
 ○ Cenário: O sistema é acessado em um dispositivo móvel
 ○ Dado:Ousuário está acessando o sistema de um dispositivo
 móvel
 ○ Quando: Ousuário visualiza a interface
 ○ Então: A interface deve se ajustar automaticamente para uma
 exibição otimizada em telas menores
 ● Cenário 2: Interface não otimizada para dispositivos móveis
 ○ Funcionalidade: Interface responsiva
 ○ Cenário: O sistema não se ajusta corretamente
 ○ Dado:Ousuário está acessando o sistema de um dispositivo
 móvel
 ○ Quando: Ousuário visualiza a interface
○ Então: O sistema deve exibir uma mensagem de erro ou
 comportamento inadequado ao renderizar em telas pequenas
 RNF003- Disponibilidade do sistema
 ● Cenário 1: Sistema disponível durante horários de pico
 ○ Funcionalidade: Alta disponibilidade do sistema
 ○ Cenário: O sistema é acessado durante horários de pico
 ○ Dado:Osistema está em operação durante o horário de pico
 ○ Quando: Umgrande número de usuários tentam acessar
 simultaneamente
 ○ Então: O sistema deve continuar operando sem interrupções
 ● Cenário 2: Sistema indisponível durante horários de pico
 ○ Funcionalidade: Alta disponibilidade do sistema
 ○ Cenário: O sistema fica indisponível
 ○ Dado:Osistema está em operação durante o horário de pico
 ○ Quando: Umgrande número de usuários tenta acessar
 simultaneamente
 ○ Então: O sistema deve exibir uma mensagem informando que
 está fora do ar
 RNF004- Segurança dos dados
 ● Cenário 1: Dados criptografados durante a transmissão
 ○ Funcionalidade: Criptografia de dados
 ○ Cenário: O sistema processa dados sensíveis do usuário
 ○ Dado:Ousuário está inserindo dados confidenciais, como
 senhas
○ Quando: Osdados são transmitidos para o servidor
 ○ Então: Os dados devem ser criptografados durante o processo
 de transmissão
 ● Cenário 2: Falha na criptografia dos dados
 ○ Funcionalidade: Criptografia de dados
 ○ Cenário: Falha na proteção dos dados do usuário
 ○ Dado:Ousuário está inserindo dados confidenciais
 ○ Quando: Osistema não criptografa os dados corretamente
 ○ Então: O sistema deve exibir um alerta de falha de segurança
 RNF005- Escalabilidade
 ● Cenário 1: Suporte a 1.000 usuários simultâneos
 ○ Funcionalidade: Suporte a múltiplos usuários simultâneos
 ○ Cenário: O sistema suporta um grande número de usuários
 simultaneamente
 ○ Dado:Osistema está sendo acessado por 1.000 usuários ao
 mesmo tempo
 ○ Quando: Todos os usuários tentam utilizar o sistema
 ○ Então: O sistema deve suportar a carga sem perda significativa
 de desempenho
 ● Cenário 2: Falha ao suportar múltiplos usuários
 ○ Funcionalidade: Suporte a múltiplos usuários simultâneos
 ○ Cenário: O sistema não suporta um grande número de usuários
 simultâneos
○ Dado:Osistema está sendo acessado por mais de 1.000
 usuários ao mesmo tempo
 ○ Quando: Muitos usuários tentam utilizar o sistema
 ○ Então: O sistema deve apresentar lentidão ou erros de
 carregamento
 FIM
