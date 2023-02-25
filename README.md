# Improvement no sistema de Avaliação de Imóveis
O desafio consiste em desenvolver um projeto para apoiar o time de corretores e corretoras da imobiliária Inside Place, que precisa melhorar o seu sistema de avaliação de imóveis tornando a precificação mais rápida, precisa e funcional por grande volume de aquisições recebidas.

Outra dor do time é a recomendação de imóveis, uma vez que um cliente ou uma cliente demonstra interesse por um imovel é recomendado apenas imoveis da mesma região pra mesma pessoa, porém essa tecnica não vem apresentando muitas conversões dos cliques

| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **Improvement no Sistema de Avaliação de Imóveis - InsidePlace**
| :label: Tecnologias | Python, PySpark, Colab, jupiter notebook, Apache, BigData
| :rocket: URL         | https://url-deploy.com.br
| :fire: Desafio     | [www.alura.com.br/challenges/data-science-2](https://www.alura.com.br/challenges/data-science-2/)


<!-- Inserir imagem com a #vitrinedev ao final do link -->
![Vitrine](https://github.com/BK-1314/Challenge-Data-Science-Alura/blob/main/Material%20de%20Apoio/Imagens/Vitrine%20Challenge%20Data%20Science%20Alura.png)


## Semana 1 de Projeto
Nesta primeira semana, foi realizada a preparação do ambiente de execução, configurando o ambiente PySpark no Google Colab e importando as bibliotecas necessárias. Em seguida, foi feita a conexão com o Dataframe, extraindo o arquivo zip e lendo o arquivo json.

![dados_brutos](https://github.com/BK-1314/Challenge-Data-Science-Alura/blob/main/Material%20de%20Apoio/Imagens/base_bruta.png)

Após essa etapa, foram realizadas análises e tratamentos nos dados. Foi extraída apenas a coluna "anuncio" que continha mais informações relevantes, como andar, área total, área útil, banheiros, características, endereço, id, quartos, suítes, tipo de anúncio, tipo de unidade, tipo de uso, vagas e valores. A base de dados foi filtrada para conter apenas os valores residenciais, de apartamentos usados.

Em seguida, foram realizadas transformações nas outras colunas que continham valores em formato de lista para valores inteiros e extraídos os demais campos de informações. Por fim, a base de dados tratada foi salva em formato Parquet, que apresentou melhor desempenho, e em formato CSV.

![dados_tratados](https://github.com/BK-1314/Challenge-Data-Science-Alura/blob/main/Material%20de%20Apoio/Imagens/base_tratada.png)

Essas etapas foram realizadas utilizando recursos do PySpark, como pyspark.sql.functions, zipfile e pyspark.sql.types, visando lidar com grandes volumes de dados de forma eficiente. As análises e tratamentos realizados permitirão a construção de um modelo de regressão para precificar imóveis e a criação de um recomendador de imóveis para a InsightPlaces, contribuindo para superar as dificuldades da empresa em alugar e vender imóveis na cidade do Rio de Janeiro.

### [Veja todo Tratamento de dados da semana 1 Aqui](https://github.com/BK-1314/Challenge-Data-Science-Alura/blob/main/Challenge%20Semana%201/Tratamento_Dados_InsightPlaces.ipynb)


###### Esse projeto faz parte do Challenge de Data Science da Altura, e tem como objetivo pôr em prática os conhecimentos as skills relacionadas com um cientista de dados em um contexto real, simulando uma atuação real dentro de uma empresa.
