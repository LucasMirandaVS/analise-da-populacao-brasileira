# Analisando os municipios brasileiros 
Usando os pacotes pandas, numpy, seaborn, requests e BeautifulSoup, Fiz web scrapping para colher dados populacionais sobre todos os municípios do Brasil e fiz uma análise exploratória das variáveis.

O site utilizado como fonte de dados foi o Wikipedia. Essa escolha se dá por conta das listas completas e atualizadas com todos os municipios do país. Os dados utilizados são referentes ao número de habitantes e Produto Interno Bruto de cada município do Brasil. Para realizar a coleta, utilizei o pacote BeautifulSoup e usei a tag html da página do wikipedia.

![taghtml](https://user-images.githubusercontent.com/77032413/181127991-34f10aad-cc78-4307-bd91-48208431c8a8.png)

Após a extração, coloquei os dados em um dataframe. O Processo foi repetido para os dados de renda (PIB) dos municipios. O dataframe final ficou assim:

![df2](https://user-images.githubusercontent.com/77032413/181128455-e01fb8b6-1234-47c3-a4bb-eaaa8b49cc2e.png)

## Analisando os dados

A primeira coisa depois de manipular e limpar os dados foi partir pra visualização. Primeiro dos maiores municípios em termos de renda, depois em termos de população:

![pibp](https://user-images.githubusercontent.com/77032413/181128761-32023207-32ec-459f-b5b3-31d2e3b11821.png)

![pibpo](https://user-images.githubusercontent.com/77032413/181128875-35ace7b7-80a6-4394-9308-dccc9e52ef59.png)

 Não coincidentemente, os municipios com maior renda também são os mais populosos. O mesmo pôde ser constatado com os menores valores. Sendo assim, achei válido analisar a correlação destes fatores, mesmo com o baixo número de variáveis. O método escolhido para visualizar a relação entre população e renda foi um heatmap de correlação.
 
 ![het](https://user-images.githubusercontent.com/77032413/181129117-45eb873c-83b1-49d9-a93e-333b988c1e0a.png)

Como esperado, a correlação entre as variáveis foi positiva e forte.
 
 # Conclusão
 O objetivo deste projeto foi coletar e limpar dados para análise através do pandas e BeautifulSoup. Ainda que limitada pelo número de variáveis, os resultados estiveram dentro do esperado. A análise completa com os comandos utilizados estão no arquivo jupyter Notebook!
