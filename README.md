# Teste - Ciência de Dados / Visão Computacional (Short Track)

Teste técnico para nossas posições em Ciência de Dados (short track)

O seguinte teste tem por premissa ser um problema base (Ref. <a href="https://teaching.cornell.edu/teaching-resources/engaging-students/problem-based-learningproblem">problem based learning</a>) de modo que você pode usá-lo como achar adequado tendo em vista a demonstração de seus conhecimentos técnicos.

Queremos entender melhor seu jeito de atacar problemas desafiadores em amostras de mundo real, além de que, do modo que está estruturada, a entrega, apesar de rápida, nos permite verificar mais detalhes de seu perfil profissional tais como organização, pontualidade e percepção quanto a suas skills de data wrangling, validação e governança e programação Python. Recomendamos ainda que o teste seja feito em no máximo 6 horas (não se preocupe em respostas muito detalhadas ou em complexidades que simplesmente não funcionariam no mundo real!).

As entregas devem ser via envio de link para um github público (ou similar) o qual contenha sua solução para o cenário a seguir. Favor não citar a Lambda3 em seu repositório.

## Cenário I

No seguinte cenário você é a pessoa cientista de dados por trás de um projeto de analytics junto a uma grande indústria norte-americana.

Os dados a serem ingeridos e analisados em nossa plataforma de Big Data são dados de compras (orders), pessoas (people) e devoluções (returns).

Sua primeira tarefa, a partir desse cenário, deve ser um relatório (de preferência um <a href="https://jupyter.org/">jupyter notebook</a> ou <a href="https://colab.research.google.com/">colab notebook</a> relatando algumas das anomalias encontradas e investigações possíveis (falamos que aqui encorajamos gente curiosa, certo?!)

O dataset a ser utilizado nesse cenário (.zip com arquivo CSV) você encontra <a href="https://drive.google.com/file/d/1a8UCbzXFbqTQi0x8tqCXPRTlB--E7o8I/view?usp=sharing">aqui</a>.

Temos um apreço muito grande por qualidade e disponibilidade. Sendo assim, é bom contarmos com métricas para nos previnir e alertar sobre quaisquer problemas bem como metrificar e monitorar as arquiteturas proposta. Logo, apreciamos se você conseguir entregar testes que mensurem a qualidade dos dados junto à sua solução desse primeiro entregável.

## Cenário II

O segundo entregável consiste na transformação de dados disponíveis em <a href="https://drive.google.com/file/d/1IDCjpDZh5St97jw4K_bAewJ8hf-rax9C/view?usp=sharing">arquivo Json</a> para o formato de dataframe, algo comum no dia a dia da empresa. Após transformar esse Json em dataframe é possível perceber que a coluna "item_list" está como dicionário. Seu gestor pediu dois pontos de atenção nessa tarefa:

- Expandir a coluna num mesmo dataframe;
- Normalizar os itens dessa coluna de dicionário e dividí-los em dois dataframes separados, seguindo o modelo relacional.

## Cenário III

Classificação de imagens para determinar se é dia ou noite:

Nesta tarefa, você candidato precisa desenvolver um modelo de aprendizado de máquina capaz de analisar imagens e classificá-las como "dia" ou "noite". Para isso, podem se utilizar de LLMs, como modelos de classificação de imagens pré-treinados, ou mesmo treinar seu próprio modelo a partir de dados rotulados. Aqui verificaremos  o pré-processamento dos dados, extração de características relevantes e treinamento de um classificador eficaz. É importante que o conjunto de dados de treinamento seja representativo e variado para garantir que o modelo seja robusto o suficiente para lidar com várias condições de iluminação.

<a href="https://drive.google.com/file/d/1ifdwWBWpVYHnU7S4TEBr8nRqtCrR_o2k/view?usp=sharing">Aqui</a> você encontra um notebook exemplo com parte de uma implementação tradicional a partir de dados rotulados do dataset AMOS que pode ser utilizado como ponto de partida para sua solução

## Cenário IV

Como último entregável favor fornecer uma arquitetura de como poderia ser implementada um sistema de detecção de cena completo, baseado no código criado no cenário anterior. Fique a vontade para se utilizar do ecossistema de computação em nuvem o qual se sente mais confiante em trabalhar, procurando usar os serviços nativos sempre que possível. Pense em questões como disponibilidade, catálogo de dados e segurança se achar cabível. Recomendamos o uso do draw.io (https://app.diagrams.net/) ou do excalidraw (https://excalidraw.com/)

## Entregáveis

Temos então quatro entregáveis:

- Relatório com exemplos de anomalias encontradas e possibilidades dentro da sua experiência e com relação aos dados da base;
- Resolução de problema de transformação de dados (NF-e);
- Classificador/LLM de imagens para determinar se é dia ou noite:
- Arquitetura AWS, Azure, GCP ou outras.

Não se esqueça de fornecer comentários a respeito da implementações propostas e melhorias (desenvolvimento incremental). Queremos entender melhor como foi seu processo de solução de problemas, quais as hipóteses levantadas e, se tivesse mais tempo, como você poderia melhorar a implementação proposta.

## Dados

| Table            | Total Rows | Total Columns                                              |
| -----------------|:--------:  | :---------------------------------------------------------:|
| Orders           | 9994       | 21                                                         |
| People           | 4          | 2                                                          |
| Returns          | 296        | 2                                                          |

## O que será avaliado?

1. Buscamos soluções bem definidas e baseadas em método: soube mostrar quais as hipóteses levantadas? Precisou ao menos de modo resumido o por que escolheu determinado caminho? Quais os prós e contras usados para se basear essa solução e quais os passos para implementá-la?
2. Qualidades dos entregáveis, tanto o report de anomalias encontradas quanto o problema em Visão Computacional e a arquitetura desenvolvidos.
3. A eficiência do método utilizado para a verificação de anomalias.
4. Se tivesse mais tempo, o que você faria para melhorar a sua solução?

Obrigado pela sua participação e boa sorte!

## 

“Perception is strong and sight weak. In strategy it is important to see distant things as if they were close and to take a distanced view of close things.”

Miyamoto Musashi. Japanese martial artist, philosopher, strategist, writer, artist (1584-1645).
