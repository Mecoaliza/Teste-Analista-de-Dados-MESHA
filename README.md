# Teste Analista de Dados
Critérios avaliadas:
- Uso de Funções DAX
- Documentação das medidas
- ETL
- Modelagem dimensional dos dados

### Levantar Indicadores
#### Responder às seguintes perguntas:
1. Qual a escola com a maior média de notas?
2. Qual o aluno com a maior média de notas e o valor dessa média?
3. Qual a média geral?
4. Qual o % de Ausentes?
5. Qual o número total de Inscritos?
6. Qual a média por disciplina?
7. Qual a média por Sexo?
8. Qual a média por Etnia?

______________

O link para baixar o arquivo está [disponível aqui](https://drive.google.com/drive/folders/1Ppd7osQTAqLDhEbYrsYKbd63GKD7Wrss?usp=share_link)

### Soluções Utilizadas

- Pentaho
- SQL Serve
- Power BI

### Fluxo de ETL

<img src="imagens\fluxo de trabalho.png">

#### Transformação Pentaho

![transformação pentaho](imagens\transformacao pentaho.jpeg)

- Carrega csv com microdados
- ajusta valores 
- preenche valores nulos por tipo
- carrega tabela no banco de dados 


#### Modelagem Dimensional

![modelagem de dados](imagens\modelagem de dados.png)

A modelagem foi adotada para analisar alguns dados sociecônomicos e tipos de falta

### Observações sobre a Solução Adotada

1. A modelagem foi realizada no power query utilizando a tabela carregada no sql server como base para criar as dimensões

2. Para analisar os dados de ausência por disciplina necessitou-se mesclar as colunas TP_PRESENCA de cada disciplina, a fim de criar duas novas colunas, uma com a descrição do tipo presenca e outra com o valor da presenca