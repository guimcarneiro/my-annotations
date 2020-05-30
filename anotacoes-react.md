# Pensamentos sobre React

### Introdução à Minha Mente *React*

Como meu primeiro contato com o desenvolvimento *front-end* de fato aconteceu com o *React*, meu modo de raciocinar sobre soluções passou a girar em torno da arquitetura da tecnologia, e sinto que isso me prende um pouco - o que se tornará um problema caso passe a atuar em projetos *front-end* de outra natureza. Apesar disso, sinto que posso discutir sobre o *React Environment* tranquilamente, visto que já venho trabalhando com ele há meses, e já possuo alguma experiência na construção de soluções utilizando-o, e elas têm sido bem-sucedidas.

## Primeiras Dúvidas

### Como acontece a comunicação entre a estrutura HTML e o código?
Esse é um problema que supera o React, e na verdade se refere a como um site funciona. Na minha concepção, construída das experiências que vivi até agora, penso que todo o funcionamento se baseia no lançamento de eventos pelos elementos HTML, e pela árvore de elementos HTML em si, e como ela está amarrada.

Penso que a árvore de nós de um arquivo HTML funciona de maneira parecida com a componentização recorrente no *React*, visto que cada elemento é composto por *n* outros elementos, e assim por diante, existindo sempre a possibilidade de lançar eventos originados de elementos bem inferiores na árvore, podendo ser capturados por elementos superiores, para que seja feito o devido tratamento e reação, uma vez que a natureza do mesmo é identificada e a reação acontece.

Acho que essas reflexões são o suficiente por hoje, pois estou mais interessado em detalhes mais complexos, que ficarão mais para o final desse arquivo.

## Pensamentos Mais Complexos