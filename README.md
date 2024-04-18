# MultithreadingGo
Neste repositório, faço anotações sobre meus estudos com multithreading.

## Conceitos básicos
O multithreading é uma característica marcante do Go e é o que o torna tão rápido em sistemas robustos.

### O que são threads?
Threads são linhas de execução de processos. Cada thread é responsável por um processo específico. Por exemplo, se temos uma thread que executa um trabalho específico e demora 20 minutos para concluí-lo, com 10 trabalhos para realizar, ela levaria 200 minutos. No entanto, se adicionarmos mais 10 threads, podemos realizar os 10 trabalhos em 20 minutos. As threads utilizam concorrência para realizar essas tarefas simultaneamente.

### O que é concorrência?
Concorrência é quando threads competem entre si pelo acesso ao kernel. Em vez de uma thread ocupar totalmente o kernel, elas competem simultaneamente pelo acesso a um recurso compartilhado, permitindo a realização de tarefas distintas ao mesmo tempo. Para impedir que duas tarefas tentem consumir o mesmo recurso ao mesmo tempo, usamos um mutex, que atua como um sinal para impedir que uma thread inicie seu processo enquanto outra thread está consumindo o recurso.

### Diferença entre paralelismo e concorrência:
Paralelismo é a execução simultânea de várias tarefas em um mesmo sistema. Em um ambiente com vários núcleos ou processadores, cada tarefa pode ser executada por um núcleo diferente ao mesmo tempo, aumentando a eficiência e reduzindo o tempo de execução.

Concorrência, por outro lado, é a execução intercalada de várias tarefas em um mesmo sistema. Em um ambiente concorrente, várias tarefas compartilham o mesmo núcleo ou processador, alternando entre si para realizar diferentes partes de suas tarefas. Isso permite que o sistema gerencie e execute várias tarefas de forma aparentemente simultânea, mesmo que elas estejam competindo pelo mesmo recurso.

Assim, a principal diferença é que no paralelismo as tarefas são executadas ao mesmo tempo, cada uma em seu próprio núcleo ou processador, enquanto na concorrência as tarefas são executadas de forma intercalada, compartilhando o mesmo núcleo ou processador.
