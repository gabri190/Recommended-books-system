# Sistema de Recomendação de Livros

## Introdução
Sistemas de recomendação são ferramentas que ajudam as pessoas a encontrar itens que possam ser do seu interesse, com base em suas preferências e histórico de comportamento. Esses sistemas são usados em diversos contextos, desde lojas online até serviços de streaming de música e vídeo. Um exemplo comum é o sistema de recomendação de livros, que sugere títulos com base em livros que uma pessoa já leu e gostou. Por exemplo, se uma pessoa leu e gostou de "O Hobbit", o sistema pode recomendar outros livros de fantasia, como "As Crônicas de Nárnia" ou "O Senhor dos Anéis". Esse tipo de sistema é muito útil para ajudar as pessoas a descobrir novos livros que possam ser interessantes para elas, especialmente quando há muitas opções disponíveis.

## Definição Técnica
Do ponto de vista do aprendizado de máquina, sistemas de recomendação são geralmente construídos utilizando algoritmos de aprendizado supervisionado ou não supervisionado. O objetivo é criar um modelo que possa aprender a partir dos dados históricos dos usuários e gerar previsões sobre os itens que possam ser do interesse deles.

No caso de livros, por exemplo, o modelo pode ser treinado com base em dados de histórico de leitura e avaliações de usuários. A partir desses dados, o modelo pode identificar padrões e relações entre livros e criar um perfil de preferência para cada usuário. Com base nesses perfis, o modelo pode recomendar novos livros que possam agradar a cada usuário individualmente.

Existem diversos algoritmos de aprendizado de máquina que podem ser usados para construir sistemas de recomendação, como a filtragem colaborativa, a decomposição de valores singulares (SVD) e as redes neurais. Cada algoritmo tem suas vantagens e desvantagens, e a escolha do melhor algoritmo para um determinado problema depende das características do conjunto de dados e dos requisitos do sistema de recomendação.

Para o caso da nossa aplicação, iremos utilizar o KNN de maneira não supervisionada,ou seja, treinar features e conseguir determinar clusters para definir gostos semelhantes ao do usuário.

## Objetivo

O objetivo principal de um sistema de recomendação de livros é ajudar os usuários a descobrir novos livros que possam ser do seu interesse, com base em suas preferências e histórico de comportamento. Essa ferramenta é muito útil para ajudar as pessoas a superar o problema da sobrecarga de informação, que acontece quando há muitas opções disponíveis e é difícil escolher qual livro ler em seguida.

Além disso, o sistema de recomendação de livros pode ajudar a melhorar a experiência do usuário em uma loja online de livros, por exemplo, aumentando as chances de uma compra ser realizada. Quando os usuários se sentem bem atendidos por um sistema de recomendação que apresenta livros de acordo com suas preferências, eles podem se sentir mais inclinados a explorar a loja e a fazer compras adicionais.

Outro objetivo importante do sistema de recomendação de livros é ajudar a loja a melhorar suas estratégias de marketing, identificando tendências de compra e de interesse do público. Com as informações geradas pelo sistema de recomendação, a loja pode entender melhor as preferências e necessidades dos seus clientes e ajustar seu estoque e estratégias de marketing para atendê-las.

## Aplicações
Existem diversas aplicações práticas do sistema de recomendação de livros, principalmente em lojas online de livros e bibliotecas digitais. Algumas das principais aplicações são:
<div>
    <li> Recomendação personalizada de livros: o sistema de recomendação pode sugerir livros com base no histórico de leitura do usuário, suas avaliações e suas preferências. Dessa forma, o usuário pode descobrir novos livros que se encaixem em seu perfil de leitura.

<li> Listas de livros recomendados: a loja online de livros pode criar listas de livros recomendados com base em temas específicos ou em tendências de mercado. Essas listas podem ser uma fonte de inspiração para os usuários que desejam explorar novos títulos.

<li> Sistemas de classificação e avaliação: o sistema de recomendação pode ajudar os usuários a avaliar livros e a compartilhar suas opiniões com outros leitores. Dessa forma, é possível criar um ambiente de discussão e interação em torno dos livros, o que pode incentivar ainda mais as compras.

<li> Análise de dados e tendências: a loja online de livros pode usar os dados gerados pelo sistema de recomendação para entender melhor as tendências de mercado e as preferências dos usuários. Com essa informação, a loja pode ajustar seu estoque e sua estratégia de marketing para atender melhor as necessidades dos seus clientes.

</div>

## Máquina preditiva

Com base nas escolhas de outras pessoas que leram o mesmo livro, o sistema de recomendação pode prever se um usuário vai gostar ou não de um determinado livro. Para isso, o sistema de recomendação pode usar um modelo de aprendizado de máquina que aprenda a partir dos dados históricos dos usuários e gere previsões sobre os livros que possam ser do interesse deles.

## Reflexões

- Se você receber uma recomendação certeira, a chance de você comprar o livro é muito maior. Por isso, é importante que o sistema de recomendação seja preciso e confiável.
- Se mais pessoas comprarem, maior será o fafturamento da empresa?
-  O sistema de recomendação pode ajudar a melhorar a experiência do usuário em uma loja online de livros, por exemplo, aumentando as chances de uma compra ser realizada. - - Quando os usuários se sentem bem atendidos por um sistema de recomendação que apresenta livros de acordo com suas preferências, eles podem se sentir mais inclinados a explorar a loja e a fazer compras adicionais.

## Dataset utilizado

O dataset Book Recommender System foi criado por Ahmadullah Siddiqui e está disponível no Kaggle. O dataset contém dados de 271370 livros e 1149779 avaliações de usuários e mais de 240000 usuários. Os dados foram coletados do Goodreads e do Amazon e estão disponíveis no Kaggle.

## Predições Realizadas:
- Algoritmo KNN

![image](https://github.com/gabri190/Recommended-books-system/assets/72319195/ad8b07c1-c90f-482f-b2fb-c325c9c39df9)

- Algoritmo KDTree

![image](https://github.com/gabri190/Recommended-books-system/assets/72319195/7c5b9361-a5e4-4b5a-ad8f-89f05c9d073c)

Essas imagens determinam também a distância média para os vizinhos mais próximos indicando o quão semelhante é o livro recomendado em relação ao livro avaliado pelo usuário.

## Análise de Resultados
- silhouette_score
	
![image](https://github.com/gabri190/Recommended-books-system/assets/72319195/dde10693-f5a6-4841-a43d-56e94288b41d)

- calinski_harabasz_score

![image](https://github.com/gabri190/Recommended-books-system/assets/72319195/c1eddc88-8cc1-47e3-97d6-bbf4d0f387ab)

## Conclusão
Em conclusão, o projeto de sistemas de recomendação utilizando machine learning é extremamente útil em diversos setores, desde o comércio eletrônico até a indústria do entretenimento. Utilizando algoritmos avançados de aprendizado de máquina, é possível oferecer aos usuários recomendações personalizadas e relevantes, aumentando a satisfação do usuário e a fidelidade à plataforma.

Ao longo deste projeto, pudemos explorar diferentes técnicas de machine learning, desde algoritmos simples de filtragem colaborativa até modelos de deep learning mais complexos, como redes neurais. Além disso, foram discutidos os desafios enfrentados na construção de sistemas de recomendação, como o problema do "cold start" e a necessidade de dados de alta qualidade.

No final, foi possível construir um sistema de recomendação eficiente e preciso, capaz de sugerir itens relevantes aos usuários com base em suas preferências e histórico de interações. Com a crescente demanda por soluções de recomendação personalizadas, acreditamos que esse projeto tem grande potencial para ajudar empresas a melhorar a experiência do usuário e aumentar o engajamento em suas plataformas.

## Proposta de Melhoria
<div>
<li> Avaliar o desempenho do modelo em conjuntos de dados maiores e mais diversificados.
<li> Investigar abordagens de aprendizado federado que permitam treinar o modelo em dados distribuídos em vários locais sem a necessidade de compartilhar dados.
<li> Explorar a utilização de técnicas de aprendizado não supervisionado para descobrir padrões ocultos nos dados e melhorar a qualidade das recomendações.
<li> Incorporar feedback explícito e implícito dos usuários para melhorar a precisão e a relevância das recomendações.
</div>

## Próximos passos

Embora o modelo de sistemas de recomendação desenvolvido neste projeto tenha apresentado resultados promissores, sempre há espaço para melhorias e aprimoramentos. Aqui estão algumas sugestões de melhorias que poderiam ser exploradas:
<div>
<li> Incorporar técnicas de processamento de linguagem natural (NLP) para melhorar a compreensão das preferências dos usuários com base em suas avaliações e comentários.
<li> Explorar abordagens de aprendizado por reforço para otimizar o desempenho do sistema de recomendação ao longo do tempo.
<li> Introduzir técnicas de transferência de aprendizado para aproveitar modelos pré-treinados em grandes conjuntos de dados e melhorar a eficiência do modelo.
<li> Utilizar técnicas de interpretabilidade de modelos para entender melhor como o sistema de recomendação toma decisões e fornecer explicações aos usuários.


</div>























