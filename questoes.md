# Questões Comentadas de UML - ENADE

---

## Questão 1: Diagrama de Classes
**Ano:** ENADE (Edição Histórica)
**Tema:** Modelagem Orientada a Objetos / Diagrama de Classes

### Enunciado
Em um sistema de gestão acadêmica, uma `Instituição` possui vários `Campi`, e cada `Campus` oferece diversos `Cursos`. Um `Aluno` está matriculado em um único `Curso`, mas pode cursar várias `Disciplinas`. 
Qual dos relacionamentos melhor representa a ligação entre `Aluno` e `Curso` considerando que a exclusão do curso implica na remoção dos alunos vinculados a ele?

a) Agregação  
b) Composição  
c) Associação Simples  
d) Dependência  
e) Generalização  

### Resposta e Comentário
* **Resposta correta:** **b) Composição**
* **Comentário:** A composição é uma forma forte de agregação (relação "todo-parte") onde o ciclo de vida da parte (`Aluno`) está fortemente vinculado ao do todo (`Curso`). Se o enunciado dá a entender que a existência do elemento subordinado depende estruturalmente da existência do elemento principal, utiliza-se a composição (losango preenchido).

---

## Questão 2: Diagrama de Casos de Uso
**Ano:** ENADE (Edição Histórica)
**Tema:** Relacionamentos entre Casos de Uso (`<<include>>` e `<<extend>>`)

### Enunciado
No contexto da UML, analise as afirmativas sobre os estereótipos `<<include>>` e `<<extend>>` em diagramas de caso de uso:

I. O relacionamento `<<include>>` indica que o comportamento de um caso de uso base é inserido em um caso de uso explicativo ou secundário em um ponto específico.  
II. O relacionamento `<<extend>>` é utilizado para representar um comportamento que é opcional ou que acontece sob determinadas condições.  

É correto o que se afirma em:
a) Apenas I  
b) Apenas II  
c) Ambas I e II  
d) Nenhuma das afirmativas  

### Resposta e Comentário
* **Resposta correta:** **b) Apenas II** (ou conforme a variação da banca onde I inverte a direção de dependência).
* **Comentário:** O `<<include>>` aponta do caso de uso base para o caso de uso incluído (obrigatório para a execução do fluxo principal). Já o `<<extend>>` aponta do caso de uso extensão para o caso de uso base, indicando uma funcionalidade opcional/condicional.

---

## Questão 3: Diagrama de Sequência
**Ano:** ENADE (Edição Histórica)
**Tema:** Interação e Mensagens

### Enunciado
No Diagrama de Sequência da UML, uma mensagem assíncrona é representada graficamente por:

a) Uma seta com linha contínua e ponta cheia.  
b) Uma seta com linha tracejada e ponta aberta.  
c) Uma seta com linha contínua e ponta em formato de "V" aberto (meia-seta).  
d) Uma barra de rolagem vertical tracejada.  

### Resposta e Comentário
* **Resposta correta:** **c) Uma seta com linha contínua e ponta em formato de "V" aberto (meia-seta).**
* **Comentário:** Na notação UML, mensagens síncronas usam ponta de seta cheia (aguardam retorno), enquanto mensagens assíncronas usam a meia-seta (o remetente não espera o término imediato da execução para continuar).

---

## Questão 4: Diagrama de Atividades
**Ano:** ENADE (Edição Histórica)
**Tema:** Ramos de Decisão e Junção

### Enunciado
Em um Diagrama de Atividades da UML, o elemento gráfico utilizado para representar a ramificação de fluxos alternativos baseados em uma condição lógica (usando guardas) é conhecido como:

a) Nó de junção (Join)  
b) Nó de decisão (Decision Node)  
c) Barras de sincronização  
d) Raia (Swimlane)  

### Resposta e Comentário
* **Resposta correta:** **b) Nó de decisão (Decision Node)**
* **Comentário:** O nó de decisão é representado por um losango, de onde partem múltiplos fluxos com condições de guarda entre colchetes (ex: `[valor > 10]`). Diferencia-se do *fork/join* (barras pretas), que tratam de concorrência e paralelismo.
