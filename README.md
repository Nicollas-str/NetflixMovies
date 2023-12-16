# Netflix

## Dashboard feito como um projeto da EBAC(Escola Britânica de artes criativas &amp; tecnologia) utilizando dados retirados do Kaggle sobre filmes e séries da Netflix.

### Resumo

Um projeto requisitado pela EBAC(Escola britânica de artes criativas &amp; tecnologia) de um dashboard com o tema aberto, a proposta é pegar um dataset do Kaggle, limpa-lo e com isso criar um dashboard usando o Google Looker Studio.

Sabendo disso, utilizei um dataset sobre filmes e series da netflix que tem como base rankear os filmes e series em um top 10 semanalmente e isso foi feito por 3 anos se iniciando em 2021.

Neste projeto foi utilizado Python para a limpeza e criação do arquivo e Google Looker Studio para a criação do dashboard.

### Informações sobre os dados

INFORMAÇÃO IMPORTANTE: OS DADOS CONTÉM ALGUMAS LETRAS OU ATÉ MESMO TÍTULOS INTEIROS COM (?) OS DADOS ESTAVAM DISPONÍVEIS ASSIM NO KAGGLE E NÃO HOUVE COMO FAZER UM TRATAMENTO DISSO.

PAÍS = País em que se baseiam os dados da linha

SIGLA_PAÍS = Sigla do país

SEMANA = Semana em que se baseiam os dados da linha

CATEGORIA = Filme ou série

RANK_SEMANAL = Rank em que o filme ficou na semana (de 1 a 10)

TÍTULO = Título do filme

TÍTULO_EPISÓDIO = Título do episódio

CONSECUTIVOS_TOP10 = Dias consecutivos em que um filme ficou em top 10

### Criação do projeto

**Sistema de pontos para aproveitar melhor os dados:**
**Já que os filmes e as vezes suas posições no rank se repetiam, construí um sistema de pontos em que na posição 1 no rank o filme recebe 10 pontos, na posição 2 ele recebe 9 e assim até 10, após isso fiz a soma dos pontos de cada filme e consegui tirar uma relevância melhor dos dados que eu tinha em mãos.**

Fiz uma análise dos dados usando o Pandas e Excel para ver o que eu tinha pra trabalhar, cheguei a conclusão de que eram pouquíssimos dados que eu tinha, então eu coloquei como objetivo aprender melhor como trabalhar com poucos dados já que é muitos mais fácil trabalhar com muitos, onde você consegue ter uma grande variedade de análises sem muita preocupação, e esse meu dataset não tinha nem quantidade de horas assistidas ou quantidade de pessoas que assistiram.

Então como primeiro item quis fazer uma visualização breve do rank mínimo e máximo em que um filme ou série alcançou e a variância do mesmo, olhando o gráfico sem nenhum filtro isso não parece de grande utilidade por que obviamente ele sempre vai estar como 1 em mínimo e 10 em máximo, mas quando é feita a relação com um filme especifico ou uma data especifica é possível tirar informações uteis disso.

Após isso eu construí dois gráficos, um de barras e um geográfico, no de barras eu utilizei o sistema de pontos e fiz um rank dos filmes, e no geográfico foi feito o rank dos filmes em cada pais, assim mostrando o filme no top rank apenas passando o cursor no pais desejado, além disso o vinculo do gráfico com o rank e o geográfico é feito automaticamente ja que se for feita a seleção de um filme ja exibe no geográfico os países que mais assistiram o mesmo, e se clica em um país é mostrado o rank dos filmes mais assistidos no gráfico de barras. 
