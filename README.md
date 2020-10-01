T1 - Simulador de um Escalonador de Tarefas e de uma Bolsa de Valores
Parte 1) Uma das principais aplicações de filas de prioridade é em sistemas operacionais. A fila de prioridade é fundamental no escalonamento de processos para serem executados no processador (CPU). Este trabalho consiste na construção de um simulador que escalona, isto é, agenda, a execução dos processos em um processador virtual.O programa deve rodar em um laço onde cada iteração do laço corresponde a uma fatia de tempo (um slice) do CPU. Cada processo tem uma prioridade atribuída que consiste de um valor inteiro no intervalo inclusivo -20 (maior prioridade) e 19 (menor prioridade).
Dentre todos os processos a espera para serem executados em uma determinada fatia de tempo, o processador deve receber o processo com a maior prioridade disponível.
Nesta simulação, cada processo terá um tamanho associado que indica o número de fatias de tempo necessárias para o conclusão do processo. Os valores de tempo devem estar no intervalo inclusivo de 1 até 100.
 Uma vez inicializado no processador, um processo deve executar por tempo exatamente igual ao seu tamanho. Ou seja, um processo não pode ser interrompido.
O simulador deverá imprimir na tela o nome do processo sendo executado no processador a cada fatia de tempo e também deve, a cada fatia de tempo, receber exatamente um comando da enumeração abaixo:

1.       "adiciona processo nome com tempo n e prioridade p"

2.       "nenhum processo novo para adicionar agora"

As ordens devem ser escritas exatamente como na enumeração acima.

Parte 2) Um sistema de compra e venda de ações necessita processar ordens de dois tipos:

1.       "Compre 100 ações por R$x cada"

2.       "Venda 100 ações por R$x cada"

Um ordem de compra com R$x só pode ser processada caso exista uma ordem de venda com preço R$y tal que y ≤ x. De forma análoga, uma ordem de venda por R$y só pode ser processada se existe uma ordem de compra com preço R$x tal que y ≤ x.
Se uma ordem de compra ou de venda é inserida mas não pode ser processada, ela precisa aguardar uma ordem futura compatível para a mesma seja processada.
Crie um sistema que permita o processamento de compra e venda de ações em tempo O(log n).
O sistema opera em um laço onde a cada instante de tempo o usuário pode inserir uma ordem de compra ou de venda ou então não inserir nenhuma ordem (neste caso, é passada uma string vazia).
As ordens devem ser escritas exatamente como na enumeração acima onde x deve ser substituído por um valor inteiro.
Junto ao código-fonte você deve explicar a lógica do sistema (se você usou uma ou mais filas de prioridade, se usou um objeto comparator, etc.)

Observações:

Você deve usar/adaptar a versão de fila de prioridade que está em anexo nesta atividade (HeapPriorityQueue.java). Opcionalmente, você pode usar o arquivo .jar como pacote em uma IDE desde que importe a mesma implementação de fila de prioridade.
A entrega da atividade só estará aberta para aqueles que tiverem criado ou que participem de algum grupo já criado. A definição do grupo se dá através da ferramenta de auto-seleção de grupos.
Todos os arquivos, métodos e classes devem conter documentação no formato Javadoc assim como comentários e nome dos autores.
Casos de plágio receberão nota 0 e serão reportados à coordenação de curso.
A adição de testes é opcional mas fortemente recomendada.
