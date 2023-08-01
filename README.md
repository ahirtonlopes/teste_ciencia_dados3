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

O Problema do Caixeiro Viajante (Traveling Salesperson - TSP) é um dos mais famosos problemas de otimização combinatória. Este problema é muito fácil de explicar, mas muito complicado de resolver - mesmo para casos com um pequeno número de cidades.

A origem do problema do caixeiro viajante não é muito clara; ele chega a ser mencionado em um manual de 1832 para caixeiros-viajantes, que incluía exemplos de passeios por 45 cidades alemãs, mas não foi formulado originalmente como um problema matemático. No entanto, em 1800, os matemáticos William Rowan Hamilton e Thomas Kirkman criaram formulações matemáticas do problema.

O TSP pode ser definido da seguinte forma: para uma determinada lista de cidades e as distâncias entre cada par delas, queremos encontrar a rota mais curta possível, que vai a cada cidade uma vez e retorna à cidade de origem.

Existe uma classe de Problemas de Pessoa Caixeira Viajante que assume que a distância de ir da cidade $ i $ à cidade $ j $ é a mesma que ir da cidade $ j $ à cidade $ i $, este tipo de TSP também é conhecido como TSP simétrico. Para o seguinte cenário sugerimos usar distâncias euclidianas, mas a formulação do modelo TSP é válida independentemente da forma como as distâncias individuais são determinadas.

A programação matemática é uma abordagem declarativa em que o modelador formula um modelo de otimização matemática que captura os principais aspectos de um problema de decisão complexo. 

Um modelo de otimização matemática tipicamente vai possuir cinco componentes, a saber:

* Conjuntos e índices;
* Parâmetros;
* Variáveis ​​de decisão;
* Função (ões) objetivo (s);
* Quaisquer restrições.

Como entregável, a indústria necessita de uma formulação de TSP que identifique a rota mais curta para as capitais brasileiras, que vai a todas as cidades uma vez e retorna à cidade de origem (os arquivos a serem utilizados, contendo os dados das capitais brasileiras a serem utilizados nesse cenário, você encontra <a href="https://drive.google.com/drive/folders/1pip1P29vKGYWUOSD0hVrdNLNQcGzG3eN?usp=sharing">aqui</a>)

states_coords.csv: contém a latitude e longitude de cada capital de estado brasileiro;
states_line.json: contém o nome dos estados e a distância em km de todos os pares possíveis assumindo uma linha conectando as cidades;
states_gmaps.json: contém o nome dos estados e a distância em km de todos os pares possíveis com as informações do Google a respeito.

## Entregáveis

Já o quarto entregável pode estar contido como comentários em suas soluções prévias, queremos entender melhor como foi seu processo de solução de problemas, quais as hipóteses levantadas e, se tivesse mais tempo, como você poderia melhorar a implementação proposta.

Ou seja, temos quatro entregáveis:

- Relatório com exemplos de anomalias encontradas e possibilidades dentro da sua experiência e com relação aos dados da base;
- Resolução de problema de transformação de dados (NF-e);
- TSP (Traveling Salesperson Problem) resolvido para as capitais brasileiras;
- Comentários a respeito da implementações propostas e melhorias (desenvolvimento incremental).

## Dados

| Table            | Total Rows | Total Columns                                              |
| -----------------|:--------:  | :---------------------------------------------------------:|
| Orders           | 9994       | 21                                                         |
| People           | 4          | 2                                                          |
| Returns          | 296        | 2                                                          |

## O que será avaliado?

1. Buscamos soluções bem definidas e baseadas em método: soube mostrar quais as hipóteses levantadas? Precisou ao menos de modo resumido o por que escolheu determinado caminho? Quais os prós e contras usados para se basear essa solução e quais os passos para implementá-la?
2. Qualidades dos entregáveis, tanto o report de anomalias encontradas quanto o TSP resolvido.  
3. A eficiência do método utilizado para a verificação de anomalias.
4. Se tivesse mais tempo, o que você faria para melhorar a sua solução?

Obrigado pela sua participação.

## 

“Perception is strong and sight weak. In strategy it is important to see distant things as if they were close and to take a distanced view of close things.”

Miyamoto Musashi. Japanese martial artist, philosopher, strategist, writer, artist (1584-1645).
