

Este resumo prático reúne os principais diagramas da UML e suas notações visuais mais cobrados na prova do ENADE, divididos entre visão estrutural e comportamental.

1. Diagrama de Classes (Visão Estrutural)

Representa a estrutura estática do sistema, mostrando classes, atributos, métodos e relacionamentos.

Estrutura da Classe

Uma classe é um retângulo dividido em três compartimentos: Nome, Atributos e Métodos.
• Visibilidade: + Público (public), - Privado (private), # Protegido (protected), ~ Pacote (package).
• Sublinhado: Indica membro estático (static).
• Itálico: Indica classe ou método abstrato.

Relacionamentos e Notações


Tipo	Notação Visual	Significado
Associação	Linha contínua (———)	Conexão estrutural entre classes. Pode ter setas de navegabilidade (—>).
Agregação	Losango vazio na ponta (◇———)	Relação "todo-parte" fraca. A parte existe sem o todo (ex: Time e Jogador).
Composição	Losango preenchido na ponta (◆———)	Relação "todo-parte" forte. Se o todo é apagado, a parte também é (ex: Pedido e Item).
Herança (Generalização)	Linha contínua com triângulo vazio (———▷)	Subclasse herda da superclasse (relação "é um").
Realização (Interface)	Linha tracejada com triângulo vazio (- - -▷)	Classe implementa os contratos de uma interface.
Dependência	Linha tracejada com seta aberta (- - ->)	Uso temporário (ex: uma classe recebe outra como parâmetro de método).


Multiplicidade (Cardinalidade)

Fica nas extremidades das linhas de associação: 1 (exatamente um), 0..1 (zero ou um), 0..* ou * (zero ou muitos), 1..* (um ou muitos).

2. Diagrama de Casos de Uso (Visão Comportamental)

Descreve as funcionalidades do sistema sob o ponto de vista do usuário externo.
• Ator (Boneco palito): Papel desempenhado por usuário ou sistema externo que interage com o sistema.
• Caso de Uso (Elipse): Funcionalidade ou objetivo entregue pelo sistema (sempre escrito com verbo no infinitivo, ex: Emitir Nota Fiscal).
• Limite do Sistema (Retângulo): Envolve os casos de uso, deixando os atores do lado de fora.
• <<include>> (Seta tracejada): Inclusão obrigatória. A seta aponta do caso base para o caso incluído (ex: Realizar Pagamento ---> Validar Cartão).
• <<extend>> (Seta tracejada): Comportamento opcional ou condicional. A seta aponta do caso de extensão para o caso base (ex: Aplicar Cupom ---> Finalizar Compra).

3. Diagrama de Sequência (Visão de Interação)

Mostra a ordem cronológica da troca de mensagens entre objetos.
• Linha de Vida (Lifeline): Retângulo no topo com uma linha vertical tracejada abaixo representando o tempo.
• Barra de Ativação: Retângulo estreito sobre a linha de vida indicando o período em que o objeto está executando uma ação.
• Mensagem Síncrona (———▶): Linha contínua com ponta cheia. O remetente pausa e espera a resposta.
• Mensagem Assíncrona (———>): Linha contínua com ponta aberta (em "V"). O remetente envia e continua sem esperar.
• Mensagem de Retorno (<- - -): Linha tracejada com ponta aberta indicando o retorno de uma chamada.
• Fragmentos Combinados (Caixas no diagrama): alt (condicional if/else), opt (opcional if), loop (repetição for/while).

4. Diagrama de Atividades (Visão Comportamental)

Funciona como um fluxograma avançado para modelar processos de negócio e algoritmos.
• Nó Inicial: Círculo preto preenchido (●).
• Nó Final de Atividade: Círculo preto com borda externa (◉).
• Ação/Atividade: Retângulo com cantos arredondados.
• Nó de Decisão / Fusão (Decision / Merge): Losango (◇). Saídas possuem condições de guarda entre colchetes, como [saldo >= valor].
• Bifurcação e União (Fork / Join): Barra preta grossa (▬). Divide um fluxo em ações paralelas simultâneas (fork) ou sincroniza fluxos paralelos antes de seguir (join).
• Raias (Swimlanes): Colunas ou linhas que dividem o diagrama para mostrar qual ator ou departamento é responsável por cada ação.

5. Diagrama de Máquina de Estados (Visão Comportamental)

Modela o ciclo de vida e as mudanças de estado de um único objeto diante de eventos.
• Estado: Retângulo com cantos arredondados representando uma situação duradoura do objeto (ex: Aguardando Pagamento, Enviado).
• Transição: Seta contínua (—>) ligando um estado a outro.
• Rótulo da Transição: Segue a sintaxe evento [condição de guarda] / ação (ex: pagar [valor correto] / emitirRecibo()).
Agora que você tem a base teórica e questões comentadas, como prefere continuar sua preparação?
• Gerar um simulado interativo com questões inéditas no estilo ENADE para testar seus conhecimentos?
• Aprofundar em algum diagrama específico onde você tenha mais dificuldade?
Se quiser o simulado, me diga quantas questões (até 25) você gostaria de resolver agora.

