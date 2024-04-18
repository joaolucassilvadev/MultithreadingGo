# MultithreadingGo
nesse repositorio faço a anotação dos meus estudos com multithreading

## Conceitos basicos
Bom ás multitreading são a marca registrada em golang e o que torna ela tão rapida em sistemas robustos.
### O que são threading? 
bom as threadings são linhas de processos, cada threading é responsavel por uma processo em si, por exemplo se temos uma threading que faz um especifico trabalho e ela demore 20 minutos para isso, se tiver 10 trabalhos para ela fazer ela demora 200 minutos. porém se adicionarmos mais 10 threadings, nós podemos fazes todos os 10 trabalhos em 20 minutos. elas se utilizam de concorrencia para fazer esse feito.

### O que é concorrencia: Bom a concorrencia é quando as threads concorrem entre si para poder ocupar o kernel, envez de uma trading ocupar totalmente o kernel elas concorrem em simultanidade por um recurs partilhado, assim fazendo tarefas distintas silmultaniamente, para impedir que duas tarefas tentem consumir um mesmo kernel usamos o mutex é como um sinal a qual impede que uma threadin ocupe ou inicie seu processo enquanto outra threadin está consumindo o kernel.
