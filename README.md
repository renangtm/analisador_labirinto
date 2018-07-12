Projeto Acadêmico de desenvolvimento e implementação de algorítimo de leitura de labirintos em formato de imagem, calculo e exibição de melhor solução. 

A imagem pode conter variações de cores, ter letras, numeros, e afins, só precisa existir um labirinto nítido.

O Algorítimo recebe 3 parâmetros atualmente, raio do objeto que vai percorrer o labirinto, nível de variação de cor e precisão.

Consiste em segmentar a imagem em quadriculado(tamanho do quadro determinado pela precisão).

Eliminar pontos onde a variação de cor excede o limite(limite é uma das variaveis).

Criar conexões entre os pontos. Gerando um grafo onde todas as ligações tem a mesma distância.

Implementar o algorítimo reduzido de Dijkstra para grafos com conexões de distancia igual.

Converter o caminho em retas.

percorrer todas as retas de 2 em 2, tentando transformar cada 2 retas em 1, linkando o ponto inicial da primeira com o ponto final da segunda. O Link só ocorre caso a variação de cor entre os pontos considerando a expessura do objeto, não seja maior que o limite. Isso ocorre até não ter mais otimizações possíveis.

Otimizar as retas resultantes, pelo mesmo principio do algorítimo de bezier, onde se pega o ponto médio de 2 retas e gera uma suavização. Porém nesse caso ele faz primeiro com o ponto médio(1/2 da reta), depois com o ponto 1/3  que esta mais ao topo e depois com o 1/4, e asism por diante limitado por uma variavel de geração de curvatura.


Segue uma implementação do algorítimo com Java Script puro em um único arquivo para facilitar a leitura do mesmo, bastando somente abrir no navegador escolher o arquivo de imagem, e clicar em carregar imagem, depois disso selecionar o ponto inicial e final na imagem. 

as 3 variaveis podem ser modificadas pelas caixas de texto para ver melhor o funcionamento do algorítimo.

"Carregar parcialmente" pode ser usado para selecionar novos pontos, porém ao alterar uma das 3 variaveis principais é preciso carregar a imagem novamente.






