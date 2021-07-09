# Análise e testes estatísticos
[<img src="https://img.shields.io/badge/author-rlrocha-orange?style=flat-square"/>](https://github.com/rlrocha)
 
 Para comparar estatisticamente resultados de abordagens distintas, é necessário conduzir testes estatísticos para analisar a hipótese de os resultados serem estatisticamente iguais. Para isso, é necessário seguir a sequência de testes considerando 5% o nível de significancia, como mostrado abaixo:

 1. Realizar o teste de Grubb para investigar a hipótese de amostras *outliers* na distribuição dos dados. Se a hipótese de a amostra ser *outlier* não for rejeitada, a amostra é então removida para o teste de normalidade subsequente.
 2. O teste de Shapiro-Wilk é encarregado de conduzir os testes de normalidade, o qual investiga a hipótese que a distribuição dos dados venha de uma distribuição Gaussiana ou normal. Se não for possível rejeitar a hipótese, então é possível realizar testes estatísticos paramétricos para comparar as abordagens, como o teste de análise da variância.
 3. O teste de Levene investiga a hipótese de que diferentes distribuições possuem variâncias iguais.
 4. Por fim, considerando que as distribuições sejam Gaussianas e possuam variâncias iguais, é realizado o teste de Análise da Variância (Analysis of Variance, ANOVA) para investigar a hipótese que a média de diferentes distribuições são iguais.

 Os testes são conduzidos cpm algumas bibliotecas da linguagem de programação Python, e encontram-se disponíves tanto offile quanto online no arquivo [analysis](analysis.ipynb).