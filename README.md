# MultithreadingGo
nesse repositorio faço a anotação dos meus estudos com multithreading

## Conceitos basicos
Bom ás multitreading são a marca registrada em golang e o que torna ela tão rapida em sistemas robustos.
### O que são threading? 
bom as threadings são linhas de processos, cada threading é responsavel por uma processo em si, por exemplo se temos uma threading que faz um especifico trabalho e ela demore 20 minutos para isso, se tiver 10 trabalhos para ela fazer ela demora 200 minutos. porém se adicionarmos mais 10 threadings, nós podemos fazes todos os 10 trabalhos em 20 minutos. elas se utilizam de concorrencia para fazer esse feito.

### O que é concorrencia
Bom a concorrencia é quando as threads concorrem entre si para poder ocupar o kernel, envez de uma trading ocupar totalmente o kernel elas concorrem em simultanidade por um recurs partilhado, assim fazendo tarefas distintas silmultaniamente, para impedir que duas tarefas tentem consumir um mesmo kernel usamos o mutex é como um sinal a qual impede que uma threadin ocupe ou inicie seu processo enquanto outra threadin está consumindo o kernel.

### Diferença entre parelelismo e concorrencia:
Bom o parelelismo ele tem a ideia de realizar tarefas paralelas em um mesmo kernel, vamos supor que temos duas tarefas, onde cada uma é realizada por uma threadin, envez delas concorrerem pelo acesso a threadin elas dividem esse acesso a threadin, por tempo, uma threading passa x minutos e outra também, quando acaba esses x minutos o sistema tira a threading que estava no kernel e coloca a que estava esperando. E possivel fazer isso com um unico kernel no computador. A concorrencia busca competir por esse recurso e os processos não são feitos de forma simultanea. 
