# Base de estudo: questões com gabarito e explicação

627 questões, agrupadas por área e por avaliação. Cada uma traz enunciado, alternativas, resposta certa, explicação, fonte e situação da explicação.


# Área 1: Aprendizado não supervisionado (clustering, análise fatorial, correspondência)

## Unsupervised Machine Learning: Análise Fatorial e PCA I

### Questão 161258-1-1
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Assinale a alternativa que indica um critério para a escolha do número de fatores a serem extraídos em uma análise fatorial por componentes principais.

- a) Considerar apenas fatores correspondentes a cargas fatoriais maiores que 50%.
- b) Considerar apenas fatores correspondentes a correlações maiores que 1.
- c) Considerar apenas fatores correspondentes a autovalores maiores que 1.
- d) Considerar apenas fatores correspondentes a scores fatoriais positivos.

**Resposta certa:** c) Considerar apenas fatores correspondentes a autovalores maiores que 1.

**Explicação:** A resposta é considerar apenas fatores com autovalores maiores que 1, o critério de Kaiser (raiz latente). Um autovalor acima de 1 significa que o fator explica mais variância do que uma variável original sozinha. Carga fatorial de 50% e scores positivos não são critérios de escolha do número de fatores.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 17

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-10
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Sobre os tipos de variáveis adequadas para realizar uma análise fatorial por componentes principais, é correto afirmar que:

- a) Somente variáveis padronizadas pelo Z-Score são aptas.
- b) Somente variáveis quantitativas são aptas.
- c) Somente variáveis categóricas são aptas.
- d) Somente variáveis qualitativas são aptas.

**Resposta certa:** b) Somente variáveis quantitativas são aptas.

**Explicação:** A resposta é que somente variáveis quantitativas (métricas) são aptas, porque a PCA depende das correlações de Pearson. Variáveis qualitativas ou categóricas não entram. A padronização pelo Z-Score é feita dentro do método e não é condição para a variável ser apta.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 3

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-2
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Dentre os testes estatísticos listados a seguir, qual deles é utilizado para avaliar a adequação global da análise fatorial nos dados?

- a) Teste F para comparação de variâncias.
- b) Teste de esfericidade de Bartlett.
- c) Teste t de diferenças de médias.
- d) Teste qui-quadrado para associação.

**Resposta certa:** b) Teste de esfericidade de Bartlett.

**Explicação:** A resposta é o teste de esfericidade de Bartlett. Ele compara a matriz de correlações com a matriz identidade e, se forem estatisticamente diferentes, a análise fatorial é adequada. Os testes F, t e qui-quadrado de associação respondem a outras perguntas.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-3
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Em relação à interpretação do p-valor do teste de esfericidade de Bartlett, assinale a alternativa correta:

- a) Se o p-valor for maior que 0.05, podemos concluir que a matriz de correlações de Pearson é estatisticamente diferente da matriz identidade, portanto, podem ser extraídos fatores a partir das variáveis originais.
- b) Se o p-valor for menor que 0.05, podemos concluir que a matriz de correlações de Pearson é estatisticamente diferente da matriz identidade, portanto, podem ser extraídos fatores a partir das variáveis originais.
- c) Se o p-valor for maior que 0.05, podemos concluir que os autovalores são estatisticamente maiores que 1, portanto, podem ser extraídos fatores a partir das variáveis originais.
- d) Se o p-valor for maior que 0.05, podemos concluir que os scores fatoriais são estatisticamente maiores que 0, portanto, podem ser extraídos fatores a partir das variáveis originais.

**Resposta certa:** b) Se o p-valor for menor que 0.05, podemos concluir que a matriz de correlações de Pearson é estatisticamente diferente da matriz identidade, portanto, podem ser extraídos fatores a partir das variáveis originais.

**Explicação:** A resposta é p-valor menor que 0,05. Nesse caso rejeita-se H0 (matriz de correlações igual à identidade), ou seja, as correlações de Pearson são diferentes de zero e dá para extrair fatores. Com p maior que 0,05 não se rejeita H0, e a análise não é adequada.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-4
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Os scores fatoriais da análise fatorial por componentes principais são:

- a) O percentual da variância compartilhada pelas variáveis originais para a formação de cada fator.
- b) Os parâmetros que relacionam o fator com as variáveis originais, representados em um modelo linear.
- c) O critério de decisão para a quantidade de fatores a serem extraídos da análise.
- d) O coeficiente de correlação entre o fator e as variáveis originais do banco de dados.

**Resposta certa:** b) Os parâmetros que relacionam o fator com as variáveis originais, representados em um modelo linear.

**Explicação:** A resposta é que os scores fatoriais são os parâmetros que relacionam o fator com as variáveis originais num modelo linear. Eles são obtidos de autovalores e autovetores da matriz de correlações. O percentual de variância é o autovalor, e a correlação entre fator e variável é a carga fatorial.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 14

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-5
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Em uma análise fatorial, foram identificados os seguintes autovalores: “2.05”, “1.10”, “0.55” e “0.30”. Utilizando o critério da raiz latente (critério de Kaiser), quantos fatores serão extraídos na PCA?

- a) 3.
- b) 4.
- c) 2.
- d) 1.

**Resposta certa:** c) 2.

**Explicação:** A resposta é 2. Pelo critério de Kaiser ficam só os fatores com autovalor maior que 1. Aqui, 2,05 e 1,10 passam, enquanto 0,55 e 0,30 ficam de fora.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 17

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-6
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Sobre os coeficientes de correlação de Pearson entre as variáveis de uma análise fatorial por componentes principais, pode-se afirmar que:

- a) Coeficientes de correlação próximos de zero propiciam a extração de um único fator, pois indicam que a relação entre as variáveis é estatisticamente significativa.
- b) Coeficientes de correlação mais próximos dos valores extremos (-1; +1) propiciam a extração de muitos fatores, pois indicam baixa correlação entre as variáveis.
- c) Coeficientes de correlação mais próximos dos valores extremos (-1; +1) propiciam a extração de um único fator.
- d) Coeficientes de correlação próximos de zero propiciam a extração de um único fator, pois indicam que a relação entre as variáveis é elevada.

**Resposta certa:** c) Coeficientes de correlação mais próximos dos valores extremos (-1; +1) propiciam a extração de um único fator.

**Explicação:** A resposta é que correlações próximas de -1 ou +1 propiciam a extração de um único fator. Isso indica que as variáveis estão relacionadas e podem ser resumidas em um fator. Já correlações próximas de zero indicam variáveis sem relação, o que levaria a fatores diferentes.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-7
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

No método da análise fatorial por componentes principais ocorre:

- a) A criação de fatores com elevada correlação entre si a partir da combinação das variáveis originais.
- b) A criação de fatores não correlacionados entre si a partir da combinação linear das variáveis originais.
- c) A criação de fatores com correlação perfeitamente negativa (-1) entre si a partir da combinação das principais variáveis da análise.
- d) A criação de fatores com correlação perfeitamente positiva (+1) entre si a partir da combinação das principais variáveis da análise.

**Resposta certa:** b) A criação de fatores não correlacionados entre si a partir da combinação linear das variáveis originais.

**Explicação:** A resposta é a criação de fatores não correlacionados entre si, a partir de combinações lineares das variáveis originais. Por isso os fatores da PCA são ortogonais, com correlação zero. Fatores muito correlacionados, ou com correlação -1 ou +1, contrariam a lógica do método.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-8
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

Dentre os elementos listados a seguir, assinale a alternativa que apresenta um elemento fundamental na análise fatorial por componentes principais:

- a) Matriz de distâncias Euclidianas.
- b) Dendrograma.
- c) Teste qui-quadrado para associação de variáveis categóricas.
- d) Matriz de correlações de Pearson.

**Resposta certa:** d) Matriz de correlações de Pearson.

**Explicação:** A resposta é a matriz de correlações de Pearson. A PCA parte das correlações entre as variáveis originais, e dela saem os autovalores e autovetores que formam os fatores. Matriz de distâncias e dendrograma pertencem à análise de agrupamentos.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 161258-1-9
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA I

No contexto da criação de rankings na análise fatorial, em relação à variável gerada como resultado do método da soma ponderada e ordenamento, assinale a alternativa correta:

- a) É uma variável métrica, pois é formada com base nos valores calculados por meio dos fatores.
- b) É uma variável qualitativa, pois separa as observações em grupos distintos.
- c) É uma variável métrica, pois é formada com base nos agrupamentos das observações.
- d) É uma variável qualitativa, pois separa as variáveis em grupos distintos.

**Resposta certa:** a) É uma variável métrica, pois é formada com base nos valores calculados por meio dos fatores.

**Explicação:** A resposta é variável métrica, formada com base nos valores dos fatores. O ranking é uma soma de fatores ponderados pela variância compartilhada, então cada observação recebe um número contínuo. O ordenamento só posiciona esses valores, mas a variável em si continua quantitativa.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 20

**Situação:** explicação conferida com o material das aulas

---

## Unsupervised Machine Learning: Análise Fatorial e PCA II

### Questão 162549-1-1
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

O p-valor = 0.000 obtido no teste de esfericidade de Bartlett para a Análise Fatorial por Componentes Principais indica que:

- a) A Análise Fatorial por Componentes Principais é adequada e pode ser implementada.
- b) Os coeficientes de correlação de Pearson entre as variáveis são todos iguais a zero.
- c) Não há adequação dos dados para a implementação da Análise Fatorial PCA.
- d) Não serão obtidos fatores adequados após a implementação da análise fatorial.

**Resposta certa:** a) A Análise Fatorial por Componentes Principais é adequada e pode ser implementada.

**Explicação:** A resposta é que a análise fatorial é adequada e pode ser implementada. Com p-valor 0,000 rejeita-se H0 do teste de Bartlett, então a matriz de correlações é diferente da identidade. Isso não quer dizer que as correlações sejam todas zero, que é o contrário.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-10
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Em relação aos fatores extraídos na análise fatorial, assinale a alternativa correta:

- a) Os valores calculados para as observações da amostra com base nos fatores formam variáveis qualitativas.
- b) Os valores calculados para as observações da amostra com base nos fatores formam variáveis categóricas.
- c) Os valores calculados para as observações da amostra com base nos fatores formam variáveis binárias.
- d) Os valores calculados para as observações da amostra com base nos fatores formam variáveis quantitativas.

**Resposta certa:** d) Os valores calculados para as observações da amostra com base nos fatores formam variáveis quantitativas.

**Explicação:** A resposta é que os valores dos fatores para cada observação formam variáveis quantitativas. Cada fator é uma combinação linear de variáveis métricas padronizadas, então resulta em número contínuo. Por isso podem ser usados como entrada em outras técnicas, como a análise de agrupamentos.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 458

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-2
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Assinale a alternativa que apresenta a correta interpretação para a carga fatorial de uma análise fatorial por componentes principais:

- a) Elevados valores indicam elevada correlação de Pearson entre a variável original e o fator em análise.
- b) Elevados valores indicam baixa correlação de Pearson entre a variável original e o fator em análise.
- c) Elevados valores indicam baixa significância do p-valor da variável original com o fator em análise.
- d) Elevados valores indicam elevada perda de variância para a variável original no fator em análise.

**Resposta certa:** a) Elevados valores indicam elevada correlação de Pearson entre a variável original e o fator em análise.

**Explicação:** A resposta é que valores elevados indicam alta correlação de Pearson entre a variável original e o fator. Quanto maior a carga, mais o fator é influenciado por aquela variável. Carga baixa indica pouca relação entre os dois.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-3
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Na criação de rankings a partir dos fatores extraídos de uma análise fatorial por componentes principais, o critério da soma ponderada e ordenamento indica que:

- a) Cada fator extraído é ponderado por seu percentual de variância compartilhada e depois é realizado o ordenamento do resultado da soma.
- b) Todos os fatores devem ter o mesmo peso na criação do ranking para posterior ordenamento.
- c) Somente o primeiro fator deve ser o representante dos resultados na criação do ranking.
- d) Utiliza-se o fator com o menor percentual de variância compartilhada para o ordenamento.

**Resposta certa:** a) Cada fator extraído é ponderado por seu percentual de variância compartilhada e depois é realizado o ordenamento do resultado da soma.

**Explicação:** A resposta é que cada fator é ponderado pelo seu percentual de variância compartilhada e depois se ordena o resultado da soma. Ri é a soma de cada fator multiplicado pelo seu percentual. Pesos iguais ou só o primeiro fator seriam outros critérios.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 20

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-4
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Considere os conceitos discutidos em aula sobre os autovalores e assinale a alternativa correta:

- a) Os autovalores mostram o percentual da variância compartilhada pelas variáveis originais para a formação de cada fator extraído, ou seja, mostram a quantidade de informação contida em cada fator.
- b) Os autovalores negativos indicam fatores que explicam mais variância do que os autovalores positivos, sendo preferível reter apenas os fatores com autovalores negativos na análise.
- c) Os autovalores devem sempre somar zero para garantir que a análise fatorial seja válida e que os fatores extraídos sejam ortogonais entre si.
- d) Os autovalores são sempre iguais a 1 em qualquer análise de componentes principais, independentemente do número de variáveis ou da estrutura de correlação dos dados.

**Resposta certa:** a) Os autovalores mostram o percentual da variância compartilhada pelas variáveis originais para a formação de cada fator extraído, ou seja, mostram a quantidade de informação contida em cada fator.

**Explicação:** A resposta é a que diz que os autovalores mostram o percentual da variância compartilhada pelas variáveis originais para formar cada fator. É a quantidade de informação do fator. Autovalor negativo não faz sentido numa matriz de correlações, e eles somam k, o número de variáveis, não zero nem sempre 1.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 12

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-5
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Assinale a alternativa que apresenta uma característica relativa ao fator derivado do maior autovalor da análise fatorial PCA:

- a) É o fator que apresenta correlações de Pearson positivas com todas as variáveis originais utilizadas na análise.
- b) É o fator que apresenta correlações de Pearson negativas com todas as variáveis originais utilizadas na análise.
- c) É o fator que contém o maior percentual da variância compartilhada pelas variáveis originais para sua formação.
- d) É o fator menos importante resultante da análise fatorial e, portanto, será excluído pelo critério de Kaiser.

**Resposta certa:** c) É o fator que contém o maior percentual da variância compartilhada pelas variáveis originais para sua formação.

**Explicação:** A resposta é que o fator do maior autovalor tem o maior percentual de variância compartilhada. Os autovalores são ordenados do maior para o menor, então o primeiro fator concentra mais informação. Ele é o mais importante, e por isso passa pelo critério de Kaiser quando é maior que 1.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 12

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-6
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Ao observar um score fatorial muito próximo a zero em determinado fator extraído por meio da Análise Fatorial PCA, interpreta-se que:

- a) A variável referente a tal score não exerce influência relevante no fator em análise.
- b) A variável referente a tal score exerce influência moderada no fator em análise.
- c) A variável referente a tal score exerce elevada influência no fator em análise.
- d) A variável referente a tal score é a única que exerce influência no fator em análise.

**Resposta certa:** a) A variável referente a tal score não exerce influência relevante no fator em análise.

**Explicação:** A resposta é que a variável não exerce influência relevante no fator. O valor próximo de zero (carga fatorial, como a aula trata) indica correlação quase nula entre variável e fator. Quanto maior em módulo, maior a influência.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-7
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

A aplicação do critério da raiz latente em uma análise fatorial por componentes principais resulta em:

- a) Um ganho de variância acima daquela existente nas variáveis originais, pois alguns fatores são deixados de fora da análise final.
- b) Um ganho de variância acima daquela existente nas variáveis originais, pois alguns fatores são criados a partir das variáveis originais.
- c) Uma perda de variância das variáveis originais, pois alguns fatores são deixados de fora da análise final.
- d) Um número de fatores maior do que a quantidade de variáveis originais existente na análise.

**Resposta certa:** c) Uma perda de variância das variáveis originais, pois alguns fatores são deixados de fora da análise final.

**Explicação:** A resposta é uma perda de variância das variáveis originais, porque alguns fatores ficam de fora. Ficando só os fatores com autovalor maior que 1, parte da variância compartilhada se perde, e as comunalidades mostram quanto sobrou de cada variável. Não existe ganho de variância nem mais fatores que variáveis.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-8
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Após a aplicação do critério da raiz latente em uma análise fatorial PCA, foram obtidos os seguintes resultados de comunalidades para as variáveis da análise:

Variável A = 0.92

Variável B = 0.85

Variável C = 0.32

Assinale a alternativa correta em relação à interpretação do resultado:
Após a aplicação do critério da raiz latente em uma análise fatorial PCA, foram obtidos os seguintes resultados de comunalidades para as variáveis da análise:
Variável A = 0.92
Variável B = 0.85
Variável C = 0.32
Assinale a alternativa correta em relação à interpretação do resultado:

- a) A Variável B apresentou a maior perda de variância.
- b) A Variável C apresentou a maior perda de variância.
- c) Nenhuma variável apresentou perda de variância.
- d) A Variável A apresentou a maior perda de variância.

**Resposta certa:** b) A Variável C apresentou a maior perda de variância.

**Explicação:** A resposta é que a Variável C teve a maior perda de variância. A comunalidade é a variância da variável retida nos fatores selecionados, então a perda é 1 menos ela: A perdeu 0,08, B perdeu 0,15 e C perdeu 1 - 0,32 = 0,68.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 162549-1-9
Área 1 · Unsupervised Machine Learning: Análise Fatorial e PCA II

Em uma modelagem de análise fatorial por componentes principais, foi feita a análise inicial dos autovalores resultantes e foi obtida a seguinte lista de autovalores. De acordo com o critério de Kaiser, a PCA deve ser parametrizada com quantos fatores?
[1.90, 1.28, 1.20, 1.16, 0.41, 0.05]

- a) 3.
- b) 2.
- c) 1.
- d) 4.

**Resposta certa:** d) 4.

**Explicação:** A resposta é 4. Pelo critério de Kaiser ficam os fatores com autovalor maior que 1, que aqui são 1,90, 1,28, 1,20 e 1,16. Os autovalores 0,41 e 0,05 ficam de fora.

**Fonte:** Aula de Análise Fatorial e PCA, pág. 17

**Situação:** explicação conferida com o material das aulas

---

## Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

### Questão 166670-1-1
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

A tabela de contingência ou tabela de classificação cruzada apresenta:

- a) As frequências absolutas observadas para cada par de categorias das variáveis.
- b) As frequências absolutas esperadas para cada par de categorias das variáveis.
- c) Os resíduos para cada par de categorias das variáveis.
- d) Os valores tabela de qui-quadrado para cada par de categorias das variáveis.

**Resposta certa:** a) As frequências absolutas observadas para cada par de categorias das variáveis.

**Explicação:** A resposta é as frequências absolutas observadas, porque a tabela de contingência (ou classificação cruzada) é o ponto de partida da análise: cada célula conta quantos casos caem no cruzamento de duas categorias. As frequências esperadas, os resíduos e os valores de qui-quadrado são tabelas derivadas dela, calculadas depois.

**Fonte:** Aula de Análise de Correspondência, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-10
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

São exemplos de variáveis qualitativas, EXCETO:

- a) Classificação em faixas de idade.
- b) Preço em Reais de um produto.
- c) Bairro do imóvel destinado à venda.
- d) Respostas sim ou não no questionário.

**Resposta certa:** b) Preço em Reais de um produto.

**Explicação:** A resposta é o preço em reais de um produto, porque é uma variável quantitativa, medida em escala numérica. Faixa de idade, bairro e resposta sim ou não são categorias. A faixa de idade engana por vir de um número, mas já está agrupada em categorias.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 166670-1-2
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Em relação às análises de correspondência simples e múltipla, pode-se afirmar que:

- a) Em um mapa perceptual, quanto mais próximas estiverem duas categorias, maior é a associação entre elas.
- b) Na análise de correspondência múltipla, é fundamental definir um modelo em que se identifique quais são as variáveis dependentes e independentes.
- c) Não permitem verificar como as categorias das variáveis se associam entre elas.
- d) A análise de correspondência simples pode ser realizada para mais de duas variáveis.

**Resposta certa:** a) Em um mapa perceptual, quanto mais próximas estiverem duas categorias, maior é a associação entre elas.

**Explicação:** A resposta é que, no mapa perceptual, categorias mais próximas indicam maior associação entre elas. A proximidade é justamente o que o mapa mostra. As outras alternativas erram: a técnica é exploratória e não exige variável dependente, ela serve para ver como as categorias se associam, e a versão simples trabalha com apenas duas variáveis.

**Fonte:** Aula de Análise de Correspondência, pág. 4, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-3
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Se o p-valor da estatística qui-quadrado resultante de uma tabela de contingência indicar p-value = 0.62, é CORRETO afirmar que:

- a) A análise de correspondência é viável, pois não existe associação significativa ao nível de significância de 5% entre as variáveis.
- b) A análise de correspondência não é viável, pois não existe associação significativa ao nível de significância de 5% entre as variáveis.
- c) A análise de correspondência não viável, pois existe associação significativa ao nível de significância de 5% entre as variáveis.
- d) A análise de correspondência é viável, pois existe associação significativa ao nível de significância de 5% entre as variáveis.

**Resposta certa:** b) A análise de correspondência não é viável, pois não existe associação significativa ao nível de significância de 5% entre as variáveis.

**Explicação:** A resposta é que a análise não é viável. Com p-valor de 0,62, bem acima de 0,05, não se rejeita a hipótese nula de independência, então não há associação significativa entre as variáveis. Sem associação não há o que representar no mapa perceptual, e o teste qui-quadrado é a etapa que libera ou não a análise.

**Fonte:** Aula de Análise de Correspondência, pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-4
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Sobre a interpretação do mapa perceptual resultante da análise de correspondência, é CORRETO afirmar que:

- a) Quanto mais próximas as categorias das variáveis, maior tende a ser a associação.
- b) A associação entre categorias das variáveis ocorre somente quando há sobreposição dos pontos no mapa perceptual.
- c) Quanto mais distantes as categorias das variáveis, maior tende a ser a associação.
- d) Quanto mais próximas as categorias das variáveis, menor tende a ser a associação.

**Resposta certa:** a) Quanto mais próximas as categorias das variáveis, maior tende a ser a associação.

**Explicação:** A resposta é que categorias mais próximas tendem a ter maior associação. A leitura do mapa perceptual é essa: a proximidade entre os pontos indica o motivo da associação. A alternativa da sobreposição exige demais, pois não é preciso que os pontos coincidam, e as de distância e de menor associação invertem a lógica.

**Fonte:** Aula de Análise de Correspondência, pág. 4

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-5
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Se há uma variável quantitativa no banco de dados e o analisa deseja analisá-la no contexto da Análise de Correspondência, uma solução CORRETA é:

- a) Calcular as matrizes de correlações de Pearson com as demais variáveis qualitativas.
- b) Realizar previamente um procedimento de categorização da variável quantitativa.
- c) Calcular as matrizes de distâncias Euclidianas com as demais variáveis qualitativas.
- d) Adicioná-la à análise sem que seja feito qualquer tratamento prévio.

**Resposta certa:** b) Realizar previamente um procedimento de categorização da variável quantitativa.

**Explicação:** A resposta é categorizar a variável quantitativa antes da análise. A análise de correspondência só trabalha com variáveis categóricas, então um valor numérico como a idade precisa virar faixas (por exemplo 0 a 30, 31 a 60, 61 a 90 anos). Correlação de Pearson e distância euclidiana não fazem parte da técnica, e incluir a variável crua não funciona.

**Fonte:** Aula de Análise de Correspondência, pág. 3

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-6
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Em uma tabela de contingência entre duas variáveis categóricas, o valor da estatística qui-quadrado da tabela e seu p-valor são utilizados para:

- a) Analisar os resíduos para cada par de categorias das variáveis em análise.
- b) Analisar se existe associação estatisticamente significativa entre as variáveis.
- c) Identificar as proporções totais de cada categoria da variável em coluna.
- d) Identificar as proporções totais de cada categoria da variável em linha.

**Resposta certa:** b) Analisar se existe associação estatisticamente significativa entre as variáveis.

**Explicação:** A resposta é analisar se existe associação estatisticamente significativa entre as variáveis. O qui-quadrado total e seu p-valor testam a hipótese de que as variáveis são independentes. A análise dos resíduos por par de categorias é um passo seguinte, que aprofunda o resultado, e não a função do qui-quadrado total.

**Fonte:** Aula de Análise de Correspondência, pág. 3, pág. 14

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-7
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Em relação às Análises de Correspondência Simples e Múltipla, é INCORRETO afirmar que são técnicas:

- a) Relacionadas à análise de mapas perceptuais.
- b) Que permitem a análise de variáveis categóricas.
- c) Adequadas para a análise de variáveis quantitativas.
- d) Utilizam-se das tabelas de contingência como base inicial de análise.

**Resposta certa:** c) Adequadas para a análise de variáveis quantitativas.

**Explicação:** A resposta é que as técnicas não são adequadas para variáveis quantitativas, e por isso essa é a afirmação incorreta. Tanto a análise simples quanto a múltipla servem a variáveis categóricas, partem de tabelas de contingência (ou da matriz de Burt) e produzem mapas perceptuais. Uma variável numérica só entra depois de categorizada.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 467

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-8
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

Considere os conceitos discutidos em aula sobre a Análise de Correspondência e assinale a alternativa CORRETA:

- a) Caso exista uma variável quantitativa que deva participar da análise, não é necessário que ela passe, previamente, por um procedimento de categorização.
- b) A análise de correspondência é uma técnica supervisionada.
- c) A análise de correspondência é adequada para fins de inferência.
- d) A análise de correspondência é uma técnica não supervisionada (exploratória).

**Resposta certa:** d) A análise de correspondência é uma técnica não supervisionada (exploratória).

**Explicação:** A resposta é que a análise de correspondência é uma técnica não supervisionada, de caráter exploratório. Ela estuda a interdependência entre as variáveis, sem modelo do tipo Y = f(X), e por isso não serve para inferência. Quanto à variável quantitativa, ela precisa ser categorizada antes, então a primeira alternativa também está errada.

**Fonte:** Aula de Análise de Correspondência, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 166670-1-9
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla I - 13/01/26

A análise dos resíduos padronizados ajustados permite:

- a) Verificar as coordenadas das categorias das variáveis que serão plotadas no mapa.
- b) Verificar as coordenadas das observações que serão plotadas no mapa.
- c) Verificar a contagem de observações para cada par de categorias das variáveis.
- d) Verificar se existe associação significativa entre pares de categorias das variáveis.

**Resposta certa:** d) Verificar se existe associação significativa entre pares de categorias das variáveis.

**Explicação:** A resposta é verificar se existe associação significativa entre pares de categorias. O resíduo padronizado ajustado de cada célula é comparado com 1,96: acima disso, a associação entre as duas categorias é significativa a 5%. Já o qui-quadrado total só diz se as variáveis, como um todo, se associam.

**Fonte:** Aula de Análise de Correspondência, pág. 16, pág. 19

**Situação:** explicação conferida com o material das aulas

---

## Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

### Questão 167434-1-1
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

Ao aplicar o teste qui-quadrado para associação entre duas variáveis qualitativas, se o p-valor indicar a não rejeição da hipótese nula, então a conclusão é que:

- a) As variáveis não apresentam associação estatisticamente significativa entre elas.
- b) As categorias com menos observações devem ser excluídas da análise.
- c) As variáveis apresentam associação estatisticamente significativa entre elas.
- d) Todas as categorias das variáveis associam-se fortemente entre elas.

**Resposta certa:** a) As variáveis não apresentam associação estatisticamente significativa entre elas.

**Explicação:** A resposta é que as variáveis não apresentam associação estatisticamente significativa. No teste qui-quadrado a hipótese nula é de independência entre as variáveis, e não rejeitá-la significa que não há evidência de associação. Isso não diz nada sobre excluir categorias com poucas observações.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 303

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-10
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

A matriz de Burt é um método utilizado para:

- a) Implementar a Análise Fatorial por Componentes Principais.
- b) Viabilizar a geração do mapa perceptual da Análise de Correspondência Múltipla.
- c) Realizar o teste qui-quadrado para associação.
- d) Transformar variáveis quantitativas em qualitativas.

**Resposta certa:** b) Viabilizar a geração do mapa perceptual da Análise de Correspondência Múltipla.

**Explicação:** A resposta é viabilizar o mapa perceptual da ACM. A matriz de Burt (B = Z'Z) reúne em uma só matriz o cruzamento de todos os pares de variáveis e, tratada como tabela de contingência, permite fazer uma análise simples e obter as coordenadas das categorias. Ela não faz análise fatorial, nem o qui-quadrado, nem categoriza variáveis.

**Fonte:** Aula de Análise de Correspondência, pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-2
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

Sobre as técnicas Análises de Correspondência Simples e Múltipla, é CORRETO afirmar que:

- a) Permitem somente a análise de variáveis quantitativas contínuas.
- b) São adequadas para a análise de variáveis qualitativas.
- c) São fundamentadas na análise das distâncias Euclidianas entre as observações.
- d) Utilizam-se das matrizes de correlações de Pearson como ponto inicial da análise.

**Resposta certa:** b) São adequadas para a análise de variáveis qualitativas.

**Explicação:** A resposta é que as técnicas são adequadas para variáveis qualitativas. A análise de correspondência simples e a múltipla trabalham com variáveis categóricas e estudam a associação entre elas e entre suas categorias. Distâncias euclidianas entre observações e correlação de Pearson pertencem a outras técnicas, como cluster e análise fatorial.

**Fonte:** Aula de Análise de Correspondência, pág. 3

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-3
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

No mapa perceptual da Análise de Correspondência Simples, os dois eixos representam:

- a) As contagens de observações em cada variável incluída na análise.
- b) O percentual de observações estatisticamente significativas de cada variável.
- c) As duas primeiras dimensões formadas a partir dos dois maiores autovalores.
- d) A quantidade de categorias presentes em cada variável incluída na análise.

**Resposta certa:** c) As duas primeiras dimensões formadas a partir dos dois maiores autovalores.

**Explicação:** A resposta é as duas primeiras dimensões, formadas pelos dois maiores autovalores. Cada autovalor é a inércia principal parcial de uma dimensão, e o mapa bidimensional usa as duas que concentram mais inércia, ou seja, que explicam mais da associação. Os eixos não representam contagens nem número de categorias.

**Fonte:** Aula de Análise de Correspondência, pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-4
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

Assinale a alternativa CORRETA em relação à técnica de Análise de Correspondência Múltipla.

- a) É uma técnica que só é aplicada quando há mais de duas variáveis quantitativas.
- b) É uma técnica que só é aplicada quando há no máximo duas variáveis categóricas.
- c) É uma técnica que recebe uma análise de correspondência simples como input e é rodada múltiplas vezes até retornar o resultado.
- d) É uma técnica para estudar as associações entre mais de duas variáveis categóricas e entre suas categorias, bem como a intensidade dessas associações.

**Resposta certa:** d) É uma técnica para estudar as associações entre mais de duas variáveis categóricas e entre suas categorias, bem como a intensidade dessas associações.

**Explicação:** A resposta é que a ACM estuda as associações entre mais de duas variáveis categóricas e entre suas categorias, além da intensidade delas. Ela é a extensão natural da análise simples, que se limita a duas variáveis. Também não é uma sequência de análises simples repetidas, e não se aplica a variáveis quantitativas.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 493

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-5
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

Assinale a alternativa que apresenta dois métodos pertinentes à elaboração da Análise de Correspondência Múltipla.

- a) K-means e matriz de dissimilaridades.
- b) Matriz binária e matriz de Burt.
- c) Matriz de correlação de Pearson e matriz de Burt.
- d) Matriz binária e distância Euclidiana.

**Resposta certa:** b) Matriz binária e matriz de Burt.

**Explicação:** A resposta é matriz binária e matriz de Burt. São os dois métodos da ACM: o da matriz binária Z gera coordenadas-padrão, e o da matriz de Burt (B = Z'Z) gera coordenadas principais, tratando a matriz como uma tabela de contingência. K-means, correlação de Pearson e distância euclidiana não fazem parte da ACM.

**Fonte:** Aula de Análise de Correspondência, pág. 31, pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-6
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

O mapa perceptual de uma Análise de Correspondência Múltipla deve ser interpretado com base:

- a) No formato do histograma gerado a partir das múltiplas variáveis da análise.
- b) Na proximidade ou distância entre as categorias das variáveis plotadas no mapa.
- c) Na contagem das categorias que foram estatisticamente plotadas no mapa.
- d) Na significância estatística das observações mais frequentemente plotadas mapa.

**Resposta certa:** b) Na proximidade ou distância entre as categorias das variáveis plotadas no mapa.

**Explicação:** A resposta é a proximidade ou distância entre as categorias plotadas. Na ACM a interpretação é a mesma da análise simples: categorias próximas no mapa indicam associação. Histograma, contagem de categorias plotadas e significância de observações não são critérios de leitura do mapa.

**Fonte:** Aula de Análise de Correspondência, pág. 4

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-7
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

Em uma Análise de Correspondência Simples, uma das variáveis apresenta 4 categorias e a outra variável apresenta 5 categorias. Qual é o número máximo de dimensões que pode ser extraído em tal análise?

- a) 5.
- b) 6.
- c) 4.
- d) 3.

**Resposta certa:** d) 3.

**Explicação:** A resposta é 3. O número máximo de dimensões (autovalores) é o mínimo entre linhas menos 1 e colunas menos 1: m = min(4 - 1, 5 - 1) = min(3, 4) = 3. A tentação é pegar o 4 ou o 5, que são as categorias, mas a conta sempre desconta 1.

**Fonte:** Aula de Análise de Correspondência, pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-8
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

Em uma Análise de Correspondência Múltipla, se a variável “A” não apresentar associação estatisticamente significativa com pelo menos uma outra variável da análise, então a variável “A”:

- a) Não pode ser considerada uma variável qualitativa.
- b) Deve ser considerada como a variável mais importante da análise.
- c) Deve ser avaliada por meio da correlação de Pearson com as demais variáveis.
- d) Pode ser retirada da Análise de Correspondência Múltipla.

**Resposta certa:** d) Pode ser retirada da Análise de Correspondência Múltipla.

**Explicação:** A resposta é que a variável A pode ser retirada da ACM. Só participam da análise as variáveis com associação significativa com pelo menos uma das outras no teste qui-quadrado. Por isso se roda o teste para cada par de variáveis antes da ACM, e quem não se associa com nenhuma sai.

**Fonte:** Aula de Análise de Correspondência, pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 167434-1-9
Área 1 · Unsupervised Machine Learning: Análise de Correspondência Simples e Múltipla II

No estudo de viabilidade da Análise de Correspondência Múltipla, uma etapa essencial é:

- a) Calcular a média, mediana, mínimo e o máximo para cada variável incluída na análise.
- b) Realizar, previamente, o procedimento de padronização pelo Z-Score em todas as variáveis.
- c) Analisar individualmente, para todas as variáveis, as frequências acumuladas nas categorias.
- d) Analisar se cada variável tem associação estatisticamente significativa com pelo menos uma outra variável em estudo.

**Resposta certa:** d) Analisar se cada variável tem associação estatisticamente significativa com pelo menos uma outra variável em estudo.

**Explicação:** A resposta é analisar se cada variável tem associação significativa com pelo menos uma outra. Antes de rodar a ACM faz-se o teste qui-quadrado para cada par de variáveis, e quem não se associa com nenhuma é excluída. Medidas descritivas e Z-Score valem para variáveis quantitativas, não para as categóricas da ACM.

**Fonte:** Aula de Análise de Correspondência, pág. 30

**Situação:** explicação conferida com o material das aulas

---

## Unsupervised Machine Learning: Clustering I

### Questão 160042-1-1
Área 1 · Unsupervised Machine Learning: Clustering I

Sobre os métodos de encadeamento na análise de cluster, quando houver pelo menos um cluster formado, é correto afirmar que:

- a) O single linkage privilegia as menores distâncias entre observações.
- b) O complete linkage privilegia as menores distâncias entre as observações.
- c) O average linkage privilegia as menores distâncias entre as observações.
- d) O complete linkage privilegia as distâncias médias entre as observações.

**Resposta certa:** a) O single linkage privilegia as menores distâncias entre observações.

**Explicação:** A resposta é que o single linkage (vizinho mais próximo) privilegia as menores distâncias, pois a distância entre clusters é o mínimo entre as distâncias das observações. O complete linkage faz o oposto e usa a maior distância, e o average linkage usa a média entre todos os pares. É por isso que as outras três alternativas estão trocadas.

**Fonte:** Aula de Clustering, pág. 15, pág. 17

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-10
Área 1 · Unsupervised Machine Learning: Clustering I

Assinale a alternativa correta em relação ao objetivo geral em uma análise de clusters.

- a) Criar grupos homogêneos internamente e heterogêneos entre si.
- b) Criar grupos homogêneos internamente e homogêneos entre si.
- c) Criar grupos heterogêneos internamente e heterogêneos entre si.
- d) Criar grupos heterogêneos internamente e homogêneos entre si.

**Resposta certa:** a) Criar grupos homogêneos internamente e heterogêneos entre si.

**Explicação:** A resposta é grupos homogêneos internamente e heterogêneos entre si. Dentro de cada grupo as observações devem ser parecidas nas variáveis usadas, e entre grupos devem ser diferentes. As outras combinações contradem a ideia de agrupar: grupos heterogêneos por dentro ou iguais entre si não separariam nada.

**Fonte:** Aula de Clustering, pág. 3

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-2
Área 1 · Unsupervised Machine Learning: Clustering I

Dentre os elementos listados a seguir, assinale a alternativa que contém os elementos diretamente relacionados à análise de cluster hierárquica aglomerativa.

- a) Alta capacidade inferencial; tabela de contingência para variáveis categóricas.
- b) Medidas de dissimilaridade; métodos de encadeamento.
- c) Matriz de correlações de Pearson; teste qui-quadrado para associações.
- d) Intervalo de confiança para média; modelo preditivo.

**Resposta certa:** b) Medidas de dissimilaridade; métodos de encadeamento.

**Explicação:** A resposta é medidas de dissimilaridade e métodos de encadeamento, que são as duas escolhas que a análise hierárquica aglomerativa exige: a distância entre observações (como a euclidiana) e a regra de distância entre clusters já formados. Inferência, tabela de contingência, qui-quadrado e intervalo de confiança pertencem a outras técnicas.

**Fonte:** Aula de Clustering, pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-3
Área 1 · Unsupervised Machine Learning: Clustering I

Na análise de cluster hierárquica aglomerativa, assinale a alternativa correta em relação ao uso do dendrograma.

- a) É utilizado para calcular a matriz de distâncias.
- b) É utilizado para padronizar as variáveis por meio do ZScore antes da realização da análise.
- c) É utilizado com a finalidade de visualizar graficamente a formação dos clusters.
- d) Tem a finalidade de apresentar todas as opções de medidas de dissimilaridade para a realização da análise.

**Resposta certa:** c) É utilizado com a finalidade de visualizar graficamente a formação dos clusters.

**Explicação:** A resposta é visualizar graficamente a formação dos clusters. O dendrograma mostra a ordem em que observações e grupos vão sendo unidos ao longo dos estágios e as distâncias de cada união. Ele não calcula a matriz de distâncias, não padroniza variáveis e não lista medidas de dissimilaridade.

**Fonte:** Aula de Clustering, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-4
Área 1 · Unsupervised Machine Learning: Clustering I

Considerando um banco de dados com 20 observações a serem clusterizadas pelo método hierárquico aglomerativo, assinale a alternativa que contém o número correto de clusters existentes no estágio zero da clusterização?

- a) 1.
- b) 20.
- c) 0.
- d) 10.

**Resposta certa:** b) 20.

**Explicação:** A resposta é 20. No método hierárquico aglomerativo o estágio zero começa com cada observação sozinha, então n observações dão n clusters. Só depois as duas mais próximas se unem (n - 1 clusters) e o processo segue até restar um único cluster. Com n = 20, o estágio zero tem 20.

**Fonte:** Aula de Clustering, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-5
Área 1 · Unsupervised Machine Learning: Clustering I

No contexto da análise de clusters, assinale a alternativa que indica corretamente quando é necessário aplicar o procedimento inicial de ZScore nas variáveis.

- a) É sempre necessário, sem exceção.
- b) Quando as variáveis já estiverem previamente padronizadas.
- c) Quando as variáveis apresentarem diferenças nas unidades de medidas.
- d) Nunca é necessário, pois as escalas se ajustam automaticamente.

**Resposta certa:** c) Quando as variáveis apresentarem diferenças nas unidades de medidas.

**Explicação:** A resposta é quando as variáveis têm unidades de medida diferentes. A distância entre observações é sensível à escala, e uma variável em unidade maior dominaria as demais. O Z-Score deixa todas com média 0 e desvio padrão 1. Se já estão na mesma unidade, não há necessidade, e o procedimento não é automático.

**Fonte:** Aula de Clustering, pág. 9

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-6
Área 1 · Unsupervised Machine Learning: Clustering I

Assinale a alterativa que apresenta a principal característica do método de encadeamento average linkage quando houver pelo menos um cluster formado na análise.

- a) Utiliza como referência a distância média entre as observações.
- b) Utiliza como referência a distância entre as observações mais próximas.
- c) Não utiliza medidas de distância entre as observações como referência.
- d) Utiliza como referência a distância entre as observações mais distantes.

**Resposta certa:** a) Utiliza como referência a distância média entre as observações.

**Explicação:** A resposta é a distância média entre as observações. No average linkage (between groups) a união de dois grupos é feita pela média das distâncias entre todos os pares de observações dos dois grupos. A distância das mais próximas é o single linkage e a das mais distantes é o complete linkage.

**Fonte:** Aula de Clustering, pág. 15

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-7
Área 1 · Unsupervised Machine Learning: Clustering I

Em um banco de dados com 100 observações a serem clusterizadas pelo método hierárquico aglomerativo, qual é o número de clusters existente ao final de todos os estágios de clusterização?

- a) 50.
- b) 1.
- c) 0.
- d) 100.

**Resposta certa:** b) 1.

**Explicação:** A resposta é 1. O método aglomerativo repete a união n - 1 vezes até sobrar um único cluster com todas as observações, não importando o tamanho da amostra. Com 100 observações, começa com 100 clusters no estágio zero e termina com 1 depois de 99 uniões.

**Fonte:** Aula de Clustering, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-8
Área 1 · Unsupervised Machine Learning: Clustering I

Em relação à escolha do método de encadeamento para uma análise de cluster hierárquica aglomerativa, assinale a alternativa correta.

- a) É irrelevante, pois sempre resultam na mesma medida de dissimilaridade independentemente do método escolhido.
- b) É relevante, pois métodos de encadeamento distintos podem gerar quantidades diferentes de clusters no estágio zero da análise.
- c) É relevante, pois métodos de encadeamento distintos podem gerar agrupamentos distintos.
- d) É irrelevante, pois sempre resultam no mesmo agrupamento independentemente do método de encadeamento escolhido.

**Resposta certa:** c) É relevante, pois métodos de encadeamento distintos podem gerar agrupamentos distintos.

**Explicação:** A resposta é que a escolha é relevante porque métodos de encadeamento diferentes podem gerar agrupamentos diferentes. O método define qual distância entre clusters é usada (mínima, máxima ou média), e isso muda quem se junta com quem. Por isso é comum comparar dendrogramas de métodos distintos. O estágio zero é sempre n clusters, qualquer que seja o método.

**Fonte:** Aula de Clustering, pág. 10, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 160042-1-9
Área 1 · Unsupervised Machine Learning: Clustering I

Assinale a alternativa INCORRETA sobre conceitos relativos à análise de clusters:

- a) Os resultados não têm caráter preditivo para observações de fora da amostra.
- b) Trata-se de uma técnica não supervisionada de machine learning.
- c) A adição de novas observações ao banco de dados pode alterar os agrupamentos.
- d) A análise de clusters tem como resultado a criação de modelos preditivos.

**Resposta certa:** d) A análise de clusters tem como resultado a criação de modelos preditivos.

**Explicação:** A resposta é a alternativa que diz que a análise de clusters cria modelos preditivos, que é a incorreta. Cluster é técnica exploratória e não supervisionada, sem caráter preditivo para observações de fora da amostra, e incluir ou retirar observações pode mudar os grupos. As outras três afirmações estão corretas.

**Fonte:** Aula de Clustering, pág. 6

**Situação:** explicação conferida com o material das aulas

---

## Unsupervised Machine Learning: Clustering II

### Questão 160647-1-1
Área 1 · Unsupervised Machine Learning: Clustering II

Assinale a alternativa que apresenta corretamente uma diferença entre o Método Hierárquico Aglomerativo e o Método Não Hierárquico K-means:

- a) No K-means, a quantidade de clusters é escolhida no passo a passo do esquema de aglomeração; no método hierárquico, a quantidade de clusters é escolhida antes de iniciar a análise.
- b) No K-means, a quantidade de clusters é escolhida a priori; no método hierárquico, a quantidade de clusters é escolhida no passo a passo do esquema de aglomeração.
- c) No K-means, o método de encadeamento é escolhido a priori; no método hierárquico, o método de encadeamento é escolhido no passo a passo do esquema de aglomeração.
- d) No K-means, o método de encadeamento é escolhido no passo a passo do esquema de aglomeração; no método hierárquico, o método de encadeamento é escolhido a priori.

**Resposta certa:** b) No K-means, a quantidade de clusters é escolhida a priori; no método hierárquico, a quantidade de clusters é escolhida no passo a passo do esquema de aglomeração.

**Explicação:** A resposta é que no K-means a quantidade de clusters é escolhida a priori, e no hierárquico ela é definida ao longo do esquema de aglomeração, passo a passo. O método de encadeamento existe só no hierárquico, e o K-means trabalha com centroides, por isso as alternativas sobre encadeamento estão erradas.

**Fonte:** Aula de Clustering, pág. 7, pág. 22

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-10
Área 1 · Unsupervised Machine Learning: Clustering II

Assinale a alternativa correta em relação aos procedimentos de clusterização:

- a) Não é correto utilizar o resultado sobre a quantidade de clusters de uma clusterização hierárquica aglomerativa como input do modelo k-means.
- b) Após o K-means, o teste F calcula a variabilidade entre os grupos dividida pela variabilidade dentro dos grupos para cada variável para analisar quais contribuíram para a formação de pelo menos um grupo.
- c) No método K-means, um cluster pode ter vários centroides.
- d) O método k-means apresenta mais limitações para trabalhar em bancos de dados com grande volume de dados quando se comparado ao método hierárquico.

**Resposta certa:** b) Após o K-means, o teste F calcula a variabilidade entre os grupos dividida pela variabilidade dentro dos grupos para cada variável para analisar quais contribuíram para a formação de pelo menos um grupo.

**Explicação:** A resposta é a do teste F depois do K-means: ele divide a variabilidade entre grupos pela variabilidade dentro dos grupos, para cada variável, e as de maior F contribuíram mais para formar ao menos um cluster. As outras estão erradas: o resultado do hierárquico pode alimentar o K-means, cada cluster tem um centroide, e o K-means lida melhor com amostras grandes.

**Fonte:** Aula de Clustering, pág. 19, pág. 27

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-2
Área 1 · Unsupervised Machine Learning: Clustering II

Em relação ao método de Elbow para identificação da quantidade de clusters, assinale a afirmativa correta:

- a) O método de Elbow e o dendrograma representam os mesmos métodos para a identificação do número ideal de clusters.
- b) Apresenta um gráfico da soma dos quadrados totais internos aos clusters em função do número de clusters.
- c) O método retorna exatamente qual é a quantidade de clusters que deve ser utilizada na modelagem.
- d) Esse método só pode ser utilizado quando a modelagem é uma clusterização hierárquica aglomerativa.

**Resposta certa:** b) Apresenta um gráfico da soma dos quadrados totais internos aos clusters em função do número de clusters.

**Explicação:** A resposta é que o Elbow apresenta o gráfico da soma dos quadrados dentro dos clusters (WCSS) para vários valores de K. Busca-se o cotovelo, ponto em que a queda da WCSS deixa de ser expressiva. Ele não dá um número exato, não é o dendrograma e é usado no K-means, não no hierárquico.

**Fonte:** Aula de Clustering, pág. 26

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-3
Área 1 · Unsupervised Machine Learning: Clustering II

Em relação ao dendrograma, é INCORRETO afirmar que:

- a) Auxilia na identificação da quantidade de clusters no método hierárquico aglomerativo.
- b) Seu estágio final mostra todas as observações agrupadas em um único cluster.
- c) Pode ser interpretado com base nos saltos de distâncias para união de observações.
- d) É um output referente ao método de clusterização não hierárquico K-means.

**Resposta certa:** d) É um output referente ao método de clusterização não hierárquico K-means.

**Explicação:** A resposta é a que diz que o dendrograma é output do K-means, que é a afirmação incorreta. O dendrograma é do método hierárquico aglomerativo: mostra a formação dos clusters até o estágio final com um único cluster e permite ler os saltos de distância. O K-means trabalha com centroides, e o dendrograma fica difícil de ler em amostras grandes.

**Fonte:** Aula de Clustering, pág. 27

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-4
Área 1 · Unsupervised Machine Learning: Clustering II

Assinale a alterativa que apresenta a principal característica do método de encadeamento “complete linkage” para a realização de uma clusterização hierárquica aglomerativa:

- a) Utiliza como referência a distância média entre as observações quando há pelo menos um cluster formado.
- b) Utiliza como referência a distância entre as observações mais distantes quando há pelo menos um cluster formado.
- c) Utiliza como referência a distância entre as observações mais próximas quando há pelo menos um cluster formado.
- d) Não utiliza medidas de distância entre as observações como referência para o agrupamento.

**Resposta certa:** b) Utiliza como referência a distância entre as observações mais distantes quando há pelo menos um cluster formado.

**Explicação:** A resposta é a distância entre as observações mais distantes. No complete linkage (furthest neighbor) a distância entre clusters é o máximo entre as distâncias de suas observações, d(MN)W = max{dMW; dNW}. A distância média é o average linkage e a das mais próximas é o single linkage.

**Fonte:** Aula de Clustering, pág. 15, pág. 17

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-5
Área 1 · Unsupervised Machine Learning: Clustering II

Assinale a alternativa que contém um elemento pertinente à análise de cluster com o Método Não Hierárquico k-means:

- a) Centroides dos clusters.
- b) Método de encadeamento.
- c) Matrizes de dissimilaridades.
- d) Dendrograma.

**Resposta certa:** a) Centroides dos clusters.

**Explicação:** A resposta é centroides dos clusters. O K-means define K a priori, sorteia os centroides iniciais, aloca cada observação ao centroide mais próximo e recalcula os centroides pela média, repetindo até estabilizar. Método de encadeamento, matriz de dissimilaridades e dendrograma são elementos do método hierárquico.

**Fonte:** Aula de Clustering, pág. 22

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-6
Área 1 · Unsupervised Machine Learning: Clustering II

Assinale a alterativa que apresenta a principal característica do método de encadeamento “average linkage” para a realização de uma clusterização hierárquica aglomerativa:

- a) Utiliza como referência a distância entre as observações mais próximas quando há pelo menos um cluster formado.
- b) Não utiliza medidas de distância entre as observações como referência para o agrupamento.
- c) Utiliza como referência a distância média entre as observações quando há pelo menos um cluster formado.
- d) Utiliza como referência a distância entre as observações mais distantes quando há pelo menos um cluster formado.

**Resposta certa:** c) Utiliza como referência a distância média entre as observações quando há pelo menos um cluster formado.

**Explicação:** A resposta é a distância média entre as observações. No average linkage (between groups) a fusão de dois clusters usa a média das distâncias entre todos os pares de observações dos grupos. O vizinho mais próximo é o single linkage e o mais distante é o complete linkage.

**Fonte:** Aula de Clustering, pág. 15

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-7
Área 1 · Unsupervised Machine Learning: Clustering II

Ao analisar um dendrograma resultante de uma análise de cluster hierárquica aglomerativa, é correto afirmar que:

- a) No último estágio, a figura indicará que cada observação corresponde ao seu próprio cluster isoladamente.
- b) É um método aplicado com o objetivo principal de escolher a medida de dissimilaridade mais apropriada aos dados.
- c) Seu resultado indica exatamente a quantidade de clusters mais apropriada aos dados.
- d) Ao traçar uma linha horizontal no gráfico, o número de vezes que a linha corta o dendrograma indica quantos clusters formam-se naquele nível.

**Resposta certa:** d) Ao traçar uma linha horizontal no gráfico, o número de vezes que a linha corta o dendrograma indica quantos clusters formam-se naquele nível.

**Explicação:** A resposta é que uma linha horizontal traçada no dendrograma indica, pelo número de cortes, quantos clusters existem naquele nível de distância. No último estágio há um cluster só, e o dendrograma não escolhe a quantidade exata nem a medida de dissimilaridade: ele apoia a decisão, em geral olhando os maiores saltos.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 359

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-8
Área 1 · Unsupervised Machine Learning: Clustering II

Em relação à clusterização por meio do método K-means, assinale a alternativa correta que representa seu objetivo ao formar os clusters:

- a) Aumentar as distâncias entre as observações pertencentes ao mesmo cluster.
- b) Diminuir as distâncias entre as observações pertencentes a clusters distintos.
- c) Diminuir as distâncias das observações de um cluster e seu respectivo centroide.
- d) Aumentar as distâncias das observações de um cluster e seu respectivo centroide.

**Resposta certa:** c) Diminuir as distâncias das observações de um cluster e seu respectivo centroide.

**Explicação:** A resposta é diminuir as distâncias entre as observações de um cluster e seu centroide. O K-means realoca as observações ao centroide mais próximo e recalcula os centroides pela média, de modo que cada cluster fique o mais compacto possível, o que equivale a minimizar a soma dos quadrados dentro dos clusters.

**Fonte:** Aula de Clustering, pág. 22

**Situação:** explicação conferida com o material das aulas

---

### Questão 160647-1-9
Área 1 · Unsupervised Machine Learning: Clustering II

Sobre a análise dos “saltos” de distâncias no dendrograma, é correto afirmar que:

- a) Quanto menores os saltos, mais heterogêneas são as observações unidas.
- b) Quanto maiores os saltos, mais homogêneas são as observações unidas.
- c) Grandes saltos unem observações muito distintas.
- d) Pequenos saltos unem observações muito distintas.

**Resposta certa:** c) Grandes saltos unem observações muito distintas.

**Explicação:** A resposta é que grandes saltos de distância unem observações muito distintas. Um salto alto no dendrograma significa que, para fazer aquela união, foi preciso aceitar uma distância grande, então os grupos juntados são heterogêneos. Por isso os saltos servem de critério para decidir onde parar e quantos clusters manter.

**Fonte:** Aula de Clustering, pág. 18

**Situação:** explicação conferida com o material das aulas

---

## Unsupervised Machine Learning: Exercícios Aplicados

### Questão 168185-1-1
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Sobre a Análise de Cluster e a Análise Fatorial PCA, assinale a alternativa CORRETA:

- a) É possível utilizar os valores obtidos pelos fatores como input na Análise de Clusters.
- b) A Análise Fatorial PCA é a técnica mais apropriada para a análise de variáveis qualitativas.
- c) São técnicas adequadas para a previsão de valores para observações de fora da amostra.
- d) A Análise Fatorial PCA depende fundamentalmente da matriz de distâncias Euclidianas.

**Resposta certa:** a) É possível utilizar os valores obtidos pelos fatores como input na Análise de Clusters.

**Explicação:** A resposta é a que permite usar os fatores como input do cluster. A aula mostra que o output de uma técnica não supervisionada pode alimentar outra, e dá como exemplo clusterizar com base nos fatores da análise fatorial. As demais falham: a PCA é para variáveis métricas, não qualitativas, e nenhuma das duas técnicas serve para prever observações fora da amostra.

**Fonte:** Aula de uso conjunto de técnicas não supervisionadas, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-10
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Em relação à Análise de Correspondência e à Análise Fatorial PCA, é CORRETO afirmar que:

- a) Os fatores obtidos na Análise Fatorial PCA podem ser utilizados como input na Análise de Correspondência Simples sem qualquer prévio tratamento.
- b) As coordenadas das observações obtidas a partir da Análise de Correspondência podem ser utilizadas como input na Análise Fatorial PCA.
- c) Não é possível relacionar as técnicas de Análise de Correspondência e Análise Fatorial PCA, pois lidam com tipos de variáveis diferentes.
- d) Os fatores obtidos na Análise Fatorial PCA podem ser utilizados como input na Análise de Correspondência Múltipla sem qualquer prévio tratamento.

**Resposta certa:** b) As coordenadas das observações obtidas a partir da Análise de Correspondência podem ser utilizadas como input na Análise Fatorial PCA.

**Explicação:** A resposta é a que usa as coordenadas da correspondência na PCA. A aula cita as coordenadas das observações do mapa perceptual como input de cluster ou de fatorial, e essas coordenadas são numéricas. Já os fatores da PCA são métricos e não servem direto na correspondência, que pede variáveis categóricas, e as técnicas podem sim ser combinadas.

**Fonte:** Aula de uso conjunto de técnicas não supervisionadas, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-2
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Na Análise de Correspondência Múltipla, uma variável deve ser mantida na análise quando:

- a) Apresentar correlação de Pearson elevada com pelo menos uma outra variável da análise.
- b) Tiver associação significativa com pelo menos uma outra variável da análise.
- c) Tiver mais de duas categorias.
- d) Tiver somente duas categorias.

**Resposta certa:** b) Tiver associação significativa com pelo menos uma outra variável da análise.

**Explicação:** A resposta é manter a variável que tem associação significativa com pelo menos uma outra. Antes da ACM se faz o teste qui-quadrado para cada par de variáveis, e quem não se associa a nenhuma das demais sai da análise. O número de categorias não entra nessa decisão, e correlação de Pearson não se aplica a variáveis categóricas.

**Fonte:** Aula de Análise de Correspondência Múltipla, pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-3
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

São elementos atribuídos à Análise Fatorial por Componentes Principais, EXCETO:

- a) Dendrograma.
- b) Scores fatoriais.
- c) Comunalidades.
- d) Cargas fatoriais.

**Resposta certa:** a) Dendrograma.

**Explicação:** O dendrograma é o gráfico da análise de cluster hierárquica, que mostra como as observações vão sendo unidas. Comunalidades, cargas fatoriais e scores fatoriais são saídas da análise fatorial por componentes principais, que trabalha com a relação entre variáveis para formar fatores.

**Fonte:** Aula de Clustering, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-4
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Sobre a variável que indica a qual cluster pertence cada observação da amostra, assinale a alternativa CORRETA:

- a) É uma variável categórica.
- b) É uma variável contínua.
- c) É uma variável métrica.
- d) É uma variável quantitativa.

**Resposta certa:** a) É uma variável categórica.

**Explicação:** A variável que diz em qual cluster cada observação caiu é categórica: ela só rotula grupos (cluster 1, 2, 3), sem ordem nem distância numérica entre os valores. Por isso as opções métrica, contínua e quantitativa não servem. Isso também explica por que ela pode entrar numa análise de correspondência.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 168185-1-5
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Em relação ao uso conjunto das técnicas não supervisionadas apresentadas nas aulas, assinale a alternativa CORRETA:

- a) A variável indicadora dos cluster obtida na Análise de Cluster pode ser utilizada como input na Análise de Correspondência.
- b) Não existe a possibilidade de uso conjunto das técnicas não supervisionadas, pois são todas independentes umas das outras.
- c) A variável indicadora dos cluster obtida na Análise de Cluster pode ser utilizada como input na Análise Fatorial PCA.
- d) Os fatores resultantes da Análise Fatorial PCA podem ser utilizados como input na Análise de Correspondência Múltipla sem qualquer tratamento prévio.

**Resposta certa:** a) A variável indicadora dos cluster obtida na Análise de Cluster pode ser utilizada como input na Análise de Correspondência.

**Explicação:** A resposta é usar a variável indicadora dos clusters na análise de correspondência. A aula cita justamente o output do cluster como input da correspondência, e o Fávero explica que o cluster vira uma variável qualitativa no banco de dados. Na PCA ela não entra porque exige variáveis métricas, e os fatores não podem ir direto para a ACM sem tratamento.

**Fonte:** Aula de uso conjunto de técnicas não supervisionadas, pág. 8; Manual de Análise de Dados (Fávero), pág. 377

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-6
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Dentre os elementos listados a seguir, assinale a alternativa que contém aqueles que são pertinentes à Análise de Clusters Hierárquica Aglomerativa:

- a) Comunalidades e mapa perceptual.
- b) Resíduos padronizados ajustados e fatores.
- c) Dendrograma e matriz de distâncias.
- d) Teste qui-quadrado e scores fatoriais.

**Resposta certa:** c) Dendrograma e matriz de distâncias.

**Explicação:** Na hierárquica aglomerativa o processo parte de uma matriz de distâncias entre as observações e é acompanhado pelo dendrograma, que mostra os saltos de distância na formação dos clusters. Comunalidades, fatores e scores são da análise fatorial, e qui-quadrado, resíduos e mapa perceptual são da correspondência.

**Fonte:** Aula de Clustering, pág. 18; Manual de Análise de Dados (Fávero), pág. 379

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-7
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Após a realização de uma Análise de Cluster, o teste F para análise de variâncias é utilizado fundamentalmente para:

- a) A criação do dendrograma com a indicação de quantos clusters devem ser formados.
- b) Escolher qual é a medida de dissimilaridade mais indicada para a análise.
- c) Escolher qual é o método de encadeamento mais indicado para a análise.
- d) Analisar quais variáveis contribuíram para a formação de pelo menos um cluster.

**Resposta certa:** d) Analisar quais variáveis contribuíram para a formação de pelo menos um cluster.

**Explicação:** A resposta é analisar quais variáveis contribuíram para formar pelo menos um cluster. O teste F compara a variabilidade entre grupos com a de dentro dos grupos, e as variáveis com maior F (junto com a significância) são as que mais separam os clusters. Ele não define o número de clusters, a medida de dissimilaridade nem o método de encadeamento.

**Fonte:** Aula de Clustering, pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-8
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Marque verdadeiro (V) ou falso (F) nas sentenças a seguir e, posteriormente, assinale a alternativa que contém a sequência CORRETA:

(   ) É possível utilizar o output de uma Análise Fatorial PCA como input na Análise de Cluster. 

(   ) É possível utilizar o output de uma Análise de Cluster como input na Análise de Correspondência Múltipla.

(   ) É possível utilizar a variável que indica a qual cluster pertence cada observação como input na Análise Fatorial por Componentes Principais.
Marque verdadeiro (V) ou falso (F) nas sentenças a seguir e, posteriormente, assinale a alternativa que contém a sequência CORRETA:
(   ) É possível utilizar o output de uma Análise Fatorial PCA como input na Análise de Cluster.
(   ) É possível utilizar o output de uma Análise de Cluster como input na Análise de Correspondência Múltipla.
(   ) É possível utilizar a variável que indica a qual cluster pertence cada observação como input na Análise Fatorial por Componentes Principais.

- a) V, V, F.
- b) F, F, F.
- c) V, V, V.
- d) V, F, V.

**Resposta certa:** a) V, V, F.

**Explicação:** A sequência é V, V, F. Os fatores da PCA podem ser input do cluster, e o output do cluster pode ser input da correspondência, como mostra a aula. A terceira é falsa porque a variável de cluster é qualitativa, e a PCA exige variáveis métricas; a aula pede respeitar o tipo de variável ao combinar as técnicas.

**Fonte:** Aula de uso conjunto de técnicas não supervisionadas, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 168185-1-9
Área 1 · Unsupervised Machine Learning: Exercícios Aplicados

Assinale a alternativa CORRETA em relação à Análise de Correspondência Simples.

- a) O input da Análise de Correspondência é uma matriz de correlações de Pearson.
- b) Tem como objetivo agrupar as variáveis em poucos fatores.
- c) Tem como objetivo verificar a correlação entre variáveis métricas contínuas.
- d) Antes de extrair o mapa perceptual da Análise de Correspondência Simples, é primordial verificar a significância estatística da associação entre as duas variáveis.

**Resposta certa:** d) Antes de extrair o mapa perceptual da Análise de Correspondência Simples, é primordial verificar a significância estatística da associação entre as duas variáveis.

**Explicação:** A resposta é a que exige checar a significância da associação antes do mapa perceptual. A ANACOR tem duas etapas: primeiro o teste qui-quadrado, depois o mapa. O input não é matriz de correlação, o objetivo não é reduzir variáveis a fatores (isso é a PCA) e a técnica é para variáveis categóricas, não métricas.

**Fonte:** Aula de Análise de Correspondência Simples, pág. 9

**Situação:** explicação conferida com o material das aulas

---


# Área 2: Regressão simples e múltipla

## Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

### Questão 169339-1-1
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Os principais critérios para a estimação de modelos de regressão por mínimos quadrados ordinários são:

- a) Somatória dos erros ao quadrado sendo igual a zero e somatória dos erros sendo a mínima possível.
- b) Somatória dos erros sendo igual a zero e somatória dos erros ao quadrado sendo a máxima possível.
- c) Somatória dos erros sendo igual a zero e somatória dos erros ao quadrado sendo igual a zero.
- d) Somatória dos erros sendo igual a zero e somatória dos erros ao quadrado sendo a mínima possível.

**Resposta certa:** d) Somatória dos erros sendo igual a zero e somatória dos erros ao quadrado sendo a mínima possível.

**Explicação:** No MQO os dois critérios são: soma dos erros igual a zero e soma dos erros ao quadrado a menor possível. Mínimo, não máximo, e a soma dos quadrados não é zero, porque isso só aconteceria se todos os pontos estivessem exatamente sobre a reta.

**Fonte:** Aula de Regressão, pág. 23; Manual de Análise de Dados (Fávero), pág. 545

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-10
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Após se estimar um modelo de regressão a partir de determinado dataset (intitulado df), pode ser interessante criar uma coluna na base de dados com os fitted values (variável yhat) do próprio objeto criado, intitulado de modelo. Para se realizar essa tarefa no software Python, podemos utilizar o código:

- a) var fitted_values
- b) df['yhat'] = modelo.fittedvalues
- c) predict yhat
- d) yhat model

**Resposta certa:** b) df['yhat'] = modelo.fittedvalues

**Explicação:** No Python, com um modelo do statsmodels, os valores ajustados ficam no atributo fittedvalues, então df['yhat'] = modelo.fittedvalues cria a coluna. O comando predict yhat é do Stata, e as outras opções não existem como sintaxe de Python.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 169339-1-2
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Assinale a alternativa INCORRETA:

- a) Modelos de regressão são técnicas de machine learning consideradas supervisionadas.
- b) Modelos de regressão são adequados para fins preditivos para outras observações não inicialmente presentes no banco de dados original.
- c) Modelos de regressão são técnicas que têm por finalidade, entre outros objetivos, a estimação de parâmetros para a definição de modelos com capacidade preditiva.
- d) Modelos de regressão têm por finalidade principal a detecção de relações de causa e efeito sobre o fenômeno de estudo.

**Resposta certa:** d) Modelos de regressão têm por finalidade principal a detecção de relações de causa e efeito sobre o fenômeno de estudo.

**Explicação:** A incorreta é a que diz que a finalidade principal é detectar causa e efeito. A regressão avalia como Y se comporta em função de X sem que necessariamente haja relação causal, e serve para estimar parâmetros e prever. As outras três descrevem corretamente um método supervisionado e preditivo.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 543

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-3
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Numa regressão simples, o quadrado do coeficiente de correlação de Pearson é chamado de coeficiente de determinação, coeficiente de explicação, coeficiente de ajuste ou simplesmente ________. É uma medida da proporção da variabilidade em uma variável que é explicada pela variabilidade da outra.

- a) Covariância
- b) R²
- c) Coeficiente angular
- d) Termo de erro

**Resposta certa:** b) R²

**Explicação:** O quadrado do coeficiente de correlação de Pearson na regressão simples é o R², também chamado de coeficiente de ajuste ou de explicação. Ele mede quanto da variação de Y é explicada pela variação de X. Covariância, coeficiente angular e termo de erro são outras coisas.

**Fonte:** Aula de Regressão, pág. 21; Manual de Análise de Dados (Fávero), pág. 553

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-4
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Sobre um modelo de regressão linear simples do tipo:




os termos representam:

[imagem: imagens/169339_1_4_0.png]

- a) Intercepto (α), coeficiente de inclinação da reta (β), variável explicativa Y e termo de erro u.
- b) Intercepto (β), coeficiente de inclinação da reta (α), variável explicativa X e termo de erro u.
- c) Intercepto (β), coeficiente de inclinação da reta (α), variável explicativa Y e termo de erro u.
- d) Intercepto (α), coeficiente de inclinação da reta (β), variável explicativa X e termo de erro u.

**Resposta certa:** d) Intercepto (α), coeficiente de inclinação da reta (β), variável explicativa X e termo de erro u.

**Explicação:** Na equação Yi = alfa + beta.Xi + ui, alfa é o intercepto, beta é a inclinação da reta, X é a variável explicativa e u é o termo de erro. Y é a dependente, então chamar Y de explicativa, ou trocar alfa e beta, está errado.

**Fonte:** Aula de Regressão Linear Simples, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-5
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

A análise de regressão com estimação por mínimos quadrados ordinários pode ser utilizada para vários objetivos, exceto:

- a) Avaliar o retorno estimado de um empreendimento em função do preço de suas unidades imobiliárias autônomas.
- b) Inferir o grau de escolaridade de consumidores (variável outcome qualitativa) em função da renda.
- c) Prever o volume de vendas de um produto em função do índice de confiança do consumidor divulgado em determinado mês.
- d) Estudar o comportamento do preço de uma ação em função do preço de uma commodity ou de outra variável econômica, como PIB ou inflação.

**Resposta certa:** b) Inferir o grau de escolaridade de consumidores (variável outcome qualitativa) em função da renda.

**Explicação:** A exceção é inferir a escolaridade, porque a variável de resultado é qualitativa. O MQO pede variável dependente métrica; para resposta categórica o caminho são modelos logísticos. Retorno de empreendimento, volume de vendas e preço de ação são variáveis quantitativas e cabem numa regressão linear.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 169339-1-6
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Assinale a alternativa CORRETA:

- a) A definição dos parâmetros e do R² são insuficientes para se determinar corretamente um modelo de regressão, já que é preciso que sejam avaliadas as significâncias estatísticas dos parâmetros.
- b) Apenas a definição dos parâmetros já é suficiente para se determinar corretamente um modelo de regressão.
- c) Apenas a definição do R² já é suficiente para se determinar corretamente um modelo de regressão.
- d) Apenas a definição dos parâmetros e do R² já é suficiente para se determinar corretamente a forma funcional de um modelo de regressão.

**Resposta certa:** a) A definição dos parâmetros e do R² são insuficientes para se determinar corretamente um modelo de regressão, já que é preciso que sejam avaliadas as significâncias estatísticas dos parâmetros.

**Explicação:** Só estimar os parâmetros e o R² não basta, pois é preciso ver se cada parâmetro é estatisticamente diferente de zero, com o teste t e o p-valor abaixo de 5%. Um R² alto pode vir junto com parâmetros sem significância, e aí o modelo não está bem especificado.

**Fonte:** Aula de Regressão, pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-7
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

São objetivos de uma regressão linear simples:

I.	A estimação de uma equação linear que apresente a relação entre uma variável dependente e uma explicativa (preditora).

II.	A estimação de uma equação exponencial que apresente a relação entre uma variável qualitativa e uma explicativa.

III.	A estimação de uma equação dentro de um espaço de Hilbert utilizando operadores autoadjuntos ou hermitianos.

IV.	O objetivo principal está na análise da relação entre duas variáveis. Essa análise sempre parte de uma variável chamada de dependente, e outra chamada de preditora (explicativa).

Marque a alternativa CORRETA:
São objetivos de uma regressão linear simples:
I.	A estimação de uma equação linear que apresente a relação entre uma variável dependente e uma explicativa (preditora).
II.	A estimação de uma equação exponencial que apresente a relação entre uma variável qualitativa e uma explicativa.
III.	A estimação de uma equação dentro de um espaço de Hilbert utilizando operadores autoadjuntos ou hermitianos.
IV.	O objetivo principal está na análise da relação entre duas variáveis. Essa análise sempre parte de uma variável chamada de dependente, e outra chamada de preditora (explicativa).

Marque a alternativa CORRETA:

- a) Todas as afirmações estão corretas.
- b) Apenas I e IV estão corretas.
- c) Apenas I, II e IV estão corretas.
- d) Apenas II e IV estão corretas.

**Resposta certa:** b) Apenas I e IV estão corretas.

**Explicação:** Só I e IV estão certas. O objetivo da regressão linear simples é uma equação linear entre uma dependente e uma explicativa. A II erra porque a dependente na regressão linear é métrica e a equação é linear. A III cita espaço de Hilbert e operadores hermitianos, que não têm relação com o tema.

**Fonte:** Aula de Regressão Linear Simples, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-8
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Sobre um modelo de regressão linear simples (como o apresentado a seguir), marque a alternativa CORRETA:
Sobre um modelo de regressão linear simples (como o apresentado a seguir), marque a alternativa CORRETA:

[imagem: imagens/169339_1_8_0.png]

- a) O termo de erro ui para cada observação i tem o valor igual a zero, necessariamente.
- b) O termo de erro ui não representa o efeito de outras variáveis não incluídas na equação.
- c) O termo de erro ui captura parte do comportamento da variável dependente Y que não foi devidamente explicada pela variável X, ou seja, faz as vezes de uma ou mais variáveis potencialmente preditoras de Y que foram omitidas no modelo.
- d) O termo de erro ui não tem qualquer função na equação.

**Resposta certa:** c) O termo de erro ui captura parte do comportamento da variável dependente Y que não foi devidamente explicada pela variável X, ou seja, faz as vezes de uma ou mais variáveis potencialmente preditoras de Y que foram omitidas no modelo.

**Explicação:** O termo de erro u é a diferença entre o valor real de Y e o previsto pelo modelo, e absorve o que X não explica, inclusive o efeito de variáveis omitidas. Não é zero para cada observação (só a soma dos erros é zero no MQO) e tem função na equação.

**Fonte:** Aula de Regressão Linear Simples, pág. 18; Manual de Análise de Dados (Fávero), pág. 542

**Situação:** explicação conferida com o material das aulas

---

### Questão 169339-1-9
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla I

Sobre o estudo dos modelos de regressão simples e múltipla, podemos afirmar o seguinte:

I.	A análise da regressão estuda a relação entre uma variável chamada de variável dependente e outras variáveis chamadas de variáveis preditoras.

II.	A relação entre suas variáveis é representada por uma equação matemática, que relaciona a variável dependente com as variáveis preditoras.

III.	A expressão designada por "modelo de regressão linear simples" é aquela em que se define uma relação linear entre a variável dependente e uma variável preditora.

IV.	Uma aplicação muito importante de um modelo de regressão é a previsão de novas ou futuras observações de Y, correspondente a um dado valor da variável explicativa X.

Escolha a alternativa CORRETA:
Sobre o estudo dos modelos de regressão simples e múltipla, podemos afirmar o seguinte:
I.	A análise da regressão estuda a relação entre uma variável chamada de variável dependente e outras variáveis chamadas de variáveis preditoras.
II.	A relação entre suas variáveis é representada por uma equação matemática, que relaciona a variável dependente com as variáveis preditoras.
III.	A expressão designada por "modelo de regressão linear simples" é aquela em que se define uma relação linear entre a variável dependente e uma variável preditora.
IV.	Uma aplicação muito importante de um modelo de regressão é a previsão de novas ou futuras observações de Y, correspondente a um dado valor da variável explicativa X.

Escolha a alternativa CORRETA:

- a) Apenas I e II estão corretas.
- b) Apenas II e IV estão corretas.
- c) Todas as afirmações estão corretas.
- d) Apenas I, II e IV estão corretas.

**Resposta certa:** c) Todas as afirmações estão corretas.

**Explicação:** Todas estão corretas. A regressão relaciona uma dependente a uma ou mais preditoras, por meio de uma equação. A regressão simples é a de uma única preditora com relação linear, e uma aplicação importante é prever Y para novos valores de X.

**Fonte:** Aula de Regressão Linear Simples, pág. 18; Aula de Regressão Múltipla, pág. 31

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

### Questão 170407-1-1
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Sobre o teste F, é CORRETO afirmar que:

- a) Avalia a significância estatística conjunta dos parâmetros.
- b) Avalia apenas a significância estatística do parâmetro correspondente ao intercepto (alpha).
- c) Avalia a significância estatística individual de cada parâmetro do modelo.
- d) Não deve ser analisado em modelos regressivos estimados por OLS.

**Resposta certa:** a) Avalia a significância estatística conjunta dos parâmetros.

**Explicação:** O teste F avalia a significância conjunta dos parâmetros. A hipótese nula é que todos os betas sejam zero, e rejeitá-la indica que pelo menos um beta é diferente de zero. A significância individual de cada parâmetro é papel do teste t.

**Fonte:** Aula de Regressão, pág. 29

**Situação:** explicação conferida com o material das aulas

---

### Questão 170407-1-10
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Muitas são as formas de replicação (multiplicação da quantidade de observações para as mesmas variáveis) de uma base de dados no Python. Em aula, vimos a função:

- a) 'mice' do 'statsmodels'.
- b) 'multiplicate' do 'pandas'.
- c) 'slice' do 'seaborn'.
- d) 'repeat' do 'numpy'.

**Resposta certa:** d) 'repeat' do 'numpy'.

**Explicação:** Para replicar as linhas de uma base no Python, a função vista foi a repeat do numpy, que repete os elementos de um array um número de vezes. As outras opções (mice, multiplicate, slice) não fazem essa tarefa nos pacotes citados.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 170407-1-2
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Avalie as afirmações a seguir e assinale a alternativa CORRETA:

I) Os modelos de regressão inserem-se naquilo que é conhecido por GLM (Generalized Linear Models).

II) A estimação OLS é adequada para todo tipo de modelo de regressão, mesmo quando a variável dependente for qualitativa.

III) Muitas são as classes de estimações que se inserem nos modelos GLM, tais como os modelos de regressão simples e múltipla, os modelos logísticos binários e multinomiais e os modelos para dados de contagem.
Avalie as afirmações a seguir e assinale a alternativa CORRETA:

I) Os modelos de regressão inserem-se naquilo que é conhecido por GLM (Generalized Linear Models).
II) A estimação OLS é adequada para todo tipo de modelo de regressão, mesmo quando a variável dependente for qualitativa.
III) Muitas são as classes de estimações que se inserem nos modelos GLM, tais como os modelos de regressão simples e múltipla, os modelos logísticos binários e multinomiais e os modelos para dados de contagem.

- a) Apenas II e III estão corretas.
- b) Apenas I e III estão corretas.
- c) Apenas I e II estão corretas.
- d) Apenas I está correta.

**Resposta certa:** b) Apenas I e III estão corretas.

**Explicação:** Estão corretas I e III. A regressão simples e múltipla, a logística e os modelos de contagem fazem parte dos GLM. A II é falsa porque o OLS pede variável dependente métrica; para dependente qualitativa usam-se outros modelos GLM, como o logístico.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 536

**Situação:** explicação conferida com o material das aulas

---

### Questão 170407-1-3
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Após a estimação de um modelo a partir da função ‘OLS.from_formula’ do pacote ‘statsmodels’ no Python, obteve-se o seguinte output, conforme imagem a seguir.

A partir do output do modelo na imagem, avalie as três afirmações abaixo e assinale a alternativa CORRETA. 

I. Os valores estimados dos coeficientes do modelo de regressão são alpha = 11,9719; beta1 (idade) = 0,0997; beta2 (horas) = -0,4013.

II. Este modelo permite a elaboração de previsões da variável cpi, desde que os valores inseridos em idade e horas estejam dentro do range, ou amplitude, dessas variáveis em nosso banco de dados.

III. Os parâmetros das variáveis preditoras idade e horas são estatisticamente significantes ao nível de confiança de 95% (nível de significância de 5%).
Após a estimação de um modelo a partir da função ‘OLS.from_formula’ do pacote ‘statsmodels’ no Python, obteve-se o seguinte output, conforme imagem a seguir.

A partir do output do modelo na imagem, avalie as três afirmações abaixo e assinale a alternativa CORRETA. 

I. Os valores estimados dos coeficientes do modelo de regressão são alpha = 11,9719; beta1 (idade) = 0,0997; beta2 (horas) = -0,4013.
II. Este modelo permite a elaboração de previsões da variável cpi, desde que os valores inseridos em idade e horas estejam dentro do range, ou amplitude, dessas variáveis em nosso banco de dados.
III. Os parâmetros das variáveis preditoras idade e horas são estatisticamente significantes ao nível de confiança de 95% (nível de significância de 5%).

[imagem: imagens/170407_1_3_0.jpg]

- a) Somente I está correta.
- b) Somente I e III estão corretas.
- c) Somente II e III estão corretas.
- d) Todas as afirmações estão corretas.

**Resposta certa:** d) Todas as afirmações estão corretas.

**Explicação:** I: o output traz Intercept 11,9719, idade 0,0997 e horas -0,4013, exatamente como no enunciado. II: previsão só vale dentro da amplitude observada, o que é a regra. III: os p-valores são 0,004 para idade e 0,005 para horas, ambos abaixo de 0,05 (e os intervalos de 95% não contêm o zero), então são significantes. As três estão corretas.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 170407-1-4
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Após a estimação de um modelo a partir da função ‘OLS.from_formula’ do pacote ‘statsmodels’ no Python, obteve-se o seguinte output, conforme imagem a seguir.

Pergunta-se: Qual o valor previsto de cpi, em média, para uma observação com idade = 40 e horas = 30?

[imagem: imagens/170407_1_4_0.jpg]

- a) 3,92.
- b) 7,47.
- c) 2,40.
- d) 5,39.

**Resposta certa:** a) 3,92.

**Explicação:** Usando os coeficientes do enunciado da questão anterior do mesmo output, o valor previsto é 11,9719 + 0,0997 x 40 - 0,4013 x 30 = 11,9719 + 3,988 - 12,039 = 3,92. As outras opções vêm de trocar sinais ou esquecer um termo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 170407-1-5
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Sobre os testes t de significância de parâmetros em modelos de regressão, é CORRETO afirmar que:

- a) Todas as alternativas anteriores estão corretas.
- b) Analisam conjuntamente os parâmetros, identificando se o modelo é relevante.
- c) Analisam individualmente cada um dos parâmetros, identificando se eles são estatisticamente significantes.
- d) Analisam apenas a significância do parâmetro correspondente ao intercepto (alpha).

**Resposta certa:** c) Analisam individualmente cada um dos parâmetros, identificando se eles são estatisticamente significantes.

**Explicação:** Os testes t analisam individualmente cada parâmetro, vendo se ele é estatisticamente diferente de zero. A análise conjunta é do teste F, e o t não se limita ao intercepto. Como só uma alternativa é a correta, a de 'todas as anteriores' fica descartada.

**Fonte:** Aula de Regressão, pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 170407-1-6
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

O gráfico a seguir foi gerado após a estimação de um modelo de regressão linear simples. A partir da análise do gráfico, assinale a alternativa CORRETA.

[imagem: imagens/170407_1_6_0.jpg]

- a) Para o nível de confiança adotado, os parâmetros alpha e beta são estatisticamente significantes.
- b) Para o nível de confiança adotado, os parâmetros alpha e beta não são estatisticamente significantes.
- c) Para o nível de confiança adotado, apenas o parâmetro alpha é estatisticamente significante.
- d) Para o nível de confiança adotado, apenas o parâmetro beta é estatisticamente significante.

**Resposta certa:** b) Para o nível de confiança adotado, os parâmetros alpha e beta não são estatisticamente significantes.

**Explicação:** O gráfico mostra a faixa de confiança em cinza em torno da reta ajustada. Em x próximo de 5 a faixa vai de cerca de -22 a 47, então inclui o zero e o alpha não é significante. Além disso, uma reta horizontal cabe dentro da faixa em todo o intervalo, ou seja, beta igual a zero não é rejeitado e o beta também não é significante.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 170407-1-7
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Após a estimação de um modelo a partir da função ‘OLS.from_formula’ do pacote ‘statsmodels’ no Python, obteve-se o seguinte output, conforme imagem a seguir.

Pergunta-se: qual é o percentual de variância da variável Y (cpi) que é capturado pelo comportamento de variação das variáveis preditoras X (idade e horas)?

[imagem: imagens/170407_1_7_0.jpg]

- a) 29,50%.
- b) 32,40%.
- c) 11,26%.
- d) 11,97%.

**Resposta certa:** b) 32,40%.

**Explicação:** A parcela da variância de Y explicada pelas preditoras é o R-squared do output, 0,324, ou 32,4%. O Adj. R-squared é 0,295 (29,5%), que penaliza o número de variáveis e não é o que a pergunta quer. Os valores 11,26 e 11,97 são a estatística F e o intercepto, sem relação com variância explicada.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 170407-1-8
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla II

Sejam as seguintes afirmações:

I) As bandas dos intervalos de confiança de parâmetros beta em modelos regressivos aumentam quando se aumenta o nível de confiança.

II) Determinado parâmetro beta pode se tornar estatisticamente não significante ao aumentarmos o nível de confiança para fins preditivos.

III) Amostras reduzidas podem fazer com que o parâmetro de intercepto alpha não se apresente estatisticamente significante em modelos regressivos.

Assinale a alternativa CORRETA:
Sejam as seguintes afirmações:
I) As bandas dos intervalos de confiança de parâmetros beta em modelos regressivos aumentam quando se aumenta o nível de confiança.
II) Determinado parâmetro beta pode se tornar estatisticamente não significante ao aumentarmos o nível de confiança para fins preditivos.
III) Amostras reduzidas podem fazer com que o parâmetro de intercepto alpha não se apresente estatisticamente significante em modelos regressivos.

Assinale a alternativa CORRETA:

- a) Apenas I está correta.
- b) Apenas II e III estão corretas.
- c) Apenas I e II estão corretas.
- d) Todas estão corretas.

**Resposta certa:** d) Todas estão corretas.

**Explicação:** As três estão certas. Quanto maior o nível de confiança, mais largo o intervalo; um intervalo mais largo pode passar a conter o zero, e aí o beta deixa de ser significante. E com amostra pequena o erro-padrão cresce, o que pode deixar até o intercepto sem significância.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 564; Aula de Regressão, pág. 30

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

### Questão 171716-1-1
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Sobre o procedimento Stepwise:

I.	Este procedimento tem a propriedade de, automaticamente, excluir ou manter os betas do modelo em função da significância estatística definida.

II.	É possível aplicar o procedimento Stepwise para que sejam eliminadas as variáveis cujos parâmetros não se mostrarem estatisticamente significantes na presença de outras variáveis.

III.	O procedimento Stepwise para a seleção de variáveis não pode ser utilizado em modelos de regressão.

Assinale a alternativa CORRETA:
Sobre o procedimento Stepwise:
I.	Este procedimento tem a propriedade de, automaticamente, excluir ou manter os betas do modelo em função da significância estatística definida.
II.	É possível aplicar o procedimento Stepwise para que sejam eliminadas as variáveis cujos parâmetros não se mostrarem estatisticamente significantes na presença de outras variáveis.
III.	O procedimento Stepwise para a seleção de variáveis não pode ser utilizado em modelos de regressão.

Assinale a alternativa CORRETA:

- a) Somente I e III estão corretas.
- b) Somente I e II estão corretas.
- c) Somente II e III estão corretas.
- d) Todas as afirmações estão corretas.

**Resposta certa:** b) Somente I e II estão corretas.

**Explicação:** Estão corretas I e II. O Stepwise exclui automaticamente as variáveis cujos parâmetros não são significantes na presença das demais, e é usado em modelos de regressão. Por isso a III é falsa, já que ele existe justamente para selecionar variáveis em regressões.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 577

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-10
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Sobre modelos de regressão:

I. Quando uma variável X apresentar uma correlação baixa e não estatisticamente significante com uma variável Y, necessariamente ela deverá estar presente no modelo final preditivo.

II. Todas as variáveis preditoras qualitativas de um modelo de regressão necessariamente devem apresentar parâmetros estatisticamente significantes.

III. Quando uma das variáveis preditoras não estiver presente no modelo final múltiplo, necessariamente esta variável não apresenta relação significante individual com a variável Y.

Assinale a alternativa CORRETA:
Sobre modelos de regressão:
I. Quando uma variável X apresentar uma correlação baixa e não estatisticamente significante com uma variável Y, necessariamente ela deverá estar presente no modelo final preditivo.
II. Todas as variáveis preditoras qualitativas de um modelo de regressão necessariamente devem apresentar parâmetros estatisticamente significantes.
III. Quando uma das variáveis preditoras não estiver presente no modelo final múltiplo, necessariamente esta variável não apresenta relação significante individual com a variável Y.

Assinale a alternativa CORRETA:

- a) Somente II e III são verdadeiras.
- b) Somente I é verdadeira.
- c) Todas as afirmações são falsas.
- d) Todas as afirmações são verdadeiras.

**Resposta certa:** c) Todas as afirmações são falsas.

**Explicação:** Todas são falsas. Uma variável pode ser relevante só na presença de outras, então baixa correlação simples não obriga nem proíbe a inclusão. Dummies não precisam ser todas significantes, e uma variável pode sair do modelo múltiplo por multicolinearidade mesmo tendo relação individual com Y.

**Fonte:** Aula de Multicolinearidade, pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-2
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Dois modelos de regressão foram estimados, sem e com transformação de Box-Cox, respectivamente. A figura a seguir apresenta os outputs dos modelos, com respectivos testes de Shapiro-Francia dos resíduos.

Pergunta-se: qual a equação do modelo preditivo mais adequado neste caso?
Dois modelos de regressão foram estimados, sem e com transformação de Box-Cox, respectivamente. A figura a seguir apresenta os outputs dos modelos, com respectivos testes de Shapiro-Francia dos resíduos.
Pergunta-se: qual a equação do modelo preditivo mais adequado neste caso?

[imagem: imagens/171716_1_2_0.jpg]

- a) d)
- b) b)
- c) a)
- d) c)

**Resposta certa:** d) c)

**Explicação:** O modelo sem Box-Cox tem Shapiro-Francia com p-valor 0,000143, então rejeita a normalidade dos resíduos. O modelo com Box-Cox (lambda 2,659) tem p-valor 0,1026, não rejeita H0 e também tem R² maior (0,96 contra 0,903). Logo vale a equação do Box-Cox, (comprimento^2,659 - 1)/2,659 = 4.995,16 + 947,23·idade, que é a alternativa c).

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-3
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Dois modelos de regressão foram estimados, sem e com transformação de Box-Cox, respectivamente. A figura a seguir apresenta os outputs dos modelos, com respectivos testes de Shapiro-Francia dos resíduos.

Pergunta-se: para o modelo mais adequado para fins preditivos, qual a estimativa aproximada da variável comprimento para uma idade de 40 semanas?

[imagem: imagens/171716_1_3_0.jpg]

- a) 20,4 cm.
- b) 79,8 cm.
- c) 40,7 cm.
- d) 60,1 cm.

**Resposta certa:** b) 79,8 cm.

**Explicação:** No modelo Box-Cox, (comprimento^2,659 - 1)/2,659 = 4.995,16 + 947,23 x 40 = 42.884,35. Multiplicando por 2,659 e somando 1 dá cerca de 114.032, e elevando a 1/2,659 chega-se a aproximadamente 79,8 cm. Sem desfazer a transformação o valor ficaria absurdo.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-4
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Estimou-se um modelo de regressão por OLS com transformação de Box-Cox, e os outputs obtidos encontram-se na figura abaixo.

Pergunta-se: qual a equação do modelo preditivo neste caso?

[imagem: imagens/171716_1_4_0.jpg]

- a) a)
- b) c)
- c) b)
- d) d)

**Resposta certa:** a) a)

**Explicação:** A figura mostra lambda de Box-Cox igual a 2,659, intercepto 4.995,16 e coeficiente de idade 947,23. A equação então é (comprimento^2,659 - 1)/2,659 = 4.995,16 + 947,23·idade, que é a alternativa a). A b) usa lambda 0,962, que não aparece na figura, e a c) troca intercepto e coeficiente.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-5
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

No Python, para se criarem n - 1 variáveis dummy a partir de uma variável original qualitativa, devemos utilizar a função:

- a) get_dummies do pacote pandas
- b) dummy_var do pacote numpy
- c) dummy_var_n_1 do pacote statsmodels
- d) gdummies do pacote seaborn

**Resposta certa:** a) get_dummies do pacote pandas

**Explicação:** A função que cria dummies no Python é o get_dummies do pandas. Para ficar com n - 1 colunas, usa-se o argumento drop_first=True, já que uma categoria vira a referência. As outras opções citadas não existem nesses pacotes.

**Fonte:** Aula de Variáveis dummy, pág. 35

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 171716-1-6
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Foi elaborado um teste de Shapiro-Francia à distribuição dos resíduos de um modelo de regressão estimado por OLS. O resultado do teste é apresentado na imagem abaixo.

A partir do resultado do teste, é possível afirmar que:

[imagem: imagens/171716_1_6_0.jpg]

- a) A distribuição dos resíduos é aderente à distribuição normal.
- b) O resultado é inconclusivo, já que o teste de Shapiro-Francia não serve para se avaliar aderência à normalidade.
- c) A distribuição dos resíduos é aderente à distribuição t-Student.
- d) A distribuição dos resíduos não é aderente à distribuição normal.

**Resposta certa:** d) A distribuição dos resíduos não é aderente à distribuição normal.

**Explicação:** O teste traz W = 0,9087, z = 3,6277 e p-valor = 0,000143. Como o p-valor está muito abaixo de 0,05, rejeita-se H0 (normalidade). Os resíduos, portanto, não são aderentes à distribuição normal, e o Shapiro-Francia serve sim para essa avaliação.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-8
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

No caso de ser necessário acrescentar em uma regressão uma variável categórica com mais de uma categoria, como devemos proceder?

- a) Neste caso, devemos incluir n + 1 dummies, em que n é a quantidade de categorias existentes na variável original.
- b) Não será possível fazer esta regressão.
- c) Neste caso, devemos incluir n dummies, em que n é a quantidade de categorias existentes na variável original.
- d) Neste caso, devemos incluir n - 1 dummies, em que n é a quantidade de categorias existentes na variável original.

**Resposta certa:** d) Neste caso, devemos incluir n - 1 dummies, em que n é a quantidade de categorias existentes na variável original.

**Explicação:** Para uma variável qualitativa com n categorias, incluem-se n - 1 dummies, e a categoria que fica de fora é a de referência. Incluir n dummies junto com o intercepto causaria multicolinearidade perfeita, e n + 1 nem faz sentido.

**Fonte:** Aula de Variáveis dummy, pág. 35

**Situação:** explicação conferida com o material das aulas

---

### Questão 171716-1-9
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla III

Sejam as seguintes afirmações:

I.	Quando à distribuição dos resíduos não se mostrar aderente à normalidade, procedimentos de normalização da variável dependente (ex.: Box-Cox) podem ser úteis para que a distribuição dos resíduos do modelo estimado se torne aderente à normalidade.

II.	A aderência da distribuição dos resíduos à normalidade pode ser identificada por meio do teste de Shapiro-Francia.

III.	Comportamentos não lineares de determinados fenômenos não podem ser identificados por meio de modelos de regressão, já que não geram coeficientes de determinação R².

Assinale a alternativa CORRETA:
Sejam as seguintes afirmações:
I.	Quando à distribuição dos resíduos não se mostrar aderente à normalidade, procedimentos de normalização da variável dependente (ex.: Box-Cox) podem ser úteis para que a distribuição dos resíduos do modelo estimado se torne aderente à normalidade.
II.	A aderência da distribuição dos resíduos à normalidade pode ser identificada por meio do teste de Shapiro-Francia.
III.	Comportamentos não lineares de determinados fenômenos não podem ser identificados por meio de modelos de regressão, já que não geram coeficientes de determinação R².

Assinale a alternativa CORRETA:

- a) Apenas I está correta.
- b) Apenas II e III estão corretas.
- c) Apenas I e II estão corretas.
- d) Todas as afirmações estão corretas.

**Resposta certa:** c) Apenas I e II estão corretas.

**Explicação:** Estão corretas I e II. O Box-Cox serve para aproximar a variável dependente da normalidade e, com isso, os resíduos, e o Shapiro-Francia avalia essa aderência. A III é falsa, pois modelos não lineares (inclusive com Box-Cox) também geram R².

**Fonte:** Aula de Box-Cox, pág. 38; Manual de Análise de Dados (Fávero), pág. 613

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

### Questão 172684-1-1
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Em relação à multicolinearidade, pode-se afirmar que:

- a) É um fenômeno que aparece em modelos regressivos apenas após a elaboração do teste de Shapiro-Francia.
- b) É a consequência da existência de correlação alta entre duas ou mais variáveis explicativas.
- c) É um fenômeno decorrente da correlação significante entre a variável dependente e os termos de erro.
- d) É um fenômeno decorrente da correlação significante entre termos de erro com defasagens temporais.

**Resposta certa:** b) É a consequência da existência de correlação alta entre duas ou mais variáveis explicativas.

**Explicação:** A multicolinearidade é a consequência de correlação alta entre duas ou mais variáveis explicativas. Não surge do teste de Shapiro-Francia e não tem a ver com correlação entre Y e erros ou entre erros defasados, que são outros problemas (endogeneidade e autocorrelação).

**Fonte:** Aula de Multicolinearidade, pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-10
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Podem ser fatores geradores da multicolinearidade:

I) Existência de variáveis que apresentam a mesma tendência durante alguns períodos, em decorrência da seleção de uma amostra que inclua apenas observações referentes a estes períodos.

II) Utilização de amostras com reduzido número de observações.

III) Utilização de valores defasados em algumas das variáveis explicativas como “novas” explicativas.

Assinale a alternativa CORRETA:
Podem ser fatores geradores da multicolinearidade:

I) Existência de variáveis que apresentam a mesma tendência durante alguns períodos, em decorrência da seleção de uma amostra que inclua apenas observações referentes a estes períodos.
II) Utilização de amostras com reduzido número de observações.
III) Utilização de valores defasados em algumas das variáveis explicativas como “novas” explicativas.

Assinale a alternativa CORRETA:

- a) Apenas I e II estão corretas.
- b) Apenas I e III estão corretas.
- c) Todas as afirmações estão corretas.
- d) Apenas II e III estão corretas.

**Resposta certa:** c) Todas as afirmações estão corretas.

**Explicação:** A resposta é que as três afirmações são fontes de multicolinearidade. Variáveis com a mesma tendência em certos períodos, amostras pequenas e o uso de valores defasados como novas explicativas aumentam a correlação entre as preditoras. É exatamente a lista de fontes geradoras apresentada em aula.

**Fonte:** Aula de Diagnóstico de multicolinearidade, pág. 43

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-2
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Sobre a estatística VIF, é CORRETO dizer que:

- a) Só são aceitos modelos de regressão múltipla com valores de VIF maiores que 100.000 para todas as variáveis preditoras.
- b) É algebricamente o inverso do R² obtido ao se estimar um modelo de regressão com determinada variável Y como dependente das demais variáveis preditoras.
- c) É algebricamente o inverso de (1 – R²), em que o R² é obtido ao se estimar um modelo de regressão com determinada variável Y como dependente dos termos de erro.
- d) É algebricamente o inverso de (1 – R²), em que o R² é obtido ao se estimar um modelo de regressão com determinada variável X como dependente das demais variáveis preditoras.

**Resposta certa:** d) É algebricamente o inverso de (1 – R²), em que o R² é obtido ao se estimar um modelo de regressão com determinada variável X como dependente das demais variáveis preditoras.

**Explicação:** O VIF é 1/Tolerance, e Tolerance = 1 - R², em que o R² vem da regressão auxiliar de uma variável X contra as demais explicativas. Então VIF = 1/(1 - R²). Não é o inverso do R² puro, não usa Y nem o termo de erro, e não existe regra de VIF acima de 100.000.

**Fonte:** Aula de Multicolinearidade, pág. 47; Manual de Análise de Dados (Fávero), pág. 585

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-3
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

A transformação de Box-Cox sobre a variável dependente:

I) Torna a especificação do modelo não linear (quando l ≠ 1).

II) Pode fazer com que os termos de erro do novo modelo estimado apresentem distribuição aderente à distribuição normal, fazendo com que se tornem adequados os intervalos de confiança dos parâmetros para fins preditivos.

III) Pode fazer com que se reduza a heterocedasticidade pela consideração de um ajuste não linear nos dados.

Assinale a alternativa CORRETA:
A transformação de Box-Cox sobre a variável dependente:
I) Torna a especificação do modelo não linear (quando l ≠ 1).
II) Pode fazer com que os termos de erro do novo modelo estimado apresentem distribuição aderente à distribuição normal, fazendo com que se tornem adequados os intervalos de confiança dos parâmetros para fins preditivos.
III) Pode fazer com que se reduza a heterocedasticidade pela consideração de um ajuste não linear nos dados.

Assinale a alternativa CORRETA:

- a) Apenas I e II estão corretas.
- b) Todas as afirmações estão corretas.
- c) Apenas II e III estão corretas.
- d) Apenas I e III estão corretas.

**Resposta certa:** b) Todas as afirmações estão corretas.

**Explicação:** A resposta é que as três afirmações estão certas. Com lambda diferente de 1 a relação entre Y e os X deixa de ser linear. O lambda é escolhido para aproximar a nova variável da normalidade, o que tende a normalizar os resíduos e deixar os intervalos de confiança mais adequados para previsão. Além disso, o ajuste não linear pode reduzir a heterocedasticidade.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 578; Aula de Modelos não lineares e Box-Cox, pág. 38

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-4
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Considere o grafo abaixo com as correlações de Pearson entre cada par de variáveis (Y, X1 e X2), sendo Y a variável dependente e X1 e X2 as variáveis preditoras de determinado modelo de regressão linear múltipla. Por meio da análise visual do grafo abaixo, é possível afirmar que:

[imagem: imagens/172684_1_4_0.jpg]

- a) Os problemas de multicolinearidade existentes no modelo estimado são decorrentes da baixa correlação entre as variáveis Y e X2.
- b) Com certeza não há problemas de multicolinearidade no modelo estimado.
- c) Há indícios de existência de fortes problemas de multicolinearidade no modelo estimado em razão da alta correlação entre as variáveis X1 e X2.
- d) Os problemas de multicolinearidade existentes no modelo estimado são decorrentes da alta correlação entre as variáveis Y e X1.

**Resposta certa:** c) Há indícios de existência de fortes problemas de multicolinearidade no modelo estimado em razão da alta correlação entre as variáveis X1 e X2.

**Explicação:** A resposta é a que fala em indícios de multicolinearidade pela alta correlação entre X1 e X2. Multicolinearidade é um problema entre as variáveis preditoras, então o que importa é a correlação X1 com X2. A correlação de cada X com Y é desejável, porque mostra que ele ajuda a explicar a dependente, e não causa o problema.

**Fonte:** Aula de Diagnóstico de multicolinearidade, pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-5
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Considere o fenômeno da heterocedasticidade, avalie as afirmações abaixo e assinale a alternativa CORRETA.

I) A heterocedasticidade é decorrente da omissão de variáveis preditoras significantes no modelo final estimado.

II) A heterocedasticidade pode ser reduzida por meio da inclusão de variáveis preditoras de Y cujos parâmetros b se mostrarem estatisticamente significantes após o procedimento Stepwise.

III) Termos de erro serão heterocedásticos quando estiverem fazendo as vezes de variáveis preditoras significantes que foram omitidas no modelo final estimado.
Considere o fenômeno da heterocedasticidade, avalie as afirmações abaixo e assinale a alternativa CORRETA.
I) A heterocedasticidade é decorrente da omissão de variáveis preditoras significantes no modelo final estimado.
II) A heterocedasticidade pode ser reduzida por meio da inclusão de variáveis preditoras de Y cujos parâmetros b se mostrarem estatisticamente significantes após o procedimento Stepwise.
III) Termos de erro serão heterocedásticos quando estiverem fazendo as vezes de variáveis preditoras significantes que foram omitidas no modelo final estimado.

- a) Apenas II e III estão corretas.
- b) Todas as afirmações estão corretas.
- c) Apenas I e III estão corretas.
- d) Apenas I e II estão corretas.

**Resposta certa:** b) Todas as afirmações estão corretas.

**Explicação:** A resposta é que todas as afirmações estão corretas. A heterocedasticidade aparece quando o termo de erro absorve o efeito de preditoras significantes que ficaram de fora do modelo. Por isso incluir essas variáveis, selecionadas pelo Stepwise, pode reduzi-la. No exemplo do livro, o modelo completo tinha heterocedasticidade e o modelo final do Stepwise não.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 604

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-6
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Considere o grafo abaixo com as correlações de Pearson entre cada par de variáveis (Y, X1 e X2), sendo Y a variável dependente e X1 e X2 as variáveis preditoras de determinado modelo de regressão linear múltipla. Por meio da análise visual do grafo abaixo, é possível afirmar que:

[imagem: imagens/172684_1_6_0.jpg]

- a) Os fortes problemas de multicolinearidade existentes no modelo estimado são decorrentes da baixa correlação entre as variáveis X1, X2 e termos de erro.
- b) Há indícios de existência de fortes problemas de multicolinearidade no modelo estimado.
- c) Os fortes problemas de multicolinearidade existentes no modelo estimado são decorrentes da alta correlação entre as variáveis Y e X2.
- d) Não há indícios de problemas de multicolinearidade no modelo estimado.

**Resposta certa:** d) Não há indícios de problemas de multicolinearidade no modelo estimado.

**Explicação:** No grafo, X1 e Y têm correlação forte, perto de 0,9 (traço roxo grosso), enquanto X1-X2 e X2-Y ficam em torno de -0,2 a -0,3 (amarelo). Multicolinearidade se avalia entre as preditoras, e X1 com X2 tem correlação fraca. Alta correlação de X1 com Y é desejável e não indica problema.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-7
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Considere os conceitos apresentados em aula e assinale a alternativa CORRETA sobre a multicolinearidade:

- a) Pode gerar interpretações erradas do modelo pela eventual distorção dos sinais dos parâmetros.
- b) Não gera erros de predições.
- c) Não gera sinais inesperados dos parâmetros estimados.
- d) Não existe este fenômeno em modelos supervisionados de machine learning.

**Resposta certa:** a) Pode gerar interpretações erradas do modelo pela eventual distorção dos sinais dos parâmetros.

**Explicação:** A resposta é que a multicolinearidade pode gerar interpretações erradas por distorcer os sinais dos parâmetros. Ela vem da alta correlação entre preditoras e também prejudica as predições, o que derruba a segunda alternativa. Sinais inesperados dos coeficientes são justamente um dos sintomas para detectá-la, e ela existe sim em modelos supervisionados.

**Fonte:** Aula de Diagnóstico de multicolinearidade, pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-8
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

O diagnóstico de heterocedasticidade em modelos regressivos pode ser realizado por meio do teste de:

- a) Galton-Pearson-Snedecor-Gosset.
- b) Box-Cox.
- c) Breusch-Pagan.
- d) Shapiro-Francia.

**Resposta certa:** c) Breusch-Pagan.

**Explicação:** A resposta é Breusch-Pagan. O teste de Breusch-Pagan/Cook-Weisberg tem como hipótese nula a variância constante dos erros, e rejeitá-la indica heterocedasticidade. Shapiro-Francia testa a normalidade dos resíduos e Box-Cox é uma transformação da variável dependente, nenhum dos dois detecta heterocedasticidade.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 588

**Situação:** explicação conferida com o material das aulas

---

### Questão 172684-1-9
Área 2 · Supervised Machine Learning: Análise de Regressão Simples e Múltipla IV

Assinale a alternativa que apresenta o gráfico com o maior indício de existência de heterocedasticidade quando da estimação de um modelo de regressão que considera as variáveis Y (dependente) e X (preditora).

[imagem: imagens/172684_1_9_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** d) d)

**Explicação:** Heterocedasticidade é variância dos erros que muda ao longo de X. No gráfico d) os pontos formam um funil: perto da origem ficam colados à reta e a dispersão aumenta conforme X cresce. Em a) e c) a faixa tem largura constante e em b) a reta é plana com pouca dispersão, então são homocedásticos.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---


# Área 3: Modelos logísticos, de contagem e multinível

## Supervised Machine Learning: Modelagem Multinível I

### Questão 177735-1-1
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Dadas as seguintes afirmações:

I) Em modelagem multinível, o procedimento de inserção de dummies de grupo não torna possível a identificação dos efeitos contextuais, visto que não se separam os efeitos observáveis dos não observáveis sobre a variável dependente.

II) Em modelagem multinível, o procedimento de inserção de dummies de grupo é a melhor decisão a ser tomada.

III) Apenas a inserção de dummies de grupo, em modelagem multinível, faz com que sejam capturados os efeitos contextuais sobre a variável dependente.

Assinale a alternativa CORRETA:
Dadas as seguintes afirmações:
I) Em modelagem multinível, o procedimento de inserção de dummies de grupo não torna possível a identificação dos efeitos contextuais, visto que não se separam os efeitos observáveis dos não observáveis sobre a variável dependente.
II) Em modelagem multinível, o procedimento de inserção de dummies de grupo é a melhor decisão a ser tomada.
III) Apenas a inserção de dummies de grupo, em modelagem multinível, faz com que sejam capturados os efeitos contextuais sobre a variável dependente.
Assinale a alternativa CORRETA:

- a) Apenas as afirmações II e III estão corretas.
- b) Todas as afirmações estão corretas.
- c) Apenas a afirmação I está correta.
- d) Apenas as afirmações I e III estão corretas.

**Resposta certa:** c) Apenas a afirmação I está correta.

**Explicação:** A resposta é que só a afirmação I está correta. Inserir dummies de grupo não separa efeitos observáveis dos não observáveis, então não captura os efeitos contextuais, e por isso a modelagem multinível é preferida. A II e a III dizem o contrário: tratam as dummies como a melhor ou a única forma de capturar o contexto.

**Fonte:** Aula de Modelagem Multinível, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-10
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Assinale a alternativa que NÃO traz um exemplo de observações aninhadas em contextos (nesta ordem), ou seja, que NÃO tornaria possível a definição direta de níveis hierárquicos para a estimação de uma modelagem multinível.

- a) Camelos e Ursos Polares.
- b) Famílias e Bairros.
- c) Alunos e Escolas.
- d) Firmas e Países.

**Resposta certa:** a) Camelos e Ursos Polares.

**Explicação:** A resposta é camelos e ursos polares, porque um animal não está aninhado no outro. Alunos em escolas, famílias em bairros e firmas em países são casos em que cada observação pertence a um contexto, o que define os níveis hierárquicos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 177735-1-2
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Em relação a modelagens multinível, afirma-se:

I) Deve haver aninhamento entre observações e contextos a que pertencem estas observações, fato que caracteriza o nível hierárquico.

II) Quando não houver grupos diretamente observáveis, técnicas não supervisionadas de machine learning, como análise de clusters, poderão ser úteis para se definirem contextos (grupos) latentes, ou não observáveis.

III) Apresentam componentes de efeitos fixos e de efeitos aleatórios em sua expressão algébrica.

Assinale a alternativa CORRETA:
Em relação a modelagens multinível, afirma-se:
I) Deve haver aninhamento entre observações e contextos a que pertencem estas observações, fato que caracteriza o nível hierárquico.
II) Quando não houver grupos diretamente observáveis, técnicas não supervisionadas de machine learning, como análise de clusters, poderão ser úteis para se definirem contextos (grupos) latentes, ou não observáveis.
III) Apresentam componentes de efeitos fixos e de efeitos aleatórios em sua expressão algébrica.
Assinale a alternativa CORRETA:

- a) Apenas as afirmações I e II estão corretas.
- b) Apenas as afirmações I e III estão corretas.
- c) Apenas as afirmações II e III estão corretas.
- d) Todas as afirmações estão corretas.

**Resposta certa:** d) Todas as afirmações estão corretas.

**Explicação:** A resposta é que as três afirmações estão corretas. Modelos multinível exigem observações aninhadas em contextos. Quando os grupos não são observáveis, a análise de clusters pode definir contextos latentes. E a expressão algébrica traz uma parte de efeitos fixos e outra de efeitos aleatórios.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 897; Aula de Modelagem Multinível, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-3
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Em relação aos modelos multinível, é CORRETO dizer que:

- a) São estimados pelo método de Máxima Verossimilhança no Conceito Restrito (REML).
- b) São estimados pelo método de Máximos Quadrados Não Ordinários.
- c) São estimados pelo método de Minimum Variance Quadratic Unbiased Estimation (MIVQUE).
- d) São estimados pelo método de Mínimos Quadrados Ordinários.

**Resposta certa:** a) São estimados pelo método de Máxima Verossimilhança no Conceito Restrito (REML).

**Explicação:** A resposta é a máxima verossimilhança restrita (REML). Os componentes de variância dos modelos multinível são estimados por máxima verossimilhança ou por REML, de forma iterativa. Mínimos quadrados ordinários não servem quando as variâncias dos termos aleatórios são diferentes de zero.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 893

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-4
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Assinale a alternativa que mostra, visualmente, o conceito de modelagem multinível.

[imagem: imagens/177735_1_4_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** c) c)

**Explicação:** Na figura c) há vários grupos coloridos, cada um com sua nuvem de pontos e sua própria reta de ajuste, com interceptos e inclinações diferentes. É isso que a modelagem multinível representa: observações aninhadas em contextos. Nas figuras a), b) e d) existe uma única reta ou curva para todos os pontos, sem grupos.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-5
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Considere o enunciado da imagem abaixo e assinale a alternativa CORRETA.

[imagem: imagens/177735_1_5_0.jpg]

- a) Possivelmente apenas o termo aleatório de inclinação (n1) apresentará variância estatisticamente significante, já que o intercepto de todas as retas é exatamente o mesmo.
- b) Os termos aleatórios de intercepto e inclinação (n0 e n1, respectivamente) possivelmente apresentarão variâncias estatisticamente significantes.
- c) Possivelmente apenas o termo aleatório de intercepto (n0) apresentará variância estatisticamente significante, já que todas as retas são paralelas.
- d) Os termos aleatórios de intercepto e inclinação (n0 e n1, respectivamente) possivelmente não apresentarão variâncias estatisticamente significantes, já que não faz sentido a estimação de um modelo multinível, e um modelo de equação única (GLM) será mais adequado neste caso.

**Resposta certa:** b) Os termos aleatórios de intercepto e inclinação (n0 e n1, respectivamente) possivelmente apresentarão variâncias estatisticamente significantes.

**Explicação:** No gráfico as retas dos grupos partem de alturas diferentes (de uns 15 até uns 40 no início) e têm inclinações distintas, algumas bem íngremes e outras quase planas, então não são paralelas nem têm o mesmo intercepto. Como a especificação traz ν0j e ν1j, os dois termos aleatórios devem ter variância significante.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-6
Área 3 · Supervised Machine Learning: Modelagem Multinível I

São nomenclaturas para os modelos multinível:

- a) Modelos para Dados de Contagem, Modelos Poisson, Modelos Binomiais Negativos, Modelos Inflacionados de Zeros.
- b) Modelos Não Supervisionados de Machine Learning.
- c) GLM, Modelos de Regressão Simples e Múltipla, Modelos Logísticos e Modelos Poisson.
- d) GLMM, Modelos Hierárquicos, GLLAMM, Random Coefficients Models, Mixed Models.

**Resposta certa:** d) GLMM, Modelos Hierárquicos, GLLAMM, Random Coefficients Models, Mixed Models.

**Explicação:** A resposta é a lista GLMM, modelos hierárquicos, GLLAMM, random coefficients models e mixed models, que são nomes usados para os modelos multinível. As outras listas trazem GLM, regressão simples, logística e Poisson, que não consideram a estrutura aninhada, ou modelos não supervisionados.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 886; Aula de Modelagem Multinível, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-7
Área 3 · Supervised Machine Learning: Modelagem Multinível I

O que são modelos multinível?

- a) São modelos que, assim como os Modelos Lineares Generalizados, consideram grupos contextuais por meio da inserção apenas de dummies como variáveis preditoras.
- b) São modelos que reconhecem a existência de estrutura hierárquica ou contextual nos dados.
- c) São modelos GLM.
- d) São modelos que não reconhecem a importância dos efeitos contextuais sobre o fenômeno em análise.

**Resposta certa:** b) São modelos que reconhecem a existência de estrutura hierárquica ou contextual nos dados.

**Explicação:** A resposta é que modelos multinível reconhecem a estrutura hierárquica ou contextual dos dados. Eles não se limitam a dummies de grupo como os GLM, e justamente levam em conta os efeitos contextuais sobre o fenômeno estudado.

**Fonte:** Aula de Modelagem Multinível, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-8
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Considere o seguinte modelo multinível da imagem abaixo em que Y é a variável dependente, X é uma variável preditora de nível 1 (indivíduos i), W é uma variável preditora contextual (grupos contextuais j), g são os parâmetros a serem estimados, n0 e n1 representam, respectivamente, os termos aleatórios de intercepto e inclinação de nível 2, e e representa os termo de erro idiossincráticos (nível 1).

Assinale a alternativa CORRETA:
Considere o seguinte modelo multinível da imagem abaixo em que Y é a variável dependente, X é uma variável preditora de nível 1 (indivíduos i), W é uma variável preditora contextual (grupos contextuais j), g são os parâmetros a serem estimados, n0 e n1 representam, respectivamente, os termos aleatórios de intercepto e inclinação de nível 2, e e representa os termo de erro idiossincráticos (nível 1).
Assinale a alternativa CORRETA:

[imagem: imagens/177735_1_8_0.jpg]

- a) Se as variâncias dos termos aleatórios n0 e n1 para os grupos j forem estatisticamente diferentes de zero, procedimentos tradicionais de estimação dos parâmetros do modelo, como mínimos quadrados ordinários, não serão adequados.
- b) Se as variâncias dos termos aleatórios n0 e n1 para os grupos j forem estatisticamente iguais a zero, procedimentos tradicionais de estimação dos parâmetros do modelo, como máximos cúbicos ordinários, não serão adequados.
- c) Se as variâncias dos termos aleatórios n0 e n1 para os grupos j forem estatisticamente diferentes a zero, procedimentos tradicionais de estimação dos parâmetros do modelo, como mínimos quadrados ordinários, serão bastante adequados.
- d) Nenhuma das anteriores.

**Resposta certa:** a) Se as variâncias dos termos aleatórios n0 e n1 para os grupos j forem estatisticamente diferentes de zero, procedimentos tradicionais de estimação dos parâmetros do modelo, como mínimos quadrados ordinários, não serão adequados.

**Explicação:** A resposta é que, se as variâncias dos termos aleatórios de intercepto e inclinação forem diferentes de zero, os mínimos quadrados ordinários não são adequados. Nesse caso há variabilidade entre grupos que o MQO ignora. As outras alternativas inventam o método dos máximos cúbicos ou dizem que o MQO serviria.

**Fonte:** Aula de Modelagem Multinível, pág. 17

**Situação:** explicação conferida com o material das aulas

---

### Questão 177735-1-9
Área 3 · Supervised Machine Learning: Modelagem Multinível I

Quatro diferentes modelos (A, B, C e D) foram estimados, a partir de diferentes critérios e considerando, ou não, a perspectiva multinível. O gráfico a seguir apresenta os valores de LogLik para cada um deles, sabendo-se que todos os LogLiks são estatisticamente diferentes entre si (informação obtida a partir de diferentes likelihood ratio tests).

Analise a imagem abaixo e responda: para fins preditivos, qual deverá ser o modelo escolhido pelo critério do LogLik?
Quatro diferentes modelos (A, B, C e D) foram estimados, a partir de diferentes critérios e considerando, ou não, a perspectiva multinível. O gráfico a seguir apresenta os valores de LogLik para cada um deles, sabendo-se que todos os LogLiks são estatisticamente diferentes entre si (informação obtida a partir de diferentes likelihood ratio tests).
Analise a imagem abaixo e responda: para fins preditivos, qual deverá ser o modelo escolhido pelo critério do LogLik?

[imagem: imagens/177735_1_9_0.jpg]

- a) A
- b) B
- c) C
- d) D

**Resposta certa:** a) A

**Explicação:** O critério do LogLik escolhe o maior valor, isto é, o menos negativo. Na figura A tem -894,568, B tem -906,803, C tem -1416,01 e D tem -1633,49. Como todos os LogLiks diferem significativamente, o modelo A é o escolhido.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Modelagem Multinível II

### Questão 178588-1-1
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Seguindo a nomenclatura adotada em aula, apresenta-se a seguinte especificação de um modelo multinível.

[imagem: imagens/178588_1_1_0.jpg]

- a) Modelo nulo HLM2.
- b) Modelos HLM3 com medidas repetidas.
- c) Modelo HLM2 com interceptos e inclinações aleatórios no nível 2.
- d) Modelos HLM3 com interceptos e inclinações aleatórios.

**Resposta certa:** c) Modelo HLM2 com interceptos e inclinações aleatórios no nível 2.

**Explicação:** A especificação tem Yij = β0j + β1j·Xij + εij, com β0j = γ00 + ν0j e β1j = γ10 + ν1j. São dois níveis (indivíduo i dentro de grupo j), com intercepto e inclinação variando por grupo via ν0j e ν1j, sem preditora de nível 2. Isso é um HLM2 com interceptos e inclinações aleatórios no nível 2.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-10
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Considerando os conceitos apresentados em aula, assinale a alternativa que apresenta uma característica central dos modelos multinível:

- a) São modelos utilizados exclusivamente quando todas as observações da amostra são independentes entre si.
- b) São modelos aplicáveis apenas a bases de dados com uma única variável dependente categórica.
- c) São modelos que reconhecem a existência de estruturas hierárquicas ou multiníveis nos dados.
- d) São modelos que exigem, necessariamente, que todas as variáveis explicativas sejam qualitativas.

**Resposta certa:** c) São modelos que reconhecem a existência de estruturas hierárquicas ou multiníveis nos dados.

**Explicação:** A resposta é que modelos multinível reconhecem estruturas hierárquicas ou multiníveis nos dados. Eles servem justamente para observações que não são independentes, por estarem aninhadas em contextos. Também não se limitam a dependente categórica nem a explicativas qualitativas.

**Fonte:** Aula de Modelagem Multinível, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-2
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Em um modelo multinível com medidas repetidas (períodos de tempo) aninhados em indivíduos, é CORRETO afirmar que:

- a) tanto indivíduos como períodos de tempo são definidos como nível 2, já que os grupos a que pertencem os indivíduos serão definidos como nível 1.
- b) os períodos de tempo são definidos como nível 2, e os indivíduos como nível 1.
- c) os períodos de tempo são definidos como nível 1, e os indivíduos como nível 2.
- d) nenhuma das anteriores.

**Resposta certa:** c) os períodos de tempo são definidos como nível 1, e os indivíduos como nível 2.

**Explicação:** A resposta é que os períodos de tempo são nível 1 e os indivíduos são nível 2. Em medidas repetidas, as observações no tempo estão aninhadas nos indivíduos, e estes podem estar aninhados em grupos, que seriam o nível 3.

**Fonte:** Aula de Modelagem Multinível, pág. 38

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-3
Área 3 · Supervised Machine Learning: Modelagem Multinível II

A partir da estimação de quatro modelos por meio de um dataset com estrutura hierárquica nos dados, obtiveram-se os respectivos valores de LogLik, conforme mostra a figura abaixo.

Pergunta-se: Qual o modelo mais adequado para fins de melhor ajuste entre os valores previstos da variável dependente (fitted values) e valores reais?
A partir da estimação de quatro modelos por meio de um dataset com estrutura hierárquica nos dados, obtiveram-se os respectivos valores de LogLik, conforme mostra a figura abaixo.
Pergunta-se: Qual o modelo mais adequado para fins de melhor ajuste entre os valores previstos da variável dependente (fitted values) e valores reais?

[imagem: imagens/178588_1_3_0.jpg]

- a) HLM2 Nulo.
- b) Modelo com Interceptos Aleatórios.
- c) OLS Nulo.
- d) Modelo com Interceptos e Inclinações Aleatórios.

**Resposta certa:** d) Modelo com Interceptos e Inclinações Aleatórios.

**Explicação:** A figura mostra LogLik de -906,803 para o modelo com interceptos e inclinações aleatórios, -1155,247 para o de interceptos aleatórios, -1416,007 para o HLM2 nulo e -1633,485 para o OLS nulo. O maior valor, o menos negativo, é o -906,803, então esse é o modelo de melhor aderência entre fitted values e valores reais.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-4
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Os modelos multinível com medidas repetidas são caracterizados:

- a) pela repetição de dados dos grupos contextuais, sendo que a estimação dos parâmetros é realizada pelo método OLS.
- b) pela evolução temporal dos dados, representada no nível 1 da análise.
- c) pela estimação dos parâmetros pelo método de scatter search fleet rout size mix evolution.
- d) pela existência de apenas um nível de análise.

**Resposta certa:** b) pela evolução temporal dos dados, representada no nível 1 da análise.

**Explicação:** A resposta é que a evolução temporal dos dados entra como nível 1 da análise. Essa evolução no tempo é o que caracteriza as medidas repetidas, e os indivíduos e grupos aparecem nos níveis 2 e 3. O método de estimação não é o OLS e há mais de um nível.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 895; Aula de Modelagem Multinível, pág. 38

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-5
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Seguindo a nomenclatura adotada em aula, apresenta-se a seguinte especificação de um modelo multinível na imagem abaixo. A partir da especificação apresentada, é possível definir o modelo proposto como sendo um.

[imagem: imagens/178588_1_5_0.jpg]

- a) Modelo nulo HLM2.
- b) Modelos HLM3 com interceptos e inclinações aleatórios.
- c) Modelos HLM2 com inclinações aleatórias.
- d) Modelo nulo HLM3 com medidas repetidas.

**Resposta certa:** a) Modelo nulo HLM2.

**Explicação:** A figura traz Yij = β0j + εij com β0j = γ00 + ν0j. Só há o intercepto aleatório ν0j, sem preditoras e sem inclinação aleatória, em dois níveis (i dentro de j). É o modelo nulo HLM2. O HLM3 exigiria um terceiro nível e o modelo com inclinações teria um termo ν1j.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-6
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Para o estudo da evolução temporal do desempenho de estudantes pertencentes a diferentes escolas, estimou-se um modelo HLM3 com medidas repetidas. Neste caso, é CORRETO dizer que os níveis 1, 2 e 3 desta modelagem serão caracterizados, respectivamente, por:

- a) escolas, estudantes e evolução temporal.
- b) estudantes, escolas e evolução temporal.
- c) a evolução temporal, estudantes e escolas.
- d) evolução temporal, escolas e estudantes.

**Resposta certa:** c) a evolução temporal, estudantes e escolas.

**Explicação:** A resposta é evolução temporal, estudantes e escolas, nessa ordem. Em um HLM3 com medidas repetidas o tempo é o nível 1, o estudante o nível 2 e a escola o nível 3, com os períodos aninhados nos estudantes e estes nas escolas.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 941

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-7
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Sejam as seguintes afirmações sobre os modelos multinível.

I) O modelo final pode ser obtido após a aplicação de um procedimento Stepwise.

II) O modelo final pode ser obtido após a aplicação de uma Step-Up Strategy, já que procedimentos tradicionais Stepwise não são definidos em modelos com componentes fixos e aleatórios.

III) Os parâmetros podem ser estimados pelo método REML (restricted estimation of maximum likelihood).

Assinale a alternativa CORRETA:
Sejam as seguintes afirmações sobre os modelos multinível.
I) O modelo final pode ser obtido após a aplicação de um procedimento Stepwise.
II) O modelo final pode ser obtido após a aplicação de uma Step-Up Strategy, já que procedimentos tradicionais Stepwise não são definidos em modelos com componentes fixos e aleatórios.
III) Os parâmetros podem ser estimados pelo método REML (restricted estimation of maximum likelihood).
Assinale a alternativa CORRETA:

- a) Apenas a afirmação I está correta.
- b) Apenas as afirmações I e III estão corretas.
- c) Todas as afirmações estão corretas.
- d) Apenas as afirmações II e III estão corretas.

**Resposta certa:** d) Apenas as afirmações II e III estão corretas.

**Explicação:** A resposta é que só II e III estão corretas. O REML é um dos métodos de estimação dos parâmetros. Como o modelo tem parte fixa e parte aleatória, o modelo final costuma ser montado incluindo termos por etapas, na lógica step-up, em vez de um Stepwise tradicional, o que torna a afirmação I incorreta.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 893

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-8
Área 3 · Supervised Machine Learning: Modelagem Multinível II

A partir de determinado dataset com estrutura hierárquica, foi estimado um modelo multinível com dois níveis (estudantes aninhados em escolas), sendo gerado um gráfico dos efeitos aleatórios de intercepto (n0j) de cada uma das escolas, conforme mostra a figura a seguir:

[imagem: imagens/178588_1_8_0.jpg]

- a) Todas as afirmações estão corretas.
- b) Apenas as afirmações I e II estão corretas.
- c) Apenas as afirmações II e III estão corretas.
- d) Nenhuma afirmação está correta.

**Resposta certa:** a) Todas as afirmações estão corretas.

**Explicação:** Pelo gráfico a escola 3 tem o maior ν0j (6,0908), então I está certa. A escola 7 tem o menor (-8,2709), então II está certa. A III também está certa: se os interceptos aleatórios variam entre escolas com variância diferente de zero, o OLS, que supõe um intercepto único, não é adequado. Logo todas estão corretas.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 178588-1-9
Área 3 · Supervised Machine Learning: Modelagem Multinível II

Escolha a alternativa que apresenta um possível código do Python para se estimar um modelo multinível HLM2, sendo y a variável dependente, x a variável preditora de nível 1 e w a variável preditora de nível 2 (contexto):

[imagem: imagens/178588_1_9_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** d) d)

**Explicação:** A alternativa d) usa sm.MixedLM.from_formula do statsmodels, com a fórmula y ~ x + w + x:w (efeitos fixos de nível 1, nível 2 e a interação), groups = 'contexto' e re_formula = 'x' para a inclinação aleatória. As outras usam funções que não existem no Python (mle, glmm, multilevel) e a a) nem tem o til da fórmula.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

### Questão 174205-1-1
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Assinale a alternativa INCORRETA sobre a função logística:

- a) A variável dependente se apresenta na forma quantitativa e com média maior que zero.
- b) A estimação dos parâmetros desta função é um processo iterativo para maximizar o acerto da probabilidade de ocorrência de um evento à sua real ocorrência, por meio do Método de Máxima Verossimilhança.
- c) Esta função é definida para que se estabeleça a probabilidade de ocorrência de determinado evento.
- d) Para se analisar a qualidade do ajuste do modelo para determinado cutoff, podemos utilizar uma matriz de confusão.

**Resposta certa:** a) A variável dependente se apresenta na forma quantitativa e com média maior que zero.

**Explicação:** A alternativa incorreta é a que diz que a variável dependente é quantitativa. Na regressão logística binária a dependente é qualitativa dicotômica. As demais estão certas: a função dá a probabilidade de um evento, os parâmetros vêm da máxima verossimilhança e o ajuste pode ser avaliado pela matriz de confusão.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 13

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-10
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Em matrizes de confusão, o que significa a especificidade?

- a) Taxa de acerto do modelo para as observações classificadas como “evento”.
- b) Taxa de acerto do modelo para as observações classificadas como “não evento”.
- c) Taxa de erro do modelo.
- d) Taxa global de acerto do modelo.

**Resposta certa:** b) Taxa de acerto do modelo para as observações classificadas como “não evento”.

**Explicação:** A resposta é a taxa de acerto para o não evento. Especificidade é o percentual de acertos considerando só as observações que de fato não são evento, enquanto a sensitividade faz o mesmo para os eventos. No exemplo do livro, 30 de 41 dá 0,7317.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 664

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-2
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Considere os conceitos apresentados em aula e assinale a alternativa CORRETA:

- a) Nos modelos de regressão logística, a variável dependente deve seguir distribuição normal e ter variância constante, sendo esses os principais pressupostos do modelo.
- b) Nos modelos de regressão logística binária, a variável dependente é contínua e as variáveis preditoras devem ser exclusivamente métricas.
- c) Nos modelos de regressão logística multinomial, a variável dependente é binária e o modelo estima os coeficientes pelo método dos mínimos quadrados ordinários.
- d) Nos modelos de regressão logística binária, a variável dependente é binária e as variáveis preditoras podem ser métricas ou não métricas.

**Resposta certa:** d) Nos modelos de regressão logística binária, a variável dependente é binária e as variáveis preditoras podem ser métricas ou não métricas.

**Explicação:** A resposta é que, na logística binária, a dependente é binária e as preditoras podem ser métricas ou não métricas. A logística não exige normalidade nem variância constante. A multinomial tem dependente com mais de duas categorias e também não usa mínimos quadrados.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-3
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

O logaritmo natural da chance de ocorrência de uma resposta do tipo “sim” é definido como:

- a) Acurácia de Napier.
- b) Probito de Euler.
- c) Logito.
- d) Probabilidade de Wald.

**Resposta certa:** c) Logito.

**Explicação:** A resposta é logito. O logito Z é o logaritmo natural da chance (odds) de ocorrência da resposta sim, ou seja, ln(p/(1-p)), e a partir dele se chega à probabilidade.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-4
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Assumindo que um logito possua o valor igual a Z = 1. Em um modelo de regressão logística binária, qual será a probabilidade de ocorrência do evento em estudo?

- a) 0,5
- b) 1
- c) 0,2689
- d) 0,7311

**Resposta certa:** d) 0,7311

**Explicação:** A resposta é 0,7311. A probabilidade é p = 1/(1+e^-Z). Para Z = 1, p = 1/(1+e^-1) = 1/(1+0,3679) = 0,7311. O valor 0,2689 é o que se obtém com Z = -1.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 643

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-5
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Assumindo que um logito possua o valor igual a Z = 0. Em um modelo de regressão logística binária, qual será a probabilidade de ocorrência do evento em estudo?

- a) 0,9933
- b) 0,5
- c) 1
- d) 0,7311

**Resposta certa:** b) 0,5

**Explicação:** A resposta é 0,5. Com Z = 0, p = 1/(1+e^0) = 1/2 = 0,5, o ponto em que a chance é 1 para 1. A probabilidade só se aproxima de 1 quando Z fica muito grande.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 643

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-6
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Os parâmetros de modelos de regressão logística são estimados por:

- a) Mínima Verossimilhança.
- b) Máxima Verossimilhança.
- c) Máximos Quadrados Ordinários.
- d) Mínimos Quadrados Ordinários.

**Resposta certa:** b) Máxima Verossimilhança.

**Explicação:** A resposta é máxima verossimilhança. Os parâmetros da logística são estimados de forma iterativa, buscando os valores que maximizam a verossimilhança de acertar a ocorrência real do evento. Mínimos quadrados ordinários são o método da regressão linear.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 13

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-7
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Sobre os conceitos probabilidade e chance, julgue as afirmações a seguir:

I) Em Estatística, a chance (em inglês, odds) de ocorrência de determinado evento é a probabilidade de sua ocorrência dividida pela probabilidade da não ocorrência desse mesmo evento.

II) Se a probabilidade de ocorrência de um evento é de 80%, então a chance de ocorrência deste evento é de 4 para 1.

III) Se a probabilidade de ocorrência de um evento é de 25%, então a chance de ocorrência deste evento é de 1 para 3.

Assinale a alternativa CORRETA:
Sobre os conceitos probabilidade e chance, julgue as afirmações a seguir:
I) Em Estatística, a chance (em inglês, odds) de ocorrência de determinado evento é a probabilidade de sua ocorrência dividida pela probabilidade da não ocorrência desse mesmo evento.
II) Se a probabilidade de ocorrência de um evento é de 80%, então a chance de ocorrência deste evento é de 4 para 1.
III) Se a probabilidade de ocorrência de um evento é de 25%, então a chance de ocorrência deste evento é de 1 para 3.
Assinale a alternativa CORRETA:

- a) Somente as afirmações II e III estão corretas.
- b) Todas as afirmações estão corretas.
- c) Somente a afirmação I está correta.
- d) Somente a afirmação III está correta.

**Resposta certa:** b) Todas as afirmações estão corretas.

**Explicação:** A resposta é que todas estão corretas. Chance é p/(1-p). Com p = 0,80, chance = 0,8/0,2 = 4, ou seja, 4 para 1. Com p = 0,25, chance = 0,25/0,75 = 1/3, ou seja, 1 para 3.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-8
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Sobre o modelo de regressão logística binária, podemos afirmar que:

- a) Trata-se de uma técnica supervisionada de machine learning para explicar ou predizer a probabilidade de ocorrência de determinado evento dicotômico em função de uma ou mais variáveis explicativas.
- b) Neste tipo de modelo, a variável dependente será sempre quantitativa.
- c) Não faz sentido estimar um modelo supervisionado de machine learning quando a variável dependente for qualitativa dicotômica.
- d) As variáveis X poderão ser somente qualitativas.

**Resposta certa:** a) Trata-se de uma técnica supervisionada de machine learning para explicar ou predizer a probabilidade de ocorrência de determinado evento dicotômico em função de uma ou mais variáveis explicativas.

**Explicação:** A resposta é a que descreve a logística binária como técnica supervisionada para explicar ou predizer a probabilidade de um evento dicotômico. A dependente é qualitativa binária, não quantitativa, e as variáveis X podem ser métricas ou não métricas, não só qualitativas.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 174205-1-9
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais I

Considere o seguinte logito para um modelo de risco de crédito de empresas (evento = obtenção de crédito):

Z = a + b1.rating + b2.disclosure

Sendo a = 0,034; b1 = 0,000275; b2 = 0,017

Para determinada empresa, tem-se que rating = 85 e disclosure = 62. Qual valor a probabilidade de ocorrência do evento em estudo decorrente de uma regressão logística binária?
Considere o seguinte logito para um modelo de risco de crédito de empresas (evento = obtenção de crédito):
Z = a + b1.rating + b2.disclosure
Sendo a = 0,034; b1 = 0,000275; b2 = 0,017
Para determinada empresa, tem-se que rating = 85 e disclosure = 62. Qual valor a probabilidade de ocorrência do evento em estudo decorrente de uma regressão logística binária?

- a) 0,999
- b) 0,752
- c) 0,333
- d) 0,248

**Resposta certa:** b) 0,752

**Explicação:** A resposta é 0,752. Z = 0,034 + 0,000275 x 85 + 0,017 x 62 = 0,034 + 0,0234 + 1,054 = 1,1114. Então p = 1/(1+e^-1,1114) = 1/(1+0,3292) = 0,752. O valor 0,248 seria a probabilidade do não evento.

**Fonte:** Aula de Modelos Logísticos Binários, pág. 12

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

### Questão 175062-1-1
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Dada a seguinte matriz de confusão (com lógica igual à apresentada em aula) obtida após a estimação de um modelo de regressão logística binária e com cutoff = 0,5, escolha a alternativa que apresenta a eficiência global do modelo (indicador de acurácia).

[imagem: imagens/175062_1_1_0.jpg]

- a) 70,20%
- b) 86,00%
- c) 12,40%
- d) 14,00%

**Resposta certa:** b) 86,00%

**Explicação:** A matriz tem 1470 verdadeiros positivos, 210 falsos positivos, 210 falsos negativos e 1110 verdadeiros negativos, total de 3000. Acurácia = (1470 + 1110)/3000 = 2580/3000 = 86,00%. Os 14,00% são a taxa de erro, (210 + 210)/3000.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-10
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Dada a seguinte matriz de confusão (com lógica igual à apresentada em aula) obtida após a estimação de um modelo de regressão logística binária e com cutoff = 0,5, escolha a alternativa que apresenta a sensitividade do modelo.

[imagem: imagens/175062_1_10_0.jpg]

- a) 30,20%
- b) 77,40%
- c) 12,50%
- d) 87,50%

**Resposta certa:** d) 87,50%

**Explicação:** A matriz mostra 1470 verdadeiros positivos e 210 falsos negativos (eventos reais classificados como 0). Sensitividade = 1470/(1470 + 210) = 1470/1680 = 87,50%. Os 12,50% são o complemento, 210/1680.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-2
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Para o estudo das probabilidades de não se chegar atrasado às aulas (categoria de referência), de se chegar atrasado à primeira aula (primeira categoria alternativa) ou de se chegar atrasado à segunda aula (segunda categoria alternativa) por parte de alunos de determinada escola, em função da distância (em km) de onde partem até a escola (variável preditora dist) e da quantidade de semáforos por que passam ao longo do trajeto (variável preditora sem), estimou-se um modelo de regressão logística multinomial. Os outputs com os parâmetros (todos estatisticamente significantes ao nível de confiança de 95%) encontram-se na imagem a seguir.

Pergunta-se: qual a probabilidade de que determinado aluno não chegue atrasado às aulas, sabendo-se que durante o trajeto de 22 km há 12 semáforos?
Para o estudo das probabilidades de não se chegar atrasado às aulas (categoria de referência), de se chegar atrasado à primeira aula (primeira categoria alternativa) ou de se chegar atrasado à segunda aula (segunda categoria alternativa) por parte de alunos de determinada escola, em função da distância (em km) de onde partem até a escola (variável preditora dist) e da quantidade de semáforos por que passam ao longo do trajeto (variável preditora sem), estimou-se um modelo de regressão logística multinomial. Os outputs com os parâmetros (todos estatisticamente significantes ao nível de confiança de 95%) encontram-se na imagem a seguir.
Pergunta-se: qual a probabilidade de que determinado aluno não chegue atrasado às aulas, sabendo-se que durante o trajeto de 22 km há 12 semáforos?

[imagem: imagens/175062_1_2_0.jpg]

- a) 41,77%
- b) 68,02%
- c) 30,52%
- d) 1,48%

**Resposta certa:** b) 68,02%

**Explicação:** Com dist = 22 e sem = 12: Z1 = -33,1352 + 0,5588x22 + 1,6699x12 = -0,80 e e^Z1 = 0,4481. Z2 = -62,2922 + 1,0784x22 + 2,8949x12 = -3,83 e e^Z2 = 0,0217. A probabilidade da categoria de referência é 1/(1 + 0,4481 + 0,0217) = 1/1,4698 = 68,02%.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-3
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Considere as seguintes afirmações:

I) A regressão logística multinomial pode ser vista como uma extensão do modelo de regressão logística binária, em situações nas quais a variável dependente apresenta múltiplas categorias.

II) É possível estimar um modelo de regressão logística em que a variável dependente apresenta mais de duas categorias.

III) Em um modelo de regressão logística multinomial são estimados (M – 1) logitos, sendo M o número de categorias da variável dependente.

Assinale a alternativa CORRETA:
Considere as seguintes afirmações:
I) A regressão logística multinomial pode ser vista como uma extensão do modelo de regressão logística binária, em situações nas quais a variável dependente apresenta múltiplas categorias.
II) É possível estimar um modelo de regressão logística em que a variável dependente apresenta mais de duas categorias.
III) Em um modelo de regressão logística multinomial são estimados (M – 1) logitos, sendo M o número de categorias da variável dependente.
Assinale a alternativa CORRETA:

- a) Somente as afirmações II e III estão corretas.
- b) Nenhuma afirmação está correta.
- c) Somente as afirmações I e II estão corretas.
- d) Todas as afirmações estão corretas.

**Resposta certa:** d) Todas as afirmações estão corretas.

**Explicação:** A resposta é todas corretas. A multinomial estende a logística binária para uma variável dependente com mais de duas categorias, então estimar logística com mais de duas categorias é possível. Escolhe-se uma categoria de referência e estimam-se M – 1 logitos: com três categorias (0, 1, 2) saem dois logitos, um para 1 e outro para 2 contra a referência 0.

**Fonte:** Aula de regressão logística multinomial, pág. 16; Manual de Análise de Dados (Fávero), pág. 668

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-4
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Para se avaliar a probabilidade de se chegar atrasado à aula (evento = atrasado; não evento = não atrasado) por parte de alunos de determinada escola, em função da distância (em km) de onde partem até a escola (variável preditora dist) e da quantidade de semáforos por que passam ao longo do trajeto (variável preditora sem), estimou-se um modelo de regressão logística binária. Os outputs encontram-se na imagem a seguir.

Pergunta-se: qual a probabilidade de que determinado aluno chegue atrasado, sabendo-se que durante o trajeto de 10 km há 10 semáforos?
Para se avaliar a probabilidade de se chegar atrasado à aula (evento = atrasado; não evento = não atrasado) por parte de alunos de determinada escola, em função da distância (em km) de onde partem até a escola (variável preditora dist) e da quantidade de semáforos por que passam ao longo do trajeto (variável preditora sem), estimou-se um modelo de regressão logística binária. Os outputs encontram-se na imagem a seguir.
Pergunta-se: qual a probabilidade de que determinado aluno chegue atrasado, sabendo-se que durante o trajeto de 10 km há 10 semáforos?

[imagem: imagens/175062_1_4_0.jpg]

- a) 34,66%
- b) 4,84%
- c) 50,77%
- d) 65,34%

**Resposta certa:** a) 34,66%

**Explicação:** Z = -26,1665 + 0,1904x10 + 2,3629x10 = -0,6335. A probabilidade é p = 1/(1 + e^0,6335) = 1/(1 + 1,8844) = 34,66%. Os 65,34% são o complemento, a chance de não chegar atrasado.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-5
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Para se verificar se pelo menos um dos betas é estatisticamente significante em um modelo de regressão logística binária, deve-se utilizar o resultado de qual teste?

- a) Box-Francia.
- b) Shapiro-Cox.
- c) Qui-quadrado (c²).
- d) F.

**Resposta certa:** c) Qui-quadrado (c²).

**Explicação:** A resposta é o qui-quadrado. Na logística binária, o teste qui-quadrado do modelo avalia a significância conjunta: se o valor-P for menor que 0,05, existe pelo menos um beta diferente de zero. Ele equivale ao teste F da regressão linear, mas não diz qual variável importa; para isso usa-se o z de Wald de cada parâmetro. Box-Francia e Shapiro-Cox não são testes de significância de betas.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 653; Aula de regressão logística multinomial, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-6
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Para se avaliar a probabilidade de se chegar atrasado à aula (evento = atrasado; não evento = não atrasado) por parte de alunos de determinada escola, em função da distância (em km) de onde partem até a escola (variável preditora dist) e da quantidade de semáforos por que passam ao longo do trajeto (variável preditora sem), estimou-se um modelo de regressão logística binária. Os outputs encontram-se na imagem a seguir.

Pergunta-se: qual a probabilidade de que determinado aluno chegue atrasado, sabendo-se que durante o trajeto de 6 km há 10 semáforos?
Para se avaliar a probabilidade de se chegar atrasado à aula (evento = atrasado; não evento = não atrasado) por parte de alunos de determinada escola, em função da distância (em km) de onde partem até a escola (variável preditora dist) e da quantidade de semáforos por que passam ao longo do trajeto (variável preditora sem), estimou-se um modelo de regressão logística binária. Os outputs encontram-se na imagem a seguir.
Pergunta-se: qual a probabilidade de que determinado aluno chegue atrasado, sabendo-se que durante o trajeto de 6 km há 10 semáforos?

[imagem: imagens/175062_1_6_0.jpg]

- a) 19,85%
- b) 50,77%
- c) 4,84%
- d) 80,15%

**Resposta certa:** a) 19,85%

**Explicação:** Z = -26,1665 + 0,1904x6 + 2,3629x10 = -1,3951. A probabilidade é p = 1/(1 + e^1,3951) = 1/(1 + 4,0355) = 19,85%. Com 6 km a chance é menor que com 10 km (34,66%), já que o coeficiente de dist é positivo. Os 80,15% são o complemento.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-7
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Foram estimados quatro modelos de regressão logística binária (A, B, C e D), com quatro diferentes grupos de variáveis preditoras. Os valores de log-likelihood de cada modelo encontram-se no gráfico a seguir.

Pergunta-se: Qual o modelo com melhor qualidade do ajuste para fins preditivos?
Foram estimados quatro modelos de regressão logística binária (A, B, C e D), com quatro diferentes grupos de variáveis preditoras. Os valores de log-likelihood de cada modelo encontram-se no gráfico a seguir.
Pergunta-se: Qual o modelo com melhor qualidade do ajuste para fins preditivos?

[imagem: imagens/175062_1_7_0.jpg]

- a) A.
- b) B.
- c) C.
- d) D.

**Resposta certa:** d) D.

**Explicação:** O melhor ajuste é o de maior log-likelihood, isto é, o menos negativo. Os valores do gráfico são A = -2071,79, B = -1781,31, C = -1207,34 e D = -557,26. O D é o mais próximo de zero, então é o de melhor qualidade de ajuste.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-8
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Um indicador bastante útil para se avaliar a eficiência de modelos de regressão logística binária, independentemente do cutoff, é:

- a) Especificidade.
- b) Área abaixo da curva ROC.
- c) Acurácia.
- d) Sensitividade.

**Resposta certa:** b) Área abaixo da curva ROC.

**Explicação:** A resposta é a área abaixo da curva ROC. Sensitividade, especificidade e acurácia mudam conforme o cutoff escolhido. A curva ROC varre todos os cutoffs possíveis entre 0 e 1 e a área abaixo dela resume a eficiência do modelo sem depender de um ponto de corte; quanto mais perto de (0,1), maior a área e melhor o modelo.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 667

**Situação:** explicação conferida com o material das aulas

---

### Questão 175062-1-9
Área 3 · Supervised Machine Learning: Modelos Logísticos Binários e Multinomiais II

Sobre a regressão logística multinomial, apresentam-se as seguintes afirmações:

I) A variável dependente se apresenta na forma qualitativa com mais de duas categorias.

II) Para uma variável qualitativa com três categorias, serão definidos dois logitos.

III) Os parâmetros são estimados por máxima verossimilhança.

Assinale a alternativa CORRETA:
Sobre a regressão logística multinomial, apresentam-se as seguintes afirmações:
I) A variável dependente se apresenta na forma qualitativa com mais de duas categorias.
II) Para uma variável qualitativa com três categorias, serão definidos dois logitos.
III) Os parâmetros são estimados por máxima verossimilhança.
Assinale a alternativa CORRETA:

- a) Nenhuma afirmação está correta.
- b) Todas as afirmações estão corretas.
- c) Somente as afirmações I e II estão corretas.
- d) Somente as afirmações II e III estão corretas.

**Resposta certa:** b) Todas as afirmações estão corretas.

**Explicação:** A resposta é todas corretas. A multinomial tem variável dependente qualitativa com mais de duas categorias. Com três categorias definem-se dois logitos, pois o número de logitos é M – 1. Como em toda regressão logística, os parâmetros são estimados por máxima verossimilhança.

**Fonte:** Aula de regressão logística multinomial, pág. 16; Manual de Análise de Dados (Fávero), pág. 668

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Modelos para Dados de Contagem I

### Questão 176031-1-1
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

São exemplos de variáveis com dados de contagem:

I) Quantidade de vezes que pacientes idosos vão ao médico por ano.

II) Quantidade de ofertas públicas de ações que são realizadas em uma amostra de países desenvolvidos e emergentes por ano.

III) Quantidade de apartamentos à venda por bairro.

IV) Faixa de renda (definida em labels qualitativos) de uma amostra de consumidores.

Assinale a alternativa correta:
São exemplos de variáveis com dados de contagem:
I) Quantidade de vezes que pacientes idosos vão ao médico por ano.
II) Quantidade de ofertas públicas de ações que são realizadas em uma amostra de países desenvolvidos e emergentes por ano.
III) Quantidade de apartamentos à venda por bairro.
IV) Faixa de renda (definida em labels qualitativos) de uma amostra de consumidores.
Assinale a alternativa correta:

- a) Nenhuma afirmação está correta.
- b) Somente as afirmações II e IV estão corretas.
- c) Todas as afirmações estão corretas.
- d) Somente as afirmações I, II e III estão corretas.

**Resposta certa:** d) Somente as afirmações I, II e III estão corretas.

**Explicação:** A resposta é somente I, II e III. Visitas ao médico por ano, ofertas públicas de ações por ano e apartamentos à venda por bairro são quantidades inteiras, não negativas, medidas numa exposição (ano, bairro), ou seja, dados de contagem. A IV é uma faixa de renda em categorias qualitativas, que não é contagem.

**Fonte:** Aula de modelos para dados de contagem, pág. 6; Manual de Análise de Dados (Fávero), pág. 726

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-10
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Os modelos de regressão Poisson e binomial negativo fazem parte do que é conhecido por modelos de regressão para dados de contagem. Qual o principal objetivo desses modelos?

- a) Analisar o comportamento, em função de variáveis preditoras, de determinada variável dependente que se apresenta na forma de contagens discretas e não negativas.
- b) Analisar o comportamento, em função de variáveis preditoras, de determinada variável dependente que se apresenta na forma quantitativa contínua, assumindo qualquer valor no intervalo dos números reais.
- c) Analisar o comportamento, em função de variáveis preditoras, de determinada variável dependente que se apresenta na forma qualitativa, com categorias mutuamente exclusivas e coletivamente exaustivas.
- d) Analisar o comportamento, em função de variáveis preditoras, de determinada variável dependente que se apresenta na forma de proporções, com valores restritos ao intervalo entre zero e um.

**Resposta certa:** a) Analisar o comportamento, em função de variáveis preditoras, de determinada variável dependente que se apresenta na forma de contagens discretas e não negativas.

**Explicação:** A resposta é a que fala em contagens discretas e não negativas. Poisson e binomial negativo explicam uma variável dependente quantitativa que só assume valores inteiros a partir de zero. As demais alternativas descrevem variável contínua (regressão linear), categórica (logística) ou proporção.

**Fonte:** Aula de modelos para dados de contagem, pág. 5; Manual de Análise de Dados (Fávero), pág. 725

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-2
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Sobre os modelos de regressão para dados de contagem, podemos avaliar a qualidade do ajuste do modelo por meio do seguinte indicador:

- a) p-value da estatística t de Student.
- b) Valor de Log-Likelihood.
- c) Área abaixo da curva ROC.
- d) Lambda (l) de Box-Cox.

**Resposta certa:** b) Valor de Log-Likelihood.

**Explicação:** A resposta é o valor de log-likelihood. Poisson e binomial negativo são estimados por máxima verossimilhança, então o ajuste se avalia pelo LL, que o método maximiza: quanto maior, melhor. O p-value do t de Student serve para parâmetros, a curva ROC é de modelos binários e o lambda de Box-Cox pertence a outra técnica.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 176031-1-3
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Uma variável com dados de contagem apresenta as seguintes características:

- a) É quantitativa, apresenta dados discretos e não negativos, e é definida uma exposição.
- b) É quantitativa, apresenta dados contínuos e negativos, e é definida uma exposição.
- c) É quantitativa, apresenta dados discretos e negativos, e não se consegue definir uma exposição.
- d) É qualitativa, apresenta dados contínuos e não negativos, e é definida uma exposição.

**Resposta certa:** a) É quantitativa, apresenta dados discretos e não negativos, e é definida uma exposição.

**Explicação:** A resposta é quantitativa, discreta e não negativa, com exposição definida. Dado de contagem é um número de ocorrências (0, 1, 2...) observado numa unidade de tempo, espaço ou grupo, que é a exposição. Por isso não pode ser contínuo, negativo ou qualitativo.

**Fonte:** Aula de modelos para dados de contagem, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-4
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Os parâmetros de um modelo de regressão do tipo Poisson são estimados pelo método de:

- a) Mínimos Quadrados Ordinários.
- b) Mínima Verossimilhança.
- c) Máximos Quadrados Ordinários.
- d) Máxima Verossimilhança.

**Resposta certa:** d) Máxima Verossimilhança.

**Explicação:** A resposta é máxima verossimilhança. Como nas logísticas binária e multinomial, os parâmetros da regressão Poisson são os que maximizam a função de verossimilhança (ou o seu logaritmo), com a variável dependente seguindo distribuição Poisson. Mínimos quadrados ordinários é o método da regressão linear, e mínima verossimilhança não existe como método.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 731; Aula de modelos para dados de contagem, pág. 3

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-5
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Com o intuito de se estudar e prever a quantidade de violações de trânsito (variável dependente violations) na cidade de Nova York por parte de membros dos corpos diplomáticos dos países pertencentes às Nações Unidas, foi estimado um modelo de regressão Poisson, considerando, como variáveis preditoras, a quantidade de membros no corpo diplomático em cada país (variável staff), o índice de corrupção de cada país (variável corruption) e o fato de haver ou não enforcement legal quanto à obrigatoriedade de se pagar a multa em caso de violação (variável binária post: ‘yes’ = há obrigatoriedade do pagamento; ‘no’ = não há obrigatoriedade do pagamento). Os outputs do referido modelo, obtidos no Python, encontram-se na imagem a seguir.

Pergunta-se: qual a quantidade esperada de violações de trânsito para um país cujo corpo diplomático seja composto por 28 membros, considerando inexistência de enforcement legal (post = ‘no’) e índice de corrupção igual a 1?
Com o intuito de se estudar e prever a quantidade de violações de trânsito (variável dependente violations) na cidade de Nova York por parte de membros dos corpos diplomáticos dos países pertencentes às Nações Unidas, foi estimado um modelo de regressão Poisson, considerando, como variáveis preditoras, a quantidade de membros no corpo diplomático em cada país (variável staff), o índice de corrupção de cada país (variável corruption) e o fato de haver ou não enforcement legal quanto à obrigatoriedade de se pagar a multa em caso de violação (variável binária post: ‘yes’ = há obrigatoriedade do pagamento; ‘no’ = não há obrigatoriedade do pagamento). Os outputs do referido modelo, obtidos no Python, encontram-se na imagem a seguir.
Pergunta-se: qual a quantidade esperada de violações de trânsito para um país cujo corpo diplomático seja composto por 28 membros, considerando inexistência de enforcement legal (post = ‘no’) e índice de corrupção igual a 1?

[imagem: imagens/176031_1_5_0.jpg]

- a) 12,93
- b) 39,32
- c) 57,54
- d) 23,73

**Resposta certa:** d) 23,73

**Explicação:** Com post = 'no' a dummy post[T.yes] vale 0. Z = 2,2127 + 0,0219x28 + 0,3418x1 = 2,2127 + 0,6132 + 0,3418 = 3,1677, e e^3,1677 é cerca de 23,7 violações. Com os coeficientes completos do output o resultado é 23,73.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-6
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

A função e o respectivo pacote para a elaboração direta do teste para verificação de existência de superdispersão nos dados da variável dependente para a estimação de modelos de contagem, no Python, são:

- a) função megadisp do pacote ultradisp.
- b) função superdisp do pacote hiperdisp.
- c) função hiperdisp do pacote megadisp.
- d) função overdisp do pacote statstests.tests.

**Resposta certa:** d) função overdisp do pacote statstests.tests.

**Explicação:** A resposta é a função overdisp do pacote statstests.tests. Ela aplica o teste de superdispersão de Cameron e Trivedi a partir do modelo Poisson estimado, e as outras funções e pacotes das alternativas não existem.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 176031-1-7
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Com o intuito de se estudar e prever a quantidade de violações de trânsito (variável dependente violations) na cidade de Nova York por parte de membros dos corpos diplomáticos dos países pertencentes às Nações Unidas, foi estimado um modelo de regressão Poisson, considerando, como variáveis preditoras, a quantidade de membros no corpo diplomático em cada país (variável staff), o índice de corrupção de cada país (variável corruption) e o fato de haver ou não enforcement legal quanto à obrigatoriedade de se pagar a multa em caso de violação (variável binária post: ‘yes’ = há obrigatoriedade do pagamento; ‘no’ = não há obrigatoriedade do pagamento). Os outputs do referido modelo, obtidos no Python, encontram-se na imagem a seguir.

Pergunta-se: qual a equação do modelo de regressão Poisson que deverá ser utilizada para fins preditivos? O subscrito i refere-se à linha (observação) do dataset.
Com o intuito de se estudar e prever a quantidade de violações de trânsito (variável dependente violations) na cidade de Nova York por parte de membros dos corpos diplomáticos dos países pertencentes às Nações Unidas, foi estimado um modelo de regressão Poisson, considerando, como variáveis preditoras, a quantidade de membros no corpo diplomático em cada país (variável staff), o índice de corrupção de cada país (variável corruption) e o fato de haver ou não enforcement legal quanto à obrigatoriedade de se pagar a multa em caso de violação (variável binária post: ‘yes’ = há obrigatoriedade do pagamento; ‘no’ = não há obrigatoriedade do pagamento). Os outputs do referido modelo, obtidos no Python, encontram-se na imagem a seguir.
Pergunta-se: qual a equação do modelo de regressão Poisson que deverá ser utilizada para fins preditivos? O subscrito i refere-se à linha (observação) do dataset.

[imagem: imagens/176031_1_7_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** a) a)

**Explicação:** No Poisson o logaritmo do valor esperado é linear nos preditores, com os coeficientes da figura: ln(violations_i) = 2,2127 + 0,0219·staff_i - 4,2968·post_yes_i + 0,3418·corruption_i. Essa é a a). A b) e a d) tiram o logaritmo, e a c) coloca o exponencial no lado errado.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-8
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

Qual a característica da superdispersão em determinada variável dependente com dados de contagem?

- a) Média estatisticamente superior à variância.
- b) Variância estatisticamente superior à entropia conjunta das variáveis preditoras.
- c) Variância estatisticamente superior à média.
- d) Variância estatisticamente superior ao desvio-padrão.

**Resposta certa:** c) Variância estatisticamente superior à média.

**Explicação:** A resposta é variância estatisticamente superior à média. No Poisson média e variância são iguais (equidispersão). Quando a variância excede a média há superdispersão, que o binomial negativo comporta ao somar um termo à variância (Var = média + phi x média ao quadrado).

**Fonte:** Manual de Análise de Dados (Fávero), pág. 744; Aula de modelos para dados de contagem, pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 176031-1-9
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem I

O principal teste para verificação de existência de superdispersão nos dados da variável dependente é o:

- a) Teste de Shapiro-Francia.
- b) Teste de Cameron e Trivedi.
- c) Teste de Vuong.
- d) Teste de Lambert.

**Resposta certa:** b) Teste de Cameron e Trivedi.

**Explicação:** A resposta é o teste de Cameron e Trivedi. Estima-se o Poisson, cria-se uma variável auxiliar e roda-se um OLS sem intercepto; se o parâmetro for estatisticamente diferente de zero há superdispersão. O teste de Vuong é outra coisa, serve para o excesso de zeros.

**Fonte:** Aula de modelos para dados de contagem, pág. 12; Manual de Análise de Dados (Fávero), pág. 765

**Situação:** explicação conferida com o material das aulas

---

## Supervised Machine Learning: Modelos para Dados de Contagem II

### Questão 176796-1-1
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

A variável dependente quantitativa a ser considerada em determinado modelo de regressão para dados de contagem apresenta as seguintes estatísticas descritivas. A priori, dentre as alternativas propostas a seguir, qual seria o modelo mais adequado a ser estimado?

[imagem: imagens/176796_1_1_0.jpg]

- a) Poisson.
- b) Binomial negativo.
- c) Logístico binário.
- d) Logístico multinomial.

**Resposta certa:** b) Binomial negativo.

**Explicação:** A figura mostra média de 6,4966 e variância de 331,6178. A variância é muito maior que a média, então há superdispersão e o Poisson (que exige equidispersão) não serve. O binomial negativo é o indicado a priori. Os logísticos são para variável dependente qualitativa.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-10
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Avalie os resultados de duas estimações de modelos de regressão para dados de contagem (Poisson e binomial negativo (BNeg)), conforme figura a seguir, e assinale a alternativa CORRETA:

[imagem: imagens/176796_1_10_0.jpg]

- a) Entre as duas estimações, a mais adequada é a Poisson, por apresentar um menor valor do beta da variável staff.
- b) Entre as duas estimações, a mais adequada é a binomial negativa, por apresentar um valor mais alto de Log-lik.
- c) As duas estimações apresentam a mesma capacidade preditiva, já que ambas levaram em consideração o mesmo tamanho da amostra (N = 298).
- d) Entre as duas estimações, a mais adequada é a Poisson, por apresentar um maior valor de intercepto.

**Resposta certa:** b) Entre as duas estimações, a mais adequada é a binomial negativa, por apresentar um valor mais alto de Log-lik.

**Explicação:** A resposta é o binomial negativo, por ter log-likelihood mais alto. Entre modelos estimados por máxima verossimilhança com a mesma amostra, o de LL maior tem melhor aderência aos dados. O tamanho da amostra igual não torna a capacidade preditiva igual, e comparar betas ou interceptos não mede qualidade de ajuste.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 811

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-2
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Em qual das alternativas a seguir há indícios de existência de equidispersão nos dados de determinada variável dependente considerada em um modelo de regressão para dados de contagem?

[imagem: imagens/176796_1_2_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** a) a)

**Explicação:** Equidispersão é média aproximadamente igual à variância. Só a a) tem isso: média 2,47 e variância 2,47. Nas outras a variância é bem maior, como em b) 1,73 e 101,73, c) 7,47 e 297,46 e d) 6,34 e 728,21, indicando superdispersão.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-3
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Em relação aos modelos inflacionados de zeros, considere as seguintes afirmações:

I) São considerados uma combinação entre um modelo para dados de contagem e um modelo para dados binários, já que são utilizados para investigar as razões que levam a determinada quantidade de ocorrências (contagens) de um fenômeno, bem como as razões que levam (ou não) à ocorrência propriamente dita deste fenômeno, independentemente da quantidade de contagens observadas.

II) Enquanto um modelo Poisson inflacionado de zeros é estimado a partir da combinação de uma distribuição Bernoulli com uma distribuição Poisson, um modelo binomial negativo inflacionado de zeros é estimado por meio da combinação de uma distribuição Bernoulli com uma distribuição Poisson-Gama.

Assinale a alternativa CORRETA:
Em relação aos modelos inflacionados de zeros, considere as seguintes afirmações:
I) São considerados uma combinação entre um modelo para dados de contagem e um modelo para dados binários, já que são utilizados para investigar as razões que levam a determinada quantidade de ocorrências (contagens) de um fenômeno, bem como as razões que levam (ou não) à ocorrência propriamente dita deste fenômeno, independentemente da quantidade de contagens observadas.
II) Enquanto um modelo Poisson inflacionado de zeros é estimado a partir da combinação de uma distribuição Bernoulli com uma distribuição Poisson, um modelo binomial negativo inflacionado de zeros é estimado por meio da combinação de uma distribuição Bernoulli com uma distribuição Poisson-Gama.
Assinale a alternativa CORRETA:

- a) Apenas a segunda afirmação está correta.
- b) Apenas a primeira afirmação está correta.
- c) As duas afirmações estão corretas.
- d) As duas afirmações estão incorretas.

**Resposta certa:** c) As duas afirmações estão corretas.

**Explicação:** A resposta é que as duas afirmações estão corretas. O modelo inflacionado de zeros combina um modelo de contagem com um binário, que explica se o fenômeno ocorre ou não. O ZIP junta Bernoulli e Poisson, enquanto o ZINB junta Bernoulli e Poisson-Gama.

**Fonte:** Aula de modelos inflacionados de zeros, pág. 18; Manual de Análise de Dados (Fávero), pág. 801

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-4
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Assinale a alternativa que mostra um histograma de determinada variável com indícios de existência de superdispersão e inflação de zeros nos dados.

[imagem: imagens/176796_1_4_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** c) c)

**Explicação:** O histograma c) tem uma barra enorme no zero (cerca de 240 observações) e cauda longa à direita, chegando perto de 150, o que mostra superdispersão com inflação de zeros. Em a) e b) a distribuição é mais comportada, e d) é praticamente binário, com só valores 0 e 1.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-5
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Em relação especificamente aos modelos de regressão Poisson inflacionados de zeros, podemos afirmar que:

I) A probabilidade p de ocorrência de nenhuma contagem para dada observação i (i = 1, 2, ..., n, em que n é o tamanho da amostra), ou seja, p(Yi = 0), é calculada levando-se em consideração a soma de um componente dicotômico com um componente de contagem.

II) Deve-se definir a probabilidade plogit de não ocorrer nenhuma contagem devido exclusivamente ao componente dicotômico, bem como a probabilidade p de ocorrência de determinada contagem m (m = 1, 2, ...), ou seja, p(Yi = m), que segue a própria expressão da probabilidade da distribuição Poisson, multiplicada por (1 – plogit).

III) São úteis apenas para variáveis preditoras qualitativas.

Assinale a alternativa CORRETA:
Em relação especificamente aos modelos de regressão Poisson inflacionados de zeros, podemos afirmar que:
I) A probabilidade p de ocorrência de nenhuma contagem para dada observação i (i = 1, 2, ..., n, em que n é o tamanho da amostra), ou seja, p(Yi = 0), é calculada levando-se em consideração a soma de um componente dicotômico com um componente de contagem.
II) Deve-se definir a probabilidade plogit de não ocorrer nenhuma contagem devido exclusivamente ao componente dicotômico, bem como a probabilidade p de ocorrência de determinada contagem m (m = 1, 2, ...), ou seja, p(Yi = m), que segue a própria expressão da probabilidade da distribuição Poisson, multiplicada por (1 – plogit).
III) São úteis apenas para variáveis preditoras qualitativas.
Assinale a alternativa CORRETA:

- a) Apenas as afirmações I e III estão corretas.
- b) Apenas as afirmações I e II estão corretas.
- c) Apenas as afirmações II e III estão corretas.
- d) Todas as afirmações estão corretas.

**Resposta certa:** b) Apenas as afirmações I e II estão corretas.

**Explicação:** A resposta é somente I e II. No ZIP o zero vem de dois processos, o componente binário e o de contagem, e p(Y = m) para m >= 1 é a Poisson multiplicada por (1 – plogit). A III é falsa: o modelo trata excesso de zeros na variável dependente e nada restringe os preditores a serem qualitativos.

**Fonte:** Aula de modelos inflacionados de zeros, pág. 20; Manual de Análise de Dados (Fávero), pág. 801

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-6
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Com o intuito de se estudar e prever a quantidade de violações de trânsito (variável dependente violations) na cidade de Nova York por parte de membros dos corpos diplomáticos dos países pertencentes às Nações Unidas, foi estimado um modelo de regressão binomial negativo, considerando, como variáveis preditoras, a quantidade de membros no corpo diplomático em cada país (variável staff), o índice de corrupção de cada país (variável corruption) e o fato de haver ou não enforcement legal quanto à obrigatoriedade de se pagar a multa em caso de violação (variável binária post: ‘yes’ = há obrigatoriedade do pagamento; ‘no’ = não há obrigatoriedade do pagamento). Os outputs do referido modelo, obtidos no Python, encontram-se na imagem seguir.

Pergunta-se: qual a equação do modelo de regressão binomial negativo que deverá ser utilizada para fins preditivos? O subscrito i refere-se à linha (row) do dataset.
Com o intuito de se estudar e prever a quantidade de violações de trânsito (variável dependente violations) na cidade de Nova York por parte de membros dos corpos diplomáticos dos países pertencentes às Nações Unidas, foi estimado um modelo de regressão binomial negativo, considerando, como variáveis preditoras, a quantidade de membros no corpo diplomático em cada país (variável staff), o índice de corrupção de cada país (variável corruption) e o fato de haver ou não enforcement legal quanto à obrigatoriedade de se pagar a multa em caso de violação (variável binária post: ‘yes’ = há obrigatoriedade do pagamento; ‘no’ = não há obrigatoriedade do pagamento). Os outputs do referido modelo, obtidos no Python, encontram-se na imagem seguir.
Pergunta-se: qual a equação do modelo de regressão binomial negativo que deverá ser utilizada para fins preditivos? O subscrito i refere-se à linha (row) do dataset.

[imagem: imagens/176796_1_6_0.jpg]

- a) a)
- b) b)
- c) c)
- d) d)

**Resposta certa:** a) a)

**Explicação:** Na alternativa a) o lado esquerdo é ln(violations), e o lado direito usa os coeficientes da tabela: 1,9469 do intercepto, 0,0400 de staff, -4,2746 de post[T.yes] e 0,4527 de corruption. No binomial negativo o logaritmo do valor esperado é linear nos preditores, então a previsão é violations = e elevado a essa soma. A b) e a d) ignoram a função de ligação log e a d) ainda omite o intercepto.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-7
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

A definição sobre a existência ou não de uma quantidade excessiva de zeros na variável dependente Y de um modelo de regressão para dados de contagem é verificada por meio de um teste específico, conhecido por:

- a) Teste de Vuong.
- b) Teste de Cameron e Trivedi.
- c) Teste de Erlang.
- d) Teste de Lambert.

**Resposta certa:** a) Teste de Vuong.

**Explicação:** A resposta é o teste de Vuong. Ele avalia se há quantidade excessiva de zeros na variável dependente e é o primeiro resultado a olhar nos modelos inflacionados de zeros. Cameron e Trivedi servem para superdispersão e Lambert é o autor do modelo ZIP.

**Fonte:** Aula de modelos inflacionados de zeros, pág. 19; Manual de Análise de Dados (Fávero), pág. 801

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-8
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

São modelos supervisionados de machine learning para dados de contagem:

- a) Regressão Poisson, Regressão Binomial Negativa, Regressão Poisson com Inflação de Zeros e Regressão Binomial Negativa com Inflação de Zeros.
- b) Regressão Logística Binária e Regressão Logística Multinomial.
- c) Regressão Gaussiana e Regressão estimada por OLS.
- d) Análise de Clusters e Análise Fatorial por Componentes Principais.

**Resposta certa:** a) Regressão Poisson, Regressão Binomial Negativa, Regressão Poisson com Inflação de Zeros e Regressão Binomial Negativa com Inflação de Zeros.

**Explicação:** A resposta é Poisson, binomial negativa, Poisson com inflação de zeros e binomial negativa com inflação de zeros. Esses são os modelos de contagem vistos. Logística binária e multinomial são para variável qualitativa, OLS e gaussiana são para variável contínua, e cluster e fatorial são técnicas não supervisionadas.

**Fonte:** Aula de modelos inflacionados de zeros, pág. 21; Manual de Análise de Dados (Fávero), pág. 803

**Situação:** explicação conferida com o material das aulas

---

### Questão 176796-1-9
Área 3 · Supervised Machine Learning: Modelos para Dados de Contagem II

Analise o seguinte resultado de um teste para verificação de existência de superdispersão na variável dependente de determinado modelo (Teste de Cameron e Trivedi) e assinale a alternativa CORRETA:

[imagem: imagens/176796_1_9_0.jpg]

- a) Verifica-se a existência de superdispersão nos dados da variável dependente.
- b) Verifica-se a existência de dispersão sub-reversa nos dados das variáveis preditoras.
- c) Verifica-se a existência de equidispersão nos dados da variável dependente.
- d) A partir deste output não se pode concluir nada a respeito de uma eventual superdispersão nos dados da variável dependente, já que (lambda – theta = delta).

**Resposta certa:** c) Verifica-se a existência de equidispersão nos dados da variável dependente.

**Explicação:** O valor-p do teste de Cameron e Trivedi na figura é 0,7516, bem acima de 0,05. Não se rejeita a hipótese nula de que o parâmetro do modelo auxiliar é zero, então não há evidência de superdispersão e a variância é igual à média, ou seja, equidispersão na variável dependente.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---


# Área 4: Árvores, redes e deep learning

## Deep Learning e Inteligência Artificial I

### Questão 203399-1-1
Área 4 · Deep Learning e Inteligência Artificial I

Considere os conceitos apresentados em aula e assinale a alternativa que apresenta uma estratégia de codificação de variáveis categóricas.

- a) Sequential binary encoding
- b) One-hot encoding
- c) Categorical gradient encoding
- d) Polynomial label encoding

**Resposta certa:** b) One-hot encoding

**Explicação:** A resposta é one-hot encoding. Ele transforma cada categoria numa coluna binária, com 1 na coluna da categoria da observação e 0 nas demais, assim a rede não enxerga uma ordem falsa entre categorias. As outras opções não são estratégias de codificação usuais.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 203399-1-10
Área 4 · Deep Learning e Inteligência Artificial I

Na Aula 2, o ciclo de aprendizado foi construído a partir de um dataset de objetos próximos da Terra (NEOs), em que cada linha é uma amostra e cada coluna é uma feature. O primeiro passo consistiu em isolar uma amostra — o objeto NEO-114, com diâmetro 0.42, velocidade 18.3, distância mínima 3.1 e magnitude 21.4 — e convertê-la em um vetor de entrada x (tensor rank-1), enquanto o rótulo y indicava se o objeto era perigoso.

Sobre essa etapa de preparação da entrada, marque a única alternativa CORRETA:
Na Aula 2, o ciclo de aprendizado foi construído a partir de um dataset de objetos próximos da Terra (NEOs), em que cada linha é uma amostra e cada coluna é uma feature. O primeiro passo consistiu em isolar uma amostra — o objeto NEO-114, com diâmetro 0.42, velocidade 18.3, distância mínima 3.1 e magnitude 21.4 — e convertê-la em um vetor de entrada x (tensor rank-1), enquanto o rótulo y indicava se o objeto era perigoso.
Sobre essa etapa de preparação da entrada, marque a única alternativa CORRETA:

- a) O vetor x é formado pelas features numéricas da amostra e o rótulo y é o alvo a ser previsto e não compõe a entrada da rede.
- b) O rótulo y deve ser concatenado ao vetor x, de modo que a rede disponha da informação necessária para realizar o aprendizado supervisionado.
- c) O vetor de entrada precisa conter o dataset completo, pois o neurônio só é capaz de calcular sua saída após processar todas as amostras simultaneamente.
- d) Cada coluna do dataset corresponde a uma amostra e cada linha a uma feature, de modo que o vetor de entrada é formado por uma coluna inteira.

**Resposta certa:** a) O vetor x é formado pelas features numéricas da amostra e o rótulo y é o alvo a ser previsto e não compõe a entrada da rede.

**Explicação:** A resposta é que x leva as features e y é o alvo fora da entrada. Cada linha é uma amostra e cada coluna uma feature, então o NEO-114 vira o vetor [0.42, 18.3, 3.1, 21.4]. O rótulo y é o que a rede tenta prever e é comparado com a saída para calcular o erro, por isso não entra em x.

**Fonte:** Data Science do Zero, pág. 312

**Situação:** explicação conferida com o material das aulas

---

### Questão 203399-1-2
Área 4 · Deep Learning e Inteligência Artificial I

Um único neurônio artificial combina cada feature do vetor de entrada com um peso, adiciona um bias e submete o resultado a uma função de ativação não linear. No exemplo da aula, essa operação foi escrita como z = w·x + b, seguida de y = σ(z). O que representa o σ nesse contexto?

- a) A taxa de aprendizado do modelo.
- b) A função sigmoide.
- c) A função de custo (loss) usada no treinamento.
- d) O vetor de pesos ajustado durante o treinamento.

**Resposta certa:** b) A função sigmoide.

**Explicação:** A resposta é a função sigmoide. O neurônio faz a soma ponderada z = w·x + b e aplica a sigmoide, y = 1 / (1 + e^-z), que é uma versão suave da função degrau e deixa a saída entre 0 e 1. A taxa de aprendizado, a loss e o vetor de pesos têm outros símbolos (eta, J, w).

**Fonte:** Data Science do Zero, pág. 308

**Situação:** explicação conferida com o material das aulas

---

### Questão 203399-1-3
Área 4 · Deep Learning e Inteligência Artificial I

A regra de atualização dos pesos no Gradient Descent foi apresentada como Wpróximo = Watual − η · ∇J(W). O que representa o ∇J(W)?

- a) Representa o vetor de derivadas parciais da loss em relação a cada peso, com indicação da direção de maior crescimento do erro.
- b) Representa a função que mede o erro do modelo em relação aos rótulos observados.
- c) Representa a taxa de aprendizagem, que define o tamanho relativo do passo dado a cada atualização.
- d) Representa o conjunto de parâmetros treináveis que são ajustados a cada iteração.

**Resposta certa:** a) Representa o vetor de derivadas parciais da loss em relação a cada peso, com indicação da direção de maior crescimento do erro.

**Explicação:** A resposta é o vetor de derivadas parciais da loss em relação a cada peso. O gradiente aponta para onde o erro cresce mais rápido, por isso o gradiente descendente subtrai eta vezes ∇J: anda no sentido contrário. J é a função de erro e eta é a taxa de aprendizagem.

**Fonte:** Data Science do Zero, pág. 143

**Situação:** explicação conferida com o material das aulas

---

### Questão 203399-1-4
Área 4 · Deep Learning e Inteligência Artificial I

O treinamento moderno de redes neurais raramente usa o dataset inteiro ou uma única amostra por atualização: adota-se uma técnica, em que os pesos são atualizados a cada lote de amostras. Que técnica é essa?

- a) Batch Gradient Descent
- b) Mini-batch Stochastic Gradient Descent
- c) Learning Rate Decay
- d) Backpropagation

**Resposta certa:** b) Mini-batch Stochastic Gradient Descent

**Explicação:** A resposta é mini-batch stochastic gradient descent. O batch usa o dataset inteiro em cada atualização e o estocástico puro usa uma amostra; o mini-batch fica no meio, atualizando os pesos a cada lote pequeno. Learning rate decay mexe no passo e backpropagation calcula os gradientes.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 203399-1-5
Área 4 · Deep Learning e Inteligência Artificial I

Um cientista de dados precisa escalonar os pixels de um conjunto de imagens (valores originais entre 0 e 255) para um intervalo fixo entre 0 e 1, antes de alimentá-los a uma rede neural. Qual técnica de escalonamento é a mais apropriada para esse cenário?

- a) Normalizer
- b) MaxAbsScaler
- c) StandardScaler
- d) MinMaxScaler

**Resposta certa:** d) MinMaxScaler

**Explicação:** A resposta é o MinMaxScaler. Ele aplica (x – min) / (max – min) e leva os valores para o intervalo fixo [0, 1], que é o que se quer com pixels de 0 a 255 (na prática, dividir por 255). O StandardScaler gera média zero e desvio um, sem limite fixo, e o Normalizer trabalha por linha.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 203399-1-6
Área 4 · Deep Learning e Inteligência Artificial I

Uma variável de renda familiar apresenta forte assimetria à direita e alguns valores extremos (outliers) muito acima da mediana. Considerando os métodos de escalonamento apresentados em aula, marque a única alternativa CORRETA:

- a) O Normalizer é a melhor opção, pois padroniza cada feature subtraindo sua média e dividindo pelo desvio-padrão.
- b) O RobustScaler é a escolha mais adequada, pois escalona os dados pela mediana e pelo intervalo interquartil (IQR), sendo resistente a outliers.
- c) O MaxAbsScaler é o mais indicado, pois remove os outliers do conjunto antes de realizar o escalonamento.
- d) O MinMaxScaler é a escolha ideal nesse caso, pois reescala os dados para o intervalo [0,1] e é insensível à presença de outliers.

**Resposta certa:** b) O RobustScaler é a escolha mais adequada, pois escalona os dados pela mediana e pelo intervalo interquartil (IQR), sendo resistente a outliers.

**Explicação:** A resposta é o RobustScaler. Ele subtrai a mediana e divide pelo intervalo interquartil (Q3 – Q1), medidas pouco afetadas por valores extremos, então serve para renda com assimetria e outliers. O MinMaxScaler é sensível a outliers e o StandardScaler é que usa média e desvio, não o Normalizer.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 203399-1-7
Área 4 · Deep Learning e Inteligência Artificial I

Durante a aula, as funções de perda baseadas em entropia cruzada foram apresentadas em três variantes. Quais são elas?

- a) L1 Loss, L2 Loss e KL Divergence
- b) BCE (Binary Cross Entropy), MSE (Mean Squared Error) e Hinge Loss
- c) BCE (Binary Cross Entropy), CCE (Categorical Cross Entropy) e SCCE (Sparse Categorical Cross Entropy)
- d) MAE (Mean Absolute Error), MSE (Mean Squared Error) e RMSE (Root Mean Squared Error)

**Resposta certa:** c) BCE (Binary Cross Entropy), CCE (Categorical Cross Entropy) e SCCE (Sparse Categorical Cross Entropy)

**Explicação:** A resposta é BCE, CCE e SCCE. A BCE é para classificação binária, a CCE para várias classes com rótulos em one-hot e a SCCE para várias classes com rótulos inteiros. MSE, MAE e RMSE são perdas de regressão, e Hinge e KL são de outras famílias.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 203399-1-8
Área 4 · Deep Learning e Inteligência Artificial I

O backpropagation é um algoritmo utilizado no treinamento de redes neurais. Qual é a finalidade geral do backpropagation?

- a) Ajustar os pesos da rede neural para reduzir o erro do modelo
- b) Armazenar os resultados do modelo em um banco de dados
- c) Definir o tipo de dado que será utilizado como entrada do modelo
- d) Criar gráficos para visualização dos dados de treinamento

**Resposta certa:** a) Ajustar os pesos da rede neural para reduzir o erro do modelo

**Explicação:** A resposta é ajustar os pesos para reduzir o erro. O backpropagation calcula o erro nas saídas, propaga esse erro de volta para as camadas ocultas e usa os gradientes para corrigir os pesos de cada camada. Não guarda resultados nem cria gráficos, e não define o tipo de entrada.

**Fonte:** Data Science do Zero, pág. 312

**Situação:** explicação conferida com o material das aulas

---

### Questão 203399-1-9
Área 4 · Deep Learning e Inteligência Artificial I

Uma matriz TF-IDF, usada para representar textos, é tipicamente esparsa. Ao aplicar um escalonamento a esses dados, é essencial preservar essa esparsidade. Qual técnica de escalonamento, discutida em aula, atende a esse requisito?

- a) MinMaxScaler
- b) Normalizer
- c) StandardScaler
- d) MaxAbsScaler

**Resposta certa:** d) MaxAbsScaler

**Explicação:** A resposta é MaxAbsScaler, que divide cada feature pelo seu valor absoluto máximo e como não subtrai média, os zeros continuam zeros e a matriz esparsa permanece esparsa. MinMaxScaler e StandardScaler deslocam os dados e destroem a esparsidade.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** ambígua: o Normalizer também preserva esparsidade, pois escala por linha sem centralizar; o gabarito segue o que a aula teria dito, e esse trecho não veio na busca.

---

## Introdução ao Deep Learning e Inteligência Artificial

### Questão 202887-1-1
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

Uma diferença significativa entre o Deep Learning (DL) e os algoritmos tradicionais de Machine Learning (ML Tradicional) reside na forma como as features (características) dos dados são tratadas. Modelos de DL, especialmente redes neurais profundas, são conhecidos por sua capacidade de aprender representações hierárquicas dos dados automaticamente, extraindo features de baixo a alto nível. Em contraste, muitos algoritmos de ML Tradicional dependem fortemente de um processo prévio chamado feature engineering, onde especialistas definem e extraem manualmente as características mais relevantes para o modelo. Considerando essas abordagens distintas, analise as seguintes afirmações:

I. Em Deep Learning, a necessidade de engenharia de features manual é significativamente reduzida ou eliminada, pois a própria rede neural já é automaticamente inicializada com features relevantes diretamente dos dados brutos antes do treinamento.

II. Algoritmos como Regressão Logística ou Decision Trees, exemplos de ML Tradicional, frequentemente exigem que o desenvolvedor selecione, transforme e crie features manualmente para que o modelo atinja um bom desempenho, um processo que demanda conhecimento do domínio e experimentação.

III. A capacidade das redes neurais profundas de aprender features hierárquicas significa que as primeiras camadas geralmente aprendem padrões simples (como bordas ou texturas em imagens), enquanto camadas mais profundas combinam esses padrões para detectar conceitos mais complexos (como objetos ou rostos).

Quais afirmações estão corretas?
Uma diferença significativa entre o Deep Learning (DL) e os algoritmos tradicionais de Machine Learning (ML Tradicional) reside na forma como as features (características) dos dados são tratadas. Modelos de DL, especialmente redes neurais profundas, são conhecidos por sua capacidade de aprender representações hierárquicas dos dados automaticamente, extraindo features de baixo a alto nível. Em contraste, muitos algoritmos de ML Tradicional dependem fortemente de um processo prévio chamado feature engineering, onde especialistas definem e extraem manualmente as características mais relevantes para o modelo. Considerando essas abordagens distintas, analise as seguintes afirmações:

I. Em Deep Learning, a necessidade de engenharia de features manual é significativamente reduzida ou eliminada, pois a própria rede neural já é automaticamente inicializada com features relevantes diretamente dos dados brutos antes do treinamento.
II. Algoritmos como Regressão Logística ou Decision Trees, exemplos de ML Tradicional, frequentemente exigem que o desenvolvedor selecione, transforme e crie features manualmente para que o modelo atinja um bom desempenho, um processo que demanda conhecimento do domínio e experimentação.
III. A capacidade das redes neurais profundas de aprender features hierárquicas significa que as primeiras camadas geralmente aprendem padrões simples (como bordas ou texturas em imagens), enquanto camadas mais profundas combinam esses padrões para detectar conceitos mais complexos (como objetos ou rostos).

Quais afirmações estão corretas?

- a) Apenas II
- b) I e III, apenas
- c) I e II, apenas
- d) II e III, apenas

**Resposta certa:** d) II e III, apenas

**Explicação:** A resposta é II e III, apenas. Regressão logística e árvores de decisão costumam pedir seleção e criação manual de features, com conhecimento do domínio. Nas redes profundas as primeiras camadas aprendem padrões simples e as seguintes os combinam em conceitos complexos. A I erra ao dizer que a rede já vem inicializada com features relevantes: elas são aprendidas durante o treino.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 202887-1-10
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

As funções de ativação são componentes essenciais nas redes neurais. Assinale a alternativa que apresenta o papel principal dessas funções nas redes neurais.

- a) As funções de ativação são responsáveis por introduzir a não-linearidade necessária para que os modelos possam aprender relações complexas nos dados.
- b) As funções de ativação são responsáveis por armazenar permanentemente os dados de treinamento utilizados pela rede neural.
- c) As funções de ativação são responsáveis por traduzir o código-fonte da rede neural de uma linguagem de programação para outra.
- d) As funções de ativação têm como principal finalidade estabelecer a conexão física entre os neurônios artificiais e o hardware do computador.

**Resposta certa:** a) As funções de ativação são responsáveis por introduzir a não-linearidade necessária para que os modelos possam aprender relações complexas nos dados.

**Explicação:** A resposta é a primeira porque, sem uma função de ativação não linear, empilhar camadas equivale a uma única transformação linear. A ativação (sigmoide, ReLU, tanh) introduz a não linearidade que deixa a rede aprender relações complexas. Guardar dados, traduzir código ou ligar neurônios ao hardware não têm nada a ver com ela.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 202887-1-2
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

Os dados de entrada de uma rede neural precisam ser representados como um objeto denominado Tensor, que possui, entre outros atributos, o rank. Assinale a alternativa CORRETA sobre o conceito de rank de um Tensor.

- a) Rank corresponde ao número total de valores armazenados no Tensor, independentemente da quantidade de eixos.
- b) Rank corresponde ao maior valor numérico encontrado entre os elementos armazenados no Tensor.
- c) Rank corresponde à soma dos valores de todos os elementos armazenados no Tensor.
- d) Rank corresponde ao número de eixos do Tensor. Em Python, utilizando bibliotecas como NumPy, TensorFlow ou PyTorch, esse conceito está relacionado ao atributo ndim.

**Resposta certa:** d) Rank corresponde ao número de eixos do Tensor. Em Python, utilizando bibliotecas como NumPy, TensorFlow ou PyTorch, esse conceito está relacionado ao atributo ndim.

**Explicação:** A resposta é o número de eixos do tensor. Escalar tem rank 0, vetor rank 1, matriz rank 2, e assim por diante; em NumPy, TensorFlow e PyTorch isso aparece como ndim. Contar valores armazenados dá o tamanho (size), não o rank.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 202887-1-3
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre a definição de Inteligência Artificial:

- a) É um campo da ciência da computação que busca desenvolver sistemas capazes de realizar tarefas que normalmente exigem inteligência humana, como aprendizado, raciocínio e tomada de decisão.
- b) É uma sub-área da estatística cujo único objetivo é prever valores numéricos futuros com base em dados históricos.
- c) É um conjunto de técnicas de programação que automatiza exclusivamente tarefas repetitivas em sistemas empresariais.
- d) É um ramo da engenharia elétrica voltado à construção de robôs físicos capazes de interagir com o ambiente.

**Resposta certa:** a) É um campo da ciência da computação que busca desenvolver sistemas capazes de realizar tarefas que normalmente exigem inteligência humana, como aprendizado, raciocínio e tomada de decisão.

**Explicação:** A resposta é a primeira porque IA é o campo da computação que busca sistemas capazes de fazer o que normalmente exigiria inteligência humana, como aprender, raciocinar e decidir. As outras alternativas encolhem demais o conceito: IA não se limita a prever números, a automatizar rotinas ou a construir robôs físicos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 202887-1-4
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

No paradigma tradicional de programação, o desenvolvedor escreve explicitamente todas as regras e a lógica necessárias para que um programa execute uma tarefa. Por outro lado, no paradigma de aprendizado de máquina, o objetivo é fazer com que o sistema aprenda essas regras a partir de dados, sem que cada passo seja codificado manualmente pelo programador para abranger todas as possibilidades. Considerando essa distinção fundamental, analise as seguintes afirmações:

I. No aprendizado de máquina supervisionado, as regras que governam a solução de um problema são inferidas a partir dos dados de entrada e saída fornecidos durante o treinamento, em vez de serem codificadas diretamente pelo programador.

II. O paradigma tradicional de programação é inerentemente mais flexível e eficaz para lidar com tarefas complexas como reconhecimento de imagem ou tradução automática, pois o programador tem controle total sobre o código.

III. Um programa tradicional executará uma tarefa exatamente como foi programado, enquanto um modelo de aprendizado de máquina pode apresentar comportamentos ou "regras" que não foram explicitamente previstas pelo desenvolvedor, mas emergiram do processo de aprendizado com os dados.

Quais afirmações estão corretas?
No paradigma tradicional de programação, o desenvolvedor escreve explicitamente todas as regras e a lógica necessárias para que um programa execute uma tarefa. Por outro lado, no paradigma de aprendizado de máquina, o objetivo é fazer com que o sistema aprenda essas regras a partir de dados, sem que cada passo seja codificado manualmente pelo programador para abranger todas as possibilidades. Considerando essa distinção fundamental, analise as seguintes afirmações:

I. No aprendizado de máquina supervisionado, as regras que governam a solução de um problema são inferidas a partir dos dados de entrada e saída fornecidos durante o treinamento, em vez de serem codificadas diretamente pelo programador.
II. O paradigma tradicional de programação é inerentemente mais flexível e eficaz para lidar com tarefas complexas como reconhecimento de imagem ou tradução automática, pois o programador tem controle total sobre o código.
III. Um programa tradicional executará uma tarefa exatamente como foi programado, enquanto um modelo de aprendizado de máquina pode apresentar comportamentos ou "regras" que não foram explicitamente previstas pelo desenvolvedor, mas emergiram do processo de aprendizado com os dados.

Quais afirmações estão corretas?

- a) Apenas III
- b) I e III, apenas
- c) Apenas I
- d) II e III, apenas

**Resposta certa:** b) I e III, apenas

**Explicação:** A resposta é I e III. No aprendizado supervisionado o modelo infere as regras a partir de pares entrada e saída, em vez de serem escritas pelo programador, e por isso pode produzir comportamentos que ninguém previu. A II inverte a lógica: justamente em tarefas como reconhecer imagem ou traduzir texto é inviável escrever todas as regras à mão, e é aí que o aprendizado de máquina leva vantagem.

**Fonte:** Data Science do Zero, pág. 205

**Situação:** explicação conferida com o material das aulas

---

### Questão 202887-1-5
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

O Deep Learning abrange diferentes especializações, todas apoiadas em uma base comum de fundamentos (função, tensor, neurônio, camada, ativação, treino). Associe cada especialização da Coluna A a um exemplo típico de aplicação na Coluna B.

Coluna A
1. Visão Computacional
2. Processamento de Linguagem Natural (NLP)
3. Sinais Temporais
4. Tarefas Multimodais / Agentes

Coluna B
( ) Previsão de séries temporais financeiras ou sensoriais ao longo do tempo
( ) Reconhecimento e classificação de objetos em imagens
( ) Tradução automática e geração de texto
( ) Um agente que combina texto, imagem e ação para executar tarefas de forma autônoma

Marque a alternativa que apresenta a sequência correta de associação, de cima para baixo:
O Deep Learning abrange diferentes especializações, todas apoiadas em uma base comum de fundamentos (função, tensor, neurônio, camada, ativação, treino). Associe cada especialização da Coluna A a um exemplo típico de aplicação na Coluna B.

Coluna A
1. Visão Computacional
2. Processamento de Linguagem Natural (NLP)
3. Sinais Temporais
4. Tarefas Multimodais / Agentes
Coluna B
( ) Previsão de séries temporais financeiras ou sensoriais ao longo do tempo
( ) Reconhecimento e classificação de objetos em imagens
( ) Tradução automática e geração de texto
( ) Um agente que combina texto, imagem e ação para executar tarefas de forma autônoma

Marque a alternativa que apresenta a sequência correta de associação, de cima para baixo:

- a) 4 – 1 – 2 – 3
- b) 3 – 1 – 2 – 4
- c) 1 – 2 – 4 – 3
- d) 1 – 3 – 4 – 2

**Resposta certa:** b) 3 – 1 – 2 – 4

**Explicação:** A resposta é 3, 1, 2, 4. Sinais temporais ficam com a previsão de séries ao longo do tempo, visão computacional com reconhecer e classificar objetos em imagens, NLP com tradução e geração de texto, e tarefas multimodais ou agentes com o agente que junta texto, imagem e ação. Basta casar cada área com o tipo de dado que ela trata.

**Fonte:** Data Science do Zero, pág. 339

**Situação:** explicação conferida com o material das aulas

---

### Questão 202887-1-6
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

A linha do tempo do Deep Learning apresenta marcos históricos que consolidaram o campo ao longo de décadas. Associe cada marco da Coluna A ao período em que ocorreu, na Coluna B.

Coluna A
1. Perceptron (Rosenblatt)
2. Popularização do algoritmo de Backpropagation
3. AlexNet vence a competição ImageNet
4. AlphaGo derrota um campeão mundial de Go

Coluna B
( ) 2012
( ) 1958
( ) 2016
( ) 1974–1986

Marque a alternativa que apresenta a sequência correta de associação, de cima para baixo:
A linha do tempo do Deep Learning apresenta marcos históricos que consolidaram o campo ao longo de décadas. Associe cada marco da Coluna A ao período em que ocorreu, na Coluna B.

Coluna A
1. Perceptron (Rosenblatt)
2. Popularização do algoritmo de Backpropagation
3. AlexNet vence a competição ImageNet
4. AlphaGo derrota um campeão mundial de Go
Coluna B
( ) 2012
( ) 1958
( ) 2016
( ) 1974–1986

Marque a alternativa que apresenta a sequência correta de associação, de cima para baixo:

- a) 3 – 1 – 4 – 2
- b) 1 – 3 – 2 – 4
- c) 3 – 2 – 4 – 1
- d) 4 – 1 – 3 – 2

**Resposta certa:** a) 3 – 1 – 4 – 2

**Explicação:** A resposta é 3, 1, 4, 2. O Perceptron de Rosenblatt é de 1958, o backpropagation se popularizou entre 1974 e 1986, a AlexNet venceu o ImageNet em 2012 e o AlphaGo derrotou um campeão de Go em 2016. A coluna B está embaralhada, então a ordem lida de cima para baixo (2012, 1958, 2016, 1974 a 1986) vira 3, 1, 4, 2.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 202887-1-7
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

Os dados de entrada de uma rede neural precisam ser representados como um objeto denominado Tensor, que possui, entre outros atributos, o shape. Assinale a alternativa CORRETA sobre o shape.

- a) shape representa apenas a quantidade total de elementos armazenados no Tensor, sem considerar a organização dos dados em eixos.
- b) shape representa a soma de todos os valores armazenados no Tensor.
- c) shape representa o maior valor numérico encontrado entre os elementos do Tensor.
- d) shape representa o número de dimensões por eixo do Tensor.

**Resposta certa:** d) shape representa o número de dimensões por eixo do Tensor.

**Explicação:** A resposta é a última porque o shape de um tensor descreve o tamanho de cada eixo, por exemplo (32, 28, 28) para um lote de 32 imagens de 28 por 28. Ele diz como os dados estão organizados, não quantos elementos há no total, nem a soma ou o maior valor dos elementos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 202887-1-8
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

O neurônio Perceptron, proposto por Frank Rosenblatt em seu artigo de 1958 ("The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain") (https://doi.org/10.1037/h0042519), é considerado um marco fundamental no desenvolvimento inicial das redes neurais. Ele foi um dos primeiros modelos computacionais inspirados no funcionamento neuronal, projetado para tarefas de classificação. Com base neste modelo pioneiro, analise as seguintes afirmações:

I. O Perceptron calcula uma soma ponderada das suas entradas (combinação linear) e aplica uma função degrau (threshold) para produzir uma saída binária, sendo capaz de aprender a classificar corretamente conjuntos de dados que são linearmente separáveis.

II. Devido à sua estrutura simples, o Perceptron original de Rosenblatt é capaz de resolver problemas de classificação complexos, incluindo o problema do OU-Exclusivo (XOR), que envolve padrões não-lineares.

III. O modelo MLP utiliza funções de ativação contínuas, como a Sigmoide ou ReLU, para permitir o ajuste fino dos pesos através de métodos baseados em gradiente, como o backpropagation.

Quais afirmações estão corretas?
O neurônio Perceptron, proposto por Frank Rosenblatt em seu artigo de 1958 ("The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain") (https://doi.org/10.1037/h0042519), é considerado um marco fundamental no desenvolvimento inicial das redes neurais. Ele foi um dos primeiros modelos computacionais inspirados no funcionamento neuronal, projetado para tarefas de classificação. Com base neste modelo pioneiro, analise as seguintes afirmações:

I. O Perceptron calcula uma soma ponderada das suas entradas (combinação linear) e aplica uma função degrau (threshold) para produzir uma saída binária, sendo capaz de aprender a classificar corretamente conjuntos de dados que são linearmente separáveis.
II. Devido à sua estrutura simples, o Perceptron original de Rosenblatt é capaz de resolver problemas de classificação complexos, incluindo o problema do OU-Exclusivo (XOR), que envolve padrões não-lineares.
III. O modelo MLP utiliza funções de ativação contínuas, como a Sigmoide ou ReLU, para permitir o ajuste fino dos pesos através de métodos baseados em gradiente, como o backpropagation.

Quais afirmações estão corretas?

- a) II e III, apenas
- b) I e III, apenas
- c) Apenas I
- d) I e II, apenas

**Resposta certa:** b) I e III, apenas

**Explicação:** A resposta é I e III. O perceptron soma as entradas com pesos, aplica uma função degrau e só aprende o que é linearmente separável. O MLP troca o degrau por ativações contínuas e derivadas (sigmoide, ReLU), o que permite ajustar pesos por gradiente com backpropagation. A II está errada: um perceptron sozinho não resolve o XOR.

**Fonte:** Data Science do Zero, pág. 306

**Situação:** explicação conferida com o material das aulas

---

### Questão 202887-1-9
Área 4 · Introdução ao Deep Learning e Inteligência Artificial

Deep Learning é um subcampo do Aprendizado de Máquina que ganhou destaque por sua capacidade de lidar com tarefas complexas, especialmente em áreas como visão computacional e processamento de linguagem natural.

Qual das seguintes afirmações melhor descreve uma característica fundamental e distintiva do Deep Learning em comparação com redes neurais artificiais mais rasas, ou algoritmos clássicos de Machine Learning?
Deep Learning é um subcampo do Aprendizado de Máquina que ganhou destaque por sua capacidade de lidar com tarefas complexas, especialmente em áreas como visão computacional e processamento de linguagem natural.
Qual das seguintes afirmações melhor descreve uma característica fundamental e distintiva do Deep Learning em comparação com redes neurais artificiais mais rasas, ou algoritmos clássicos de Machine Learning?

- a) A principal característica do Deep Learning é a sua capacidade de funcionar apenas com dados não estruturados, como imagens e texto, sendo inadequado para dados tabulares.
- b) Deep Learning utiliza redes neurais artificiais com múltiplas camadas ocultas ("profundas") que aprendem representações hierárquicas dos dados, permitindo que o modelo descubra padrões complexos de forma mais automática.
- c) Deep Learning elimina completamente a necessidade de pré-processamento de dados, pois as redes profundas, sendo aproximadores universais, conseguem lidar diretamente com dados brutos.
- d) O diferencial do Deep Learning está no uso exclusivo de algoritmos de otimização como o SGD, algo que não é empregado em outras formas de Aprendizado de Máquina.

**Resposta certa:** b) Deep Learning utiliza redes neurais artificiais com múltiplas camadas ocultas ("profundas") que aprendem representações hierárquicas dos dados, permitindo que o modelo descubra padrões complexos de forma mais automática.

**Explicação:** A resposta é a segunda porque o traço do Deep Learning é empilhar várias camadas ocultas que aprendem representações hierárquicas, descobrindo padrões complexos com menos engenharia manual de atributos. As outras exageram: DL também roda em dados tabulares, não elimina todo pré-processamento e usa otimizadores como o SGD que também aparecem em modelos clássicos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Árvores, Redes e Ensemble Models I

### Questão 199610-1-1
Área 4 · Árvores, Redes e Ensemble Models I

Um cientista de dados treinou uma árvore de decisão e obteve 100% de acurácia no conjunto de treinamento e 72% de acurácia no conjunto de teste. Esse comportamento indica que:

- a) O modelo generaliza bem para dados novos, pois teve alto desempenho no treino.
- b) O modelo apresenta overfitting, pois memorizou os dados de treino e teve queda de desempenho em dados não vistos.
- c) O modelo apresenta underfitting, pois não aprendeu suficientemente os padrões dos dados.
- d) O resultado é ideal, pois a acurácia no teste está próxima da acurácia no treino.

**Resposta certa:** b) O modelo apresenta overfitting, pois memorizou os dados de treino e teve queda de desempenho em dados não vistos.

**Explicação:** A resposta é overfitting. Acerto de 100% no treino contra 72% no teste mostra que a árvore decorou os exemplos, ruído incluído, e não generaliza para dados novos. Underfitting apareceria como desempenho ruim já no treino, e a distância entre as duas acurácias é justamente o sinal de alerta, não de resultado ideal.

**Fonte:** Aula de Árvores de Decisão, pág. 36

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-10
Área 4 · Árvores, Redes e Ensemble Models I

Ao construir uma árvore de decisão utilizando o scikit-learn, um analista percebeu overfitting no modelo inicial. Como estratégia para reduzir esse problema, ele decide ajustar hiperparâmetros. Qual hiperparâmetro tem impacto direto no controle da profundidade da árvore?

- a) test_size
- b) random_state
- c) max_depth
- d) criterion

**Resposta certa:** c) max_depth

**Explicação:** A resposta é max_depth, que define a profundidade máxima da árvore, e limitá-la reduz a memorização dos dados de treino. O test_size só define a proporção da base separada para teste, o random_state fixa a semente de aleatoriedade e o criterion escolhe o critério de divisão dos nós.

**Fonte:** Aula de Árvores de Decisão, pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-2
Área 4 · Árvores, Redes e Ensemble Models I

Em um problema de classificação, qual das alternativas abaixo apresenta a métrica de avaliação que mede a proporção de positivos reais corretamente identificados pelo modelo?

- a) Especificidade (specificity).
- b) Acurácia (accuracy).
- c) Sensibilidade (recall).
- d) Precisão (precision).

**Resposta certa:** c) Sensibilidade (recall).

**Explicação:** A resposta é sensibilidade (recall), que mede quantos dos positivos reais o modelo encontrou: VP / (VP + FN). A precisão é a mais tentadora, mas olha para os positivos previstos: VP / (VP + FP). A acurácia conta todos os acertos e a especificidade fala dos negativos reais.

**Fonte:** Aula de Árvores de Decisão, pág. 22

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-3
Área 4 · Árvores, Redes e Ensemble Models I

Em um problema de análise de crédito, o modelo classifica clientes como "bons pagadores" ou "inadimplentes". Ao avaliar a matriz de confusão, o banco identifica um caso em que o modelo previu "bom pagador" para um cliente que, na realidade, se tornou inadimplente. Esse caso corresponde a:

- a) Verdadeiro negativo (VN), pois o modelo acertou a classificação do cliente.
- b) Falso positivo (FP), pois o modelo previu inadimplência para quem honraria o pagamento.
- c) Verdadeiro positivo (VP), pois o modelo identificou corretamente um mau pagador.
- d) Falso negativo (FN), pois o modelo previu bom pagador para um cliente que não pagou.

**Resposta certa:** d) Falso negativo (FN), pois o modelo previu bom pagador para um cliente que não pagou.

**Explicação:** A resposta é falso negativo. Aqui o evento positivo é a inadimplência: o modelo disse "bom pagador" (negativo) e o cliente não pagou, ou seja, o crédito foi concedido a quem deu calote. O falso positivo seria o contrário, prever inadimplência para quem pagaria.

**Fonte:** Aula de Árvores de Decisão, pág. 25

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-4
Área 4 · Árvores, Redes e Ensemble Models I

Considere as seguintes afirmações sobre desvantagens e limitações das árvores de decisão:

I — Árvores muito profundas tendem a memorizar os dados de treino, aumentando o risco de overfitting.

II — Alterações no conjunto de treinamento são incapazes de gerar árvores diferentes, o que indica alta estabilidade do modelo.

III — Árvores de decisão apresentam dificuldade em extrapolar tendências para valores fora da faixa observada no conjunto de treinamento.

Assinale a alternativa correta:
Considere as seguintes afirmações sobre desvantagens e limitações das árvores de decisão:
I — Árvores muito profundas tendem a memorizar os dados de treino, aumentando o risco de overfitting.
II — Alterações no conjunto de treinamento são incapazes de gerar árvores diferentes, o que indica alta estabilidade do modelo.
III — Árvores de decisão apresentam dificuldade em extrapolar tendências para valores fora da faixa observada no conjunto de treinamento.
Assinale a alternativa correta:

- a) Somente os enunciados I e III estão corretos.
- b) Somente o enunciado I está correto.
- c) Todos os enunciados estão corretos.
- d) Somente os enunciados II e III estão corretos.

**Resposta certa:** a) Somente os enunciados I e III estão corretos.

**Explicação:** A resposta é I e III. Árvores profundas decoram o treino, e elas extrapolam mal, porque as folhas só devolvem valores vistos no treinamento. A II inverte o fato: pequenas alterações nos dados podem gerar uma árvore completamente diferente, o que indica instabilidade, não estabilidade.

**Fonte:** Aula de Árvores de Decisão, pág. 35

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-5
Área 4 · Árvores, Redes e Ensemble Models I

Considere as seguintes afirmações sobre métricas de avaliação em problemas de regressão:

I — O RMSE, por ser a raiz quadrada do MSE, é expresso na mesma unidade da variável de interesse, o que facilita sua interpretação prática.

II — O MAE é ideal quando se quer uma métrica robusta a outliers e fácil de se interpretar.

III — O R² representa a proporção da variância da variável-alvo que é explicada pelo modelo.

Assinale a alternativa correta:
Considere as seguintes afirmações sobre métricas de avaliação em problemas de regressão:
I — O RMSE, por ser a raiz quadrada do MSE, é expresso na mesma unidade da variável de interesse, o que facilita sua interpretação prática.
II — O MAE é ideal quando se quer uma métrica robusta a outliers e fácil de se interpretar.
III — O R² representa a proporção da variância da variável-alvo que é explicada pelo modelo.
Assinale a alternativa correta:

- a) Somente o enunciado I está correto.
- b) Somente os enunciados II e III estão corretos.
- c) Todos os enunciados estão corretos.
- d) Somente os enunciados I e III estão corretos.

**Resposta certa:** c) Todos os enunciados estão corretos.

**Explicação:** A resposta é todos corretos. O RMSE é a raiz do MSE e volta para a unidade da variável original. O MAE é a média dos erros absolutos, pouco afetado por outliers e fácil de ler. O R² é a proporção da variância da variável-alvo explicada pelo modelo.

**Fonte:** Aula de Árvores de Decisão, pág. 29

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-6
Área 4 · Árvores, Redes e Ensemble Models I

Qual das alternativas abaixo apresenta possíveis causas de overfitting?

- a) Poda excessiva da árvore e limitação rigorosa da profundidade máxima permitida.
- b) Grande quantidade de dados de treinamento e uso de validação cruzada durante o ajuste dos hiperparâmetros.
- c) Árvore muito profunda, muitas variáveis ou atributos irrelevantes e pouca quantidade de dados de treinamento.
- d) Árvore muito rasa, poucas variáveis relevantes e alta regularização aplicada ao modelo.

**Resposta certa:** c) Árvore muito profunda, muitas variáveis ou atributos irrelevantes e pouca quantidade de dados de treinamento.

**Explicação:** A resposta é a que junta árvore muito profunda, muitos atributos irrelevantes e pouco dado de treino. Todos esses fatores deixam o modelo livre para memorizar ruído. As demais alternativas descrevem o oposto: poda, regularização alta, árvore rasa e muito dado com validação cruzada combatem o overfitting.

**Fonte:** Aula de Árvores de Decisão, pág. 36

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-7
Área 4 · Árvores, Redes e Ensemble Models I

Em uma árvore de decisão, a estrutura é composta por diferentes tipos de nós, cada um com um papel específico no processo de tomada de decisão. Sobre esses elementos, assinale a alternativa correta:

- a) O nó raiz é o ponto de partida da árvore e representa o conjunto de dados completo, enquanto as folhas contêm os resultados finais da predição.
- b) Os nós internos são responsáveis por armazenar apenas os dados originais, sem realizar qualquer tipo de divisão.
- c) As folhas realizam perguntas sobre as variáveis dos dados, e os nós internos armazenam os resultados finais.
- d) O nó raiz representa o resultado final da classificação, enquanto as folhas contêm o conjunto de dados completo.

**Resposta certa:** a) O nó raiz é o ponto de partida da árvore e representa o conjunto de dados completo, enquanto as folhas contêm os resultados finais da predição.

**Explicação:** A resposta é a primeira. O nó raiz é o ponto de partida e representa o conjunto de dados completo, os nós internos fazem as perguntas sobre as variáveis e as folhas trazem o resultado final da predição. As outras alternativas trocam esses papéis.

**Fonte:** Aula de Árvores de Decisão, pág. 7

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-8
Área 4 · Árvores, Redes e Ensemble Models I

Considere as seguintes afirmações sobre as vantagens das árvores de decisão:

I — As árvores de decisão são consideradas modelos "white box", pois suas previsões podem ser explicadas por uma sequência clara de regras e condições.

II — As árvores de decisão exigem normalização e padronização obrigatórias de todas as variáveis numéricas antes do treinamento.

III — As árvores de decisão podem trabalhar simultaneamente com variáveis numéricas e categóricas, o que amplia sua aplicação em diferentes problemas de negócio.

Assinale a alternativa correta:
Considere as seguintes afirmações sobre as vantagens das árvores de decisão:
I — As árvores de decisão são consideradas modelos "white box", pois suas previsões podem ser explicadas por uma sequência clara de regras e condições.
II — As árvores de decisão exigem normalização e padronização obrigatórias de todas as variáveis numéricas antes do treinamento.
III — As árvores de decisão podem trabalhar simultaneamente com variáveis numéricas e categóricas, o que amplia sua aplicação em diferentes problemas de negócio.
Assinale a alternativa correta:

- a) Somente o enunciado I está correto.
- b) Os enunciados I e II estão corretos.
- c) Somente o enunciado III está correto.
- d) Os enunciados I e III estão corretos.

**Resposta certa:** d) Os enunciados I e III estão corretos.

**Explicação:** A resposta é I e III. A árvore é um modelo white box, pois cada previsão se explica por uma cadeia de regras, e aceita variáveis numéricas e categóricas ao mesmo tempo. A II está errada: justamente uma vantagem da árvore é exigir pouco tratamento, em geral sem precisar normalizar ou padronizar as variáveis.

**Fonte:** Aula de Árvores de Decisão, pág. 9

**Situação:** explicação conferida com o material das aulas

---

### Questão 199610-1-9
Área 4 · Árvores, Redes e Ensemble Models I

Um cientista de dados deseja construir um modelo baseado em árvores de decisão para prever o preço de venda de imóveis, uma variável contínua expressa em reais. Considerando o tipo de problema descrito, assinale a alternativa correta:

- a) Deve ser utilizada uma árvore de regressão, cuja folha retorna a média dos valores dos dados que caíram nela.
- b) Deve ser utilizada uma árvore de classificação, cuja folha retorna a classe mais frequente entre as observações.
- c) Deve ser utilizada uma árvore de classificação, pois o preço é uma variável mensurável.
- d) Árvores de decisão não são adequadas para problemas que envolvem variáveis numéricas contínuas.

**Resposta certa:** a) Deve ser utilizada uma árvore de regressão, cuja folha retorna a média dos valores dos dados que caíram nela.

**Explicação:** A resposta é árvore de regressão. O preço do imóvel é um número contínuo, e nesse caso a folha devolve a média dos valores que caíram nela. A árvore de classificação serve para prever categorias e a folha devolve a classe mais frequente. Árvores lidam bem com alvo contínuo, então a última alternativa também está errada.

**Fonte:** Aula de Árvores de Decisão, pág. 13

**Situação:** explicação conferida com o material das aulas

---

## Árvores, Redes e Ensemble Models II

### Questão 200689-1-1
Área 4 · Árvores, Redes e Ensemble Models II

O bagging (Bootstrap Aggregating) é uma técnica de ensemble baseada em amostragem com reposição. Sobre esse método, assinale a alternativa correta:

- a) O bagging tem como principal objetivo aumentar o viés dos modelos base, deixando-os mais simples.
- b) Cada modelo base é treinado com o conjunto de dados completo, sem qualquer reamostragem.
- c) Os modelos base são treinados de forma sequencial, sendo que cada modelo corrige os erros do anterior.
- d) A amostragem com reposição gera, em média, amostras contendo cerca de 63% dos registros originais distintos, o que gera diversidade entre os modelos.

**Resposta certa:** d) A amostragem com reposição gera, em média, amostras contendo cerca de 63% dos registros originais distintos, o que gera diversidade entre os modelos.

**Explicação:** A resposta é a última. No bootstrap cada amostra tem o tamanho da base original e é sorteada com reposição, então cerca de 63% dos registros aparecem ao menos uma vez e o resto se repete. Essa variação entre amostras dá diversidade aos modelos. Treino sequencial corrigindo erros é o boosting, e o bagging mira reduzir variância, não aumentar viés.

**Fonte:** Aula de Ensemble Models, pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-10
Área 4 · Árvores, Redes e Ensemble Models II

Considere os conceitos discutidos em aula sobre bagging e assinale a alternativa correta:

- a) Treina vários modelos do mesmo tipo de forma sequencial, em que cada modelo é ajustado para corrigir os erros cometidos pelo modelo anterior.
- b) Treina vários modelos do mesmo tipo usando diferentes amostras do conjunto de treinamento. A combinação das previsões reduz a variabilidade e melhora a generalização.
- c) Treina um único modelo complexo repetidamente sobre o conjunto de treinamento completo, ajustando seus pesos a cada iteração para reduzir o erro.
- d) Treina vários modelos de tipos diferentes (por exemplo, árvore de decisão, regressão logística e SVM) e seleciona apenas o modelo com melhor desempenho individual.

**Resposta certa:** b) Treina vários modelos do mesmo tipo usando diferentes amostras do conjunto de treinamento. A combinação das previsões reduz a variabilidade e melhora a generalização.

**Explicação:** A resposta é a segunda: o bagging treina vários modelos do mesmo tipo, cada um em uma amostra diferente do treino, e combina as previsões, o que reduz a variabilidade e melhora a generalização. A primeira descreve o boosting, que é sequencial. A quarta lembra o stacking, que usa modelos de tipos diferentes com um meta-modelo.

**Fonte:** Aula de Ensemble Models, pág. 14

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-2
Área 4 · Árvores, Redes e Ensemble Models II

Considere as seguintes afirmações sobre o método de boosting:

I — Os modelos são treinados de forma sequencial, e cada novo modelo busca corrigir os erros cometidos pelos modelos anteriores.

II — Assim como no bagging, os modelos do boosting são treinados de forma totalmente independente e em paralelo.

III — A previsão final é obtida por meio de uma combinação ponderada das previsões dos modelos da sequência.

Assinale a alternativa correta:
Considere as seguintes afirmações sobre o método de boosting:
I — Os modelos são treinados de forma sequencial, e cada novo modelo busca corrigir os erros cometidos pelos modelos anteriores.
II — Assim como no bagging, os modelos do boosting são treinados de forma totalmente independente e em paralelo.
III — A previsão final é obtida por meio de uma combinação ponderada das previsões dos modelos da sequência.
Assinale a alternativa correta:

- a) Somente os enunciados II e III estão corretos.
- b) Somente os enunciados I e III estão corretos.
- c) Somente o enunciado I está correto.
- d) Todos os enunciados estão corretos.

**Resposta certa:** b) Somente os enunciados I e III estão corretos.

**Explicação:** A resposta é I e III. No boosting os modelos são treinados em sequência, cada um atacando os erros do anterior, e a previsão final é a soma ponderada de todos. A II está errada: treino independente e em paralelo é característica do bagging, não do boosting.

**Fonte:** Aula de Ensemble Models, pág. 14 e pág. 27

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-3
Área 4 · Árvores, Redes e Ensemble Models II

Considere os conceitos discutidos em aula sobre as diferentes estratégias de ensemble learning e assinale a alternativa INCORRETA:

- a) Stacking combina as previsões de modelos de tipos diferentes por meio de um modelo combinador (meta-modelo), que aprende a melhor forma de ponderar essas previsões.
- b) Boosting treina modelos de forma sequencial e dependente, atribuindo maior peso às observações que foram classificadas incorretamente pelos modelos anteriores.
- c) Bagging combina modelos treinados em paralelo sobre diferentes amostras bootstrap do conjunto de treinamento, com o objetivo principal de reduzir a variância.
- d) Voting/Averaging é a forma mais sofisticada de ensemble. Treina modelos de forma sequencial, em que cada novo modelo busca corrigir os erros dos anteriores.

**Resposta certa:** d) Voting/Averaging é a forma mais sofisticada de ensemble. Treina modelos de forma sequencial, em que cada novo modelo busca corrigir os erros dos anteriores.

**Explicação:** A questão pede a INCORRETA, e é a última. Voting/Averaging é a forma mais simples de ensemble, com modelos treinados de forma independente e previsões combinadas por votação ou média. Treinar em sequência corrigindo os erros do anterior é o boosting. As outras três descrevem bem stacking, boosting e bagging.

**Fonte:** Aula de Ensemble Models, pág. 14

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-4
Área 4 · Árvores, Redes e Ensemble Models II

O trade-off viés-variância é um conceito central para entender o comportamento de modelos de aprendizado de máquina. Sobre esse tema, assinale a alternativa correta:

- a) Modelos com alto viés são excessivamente flexíveis e tendem a sofrer overfitting, ajustando-se ao ruído dos dados.
- b) Modelos com alto viés normalmente são muito simplistas para capturar os padrões verdadeiros dos dados, ajustando mal tanto os dados de treino quanto os de teste.
- c) Modelos com alta variância produzem previsões consistentes, mas frequentemente distantes do valor real.
- d) É possível reduzir simultaneamente o viés e a variância a zero por meio da escolha adequada de hiperparâmetros.

**Resposta certa:** b) Modelos com alto viés normalmente são muito simplistas para capturar os padrões verdadeiros dos dados, ajustando mal tanto os dados de treino quanto os de teste.

**Explicação:** A resposta é a segunda: alto viés significa modelo simplista demais, que ajusta mal tanto o treino quanto o teste. A primeira troca os conceitos, já que modelo flexível demais e sujeito a overfitting tem alta variância. A terceira também erra, pois previsões consistentes mas fora do alvo são o alto viés. E não dá para zerar viés e variância ao mesmo tempo.

**Fonte:** Aula de Ensemble Models, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-5
Área 4 · Árvores, Redes e Ensemble Models II

Em um ensemble de classificação utilizando a estratégia de Hard Voting, três modelos foram treinados para diagnosticar se um paciente possui uma doença. As previsões individuais foram:

Modelo A: Doença
Modelo B: Saudável
Modelo C: Doença

Considerando o funcionamento do Hard Voting, assinale a alternativa correta:
Em um ensemble de classificação utilizando a estratégia de Hard Voting, três modelos foram treinados para diagnosticar se um paciente possui uma doença. As previsões individuais foram:
Considerando o funcionamento do Hard Voting, assinale a alternativa correta:

- a) O resultado final não pode ser determinado, pois o Hard Voting exige unanimidade entre os modelos.
- b) O resultado final será "Doença", pois essa foi a classe mais votada entre os modelos (2 votos contra 1).
- c) O resultado final será "Saudável", pois a previsão do Modelo B é considerada mais confiável.
- d) O resultado final será a média das probabilidades previstas por cada modelo, resultando em "Saudável".

**Resposta certa:** b) O resultado final será "Doença", pois essa foi a classe mais votada entre os modelos (2 votos contra 1).

**Explicação:** A resposta é Doença. No hard voting cada modelo vota em uma classe e vence a mais votada: Doença recebe 2 votos (A e C) contra 1 de Saudável (B). Não exige unanimidade, nenhum voto pesa mais que outro e a média de probabilidades é o soft voting, outra estratégia.

**Fonte:** Aula de Ensemble Models, pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-6
Área 4 · Árvores, Redes e Ensemble Models II

Assinale a alternativa que corresponde a um hiperparâmetro do Random Forest:

- a) n_estimators
- b) sklearn
- c) alpha_regularization
- d) kernel

**Resposta certa:** a) n_estimators

**Explicação:** A resposta é n_estimators, que define o número de árvores da floresta. Sklearn é a biblioteca, não um hiperparâmetro. Alpha_regularization não é parâmetro da Random Forest, e kernel pertence a modelos como o SVM.

**Fonte:** Aula de Ensemble Models, pág. 38

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-7
Área 4 · Árvores, Redes e Ensemble Models II

Durante o treinamento com bagging, algumas observações do conjunto original nunca são sorteadas para compor uma determinada amostra bootstrap. Esses registros são chamados de out-of-bag (OOB). Qual é a utilidade prática desses registros?

- a) São utilizados obrigatoriamente para reforçar o treinamento, sendo incluídos em uma segunda rodada.
- b) Servem como um conjunto de validação embutido para o modelo em questão, pois não foram vistos por ele durante o treinamento.
- c) São descartados definitivamente, pois representam ruído e não podem ser aproveitados.
- d) Representam apenas registros duplicados e não contribuem para a avaliação do modelo.

**Resposta certa:** b) Servem como um conjunto de validação embutido para o modelo em questão, pois não foram vistos por ele durante o treinamento.

**Explicação:** A resposta é a segunda. Os registros out-of-bag ficam de fora da amostra bootstrap de cada modelo (cerca de 37%) e portanto nunca foram vistos por ele no treino, o que permite usá-los como conjunto de teste embutido, sem separar dados de validação. Não são ruído nem duplicatas.

**Fonte:** Aula de Ensemble Models, pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-8
Área 4 · Árvores, Redes e Ensemble Models II

Considere os assuntos discutidos em aula e assinale a alternativa que apresenta corretamente limitações de uma árvore de decisão individual:

- a) Alta estabilidade nas previsões, mesmo diante de pequenas alterações na base de dados.
- b) Baixo viés e baixa variância, o que a torna equivalente a um ensemble em termos de robustez.
- c) Necessidade de grandes volumes de dados para evitar overfitting, sendo imune a variações na amostra de treinamento.
- d) Tendência a overfitting e alta sensibilidade a pequenas mudanças nos dados de treinamento.

**Resposta certa:** d) Tendência a overfitting e alta sensibilidade a pequenas mudanças nos dados de treinamento.

**Explicação:** A resposta é a última. Uma árvore individual tende a crescer demais e decorar o treino (overfitting) e pequenas mudanças na base podem gerar uma árvore completamente diferente. Por isso ela costuma ter baixo viés e alta variância, bem longe da estabilidade de um ensemble.

**Fonte:** Aula de Ensemble Models, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 200689-1-9
Área 4 · Árvores, Redes e Ensemble Models II

Em um problema de regressão para prever o preço de um imóvel, três modelos foram treinados e geraram as seguintes previsões:

Modelo A: R$ 320 mil
Modelo B: R$ 290 mil
Modelo C: R$ 350 mil

Utilizando a estratégia de ensemble por Averaging, qual será o valor final previsto?
Em um problema de regressão para prever o preço de um imóvel, três modelos foram treinados e geraram as seguintes previsões:
Utilizando a estratégia de ensemble por Averaging, qual será o valor final previsto?

- a) R$ 320 mil, pois o Averaging seleciona a previsão do modelo mediano entre os três valores.
- b) R$ 350 mil, pois o Averaging seleciona sempre a maior previsão entre os modelos.
- c) R$ 320 mil, pois o Averaging calcula a média aritmética das previsões numéricas dos modelos.
- d) R$ 290 mil, pois o Averaging seleciona a previsão do modelo com menor valor, por segurança.

**Resposta certa:** c) R$ 320 mil, pois o Averaging calcula a média aritmética das previsões numéricas dos modelos.

**Explicação:** A resposta é R$ 320 mil. No averaging de regressão a previsão final é a média aritmética das previsões: (320 + 290 + 350) / 3 = 960 / 3 = 320. Coincide com o valor do modelo A, mas não é escolha do modelo mediano, é a média.

**Fonte:** Aula de Ensemble Models, pág. 19

**Situação:** explicação conferida com o material das aulas

---

## Árvores, Redes e Ensemble Models III

### Questão 201533-1-1
Área 4 · Árvores, Redes e Ensemble Models III

Assinale a alternativa que apresenta a diferença central entre a Regularização L1 e a Regularização L2 no XGBoost.

- a) Diferente da L1, a Regularização L2 normalmente não zera contribuições, mas suaviza os valores, tornando o modelo mais estável e menos sensível a variações ou padrões extremos nos dados de treino.
- b) Diferente da L2, a Regularização L1 normalmente não zera contribuições, mas distribui o peso igualmente entre todas as variáveis, evitando que qualquer atributo seja descartado do modelo.
- c) Tanto a Regularização L1 quanto a L2 têm como objetivo exclusivo acelerar o tempo de treinamento do modelo, não exercendo nenhuma influência sobre os pesos atribuídos às variáveis.
- d) A Regularização L1 penaliza apenas os erros de classificação em variáveis contínuas, enquanto a L2 penaliza exclusivamente os erros em variáveis categóricas.

**Resposta certa:** a) Diferente da L1, a Regularização L2 normalmente não zera contribuições, mas suaviza os valores, tornando o modelo mais estável e menos sensível a variações ou padrões extremos nos dados de treino.

**Explicação:** A resposta é a primeira. A L1 (reg_alpha) penaliza a soma dos valores absolutos dos pesos das folhas e pode zerar contribuições, e a L2 (reg_lambda) penaliza pesos grandes mas em geral só os suaviza, sem zerar, deixando o modelo mais estável. A segunda alternativa inverte isso, e nenhuma delas existe para acelerar o treino.

**Fonte:** Aula de Ensemble Models, pág. 43

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-10
Área 4 · Árvores, Redes e Ensemble Models III

A biblioteca XGBoost tornou-se uma das ferramentas mais utilizadas em problemas de aprendizado supervisionado. Sobre suas características, assinale a alternativa CORRETA:

- a) O XGBoost é uma implementação otimizada de gradient boosting que traz regularização L1 e L2 embutidas, ajudando a controlar a complexidade das árvores e proteger contra overfitting.
- b) O XGBoost é uma variação do KNN aplicada a problemas de classificação binária.
- c) O XGBoost não permite ajuste de hiperparâmetros e utiliza apenas os valores padrão internos da biblioteca.
- d) O XGBoost implementa exclusivamente o algoritmo de bagging, treinando árvores de forma paralela e independente.

**Resposta certa:** a) O XGBoost é uma implementação otimizada de gradient boosting que traz regularização L1 e L2 embutidas, ajudando a controlar a complexidade das árvores e proteger contra overfitting.

**Explicação:** A resposta é a primeira: o XGBoost é uma biblioteca otimizada de gradient boosting, com regularização L1 e L2 embutida para controlar a complexidade das árvores. Não é uma variação do KNN, aceita ajuste de hiperparâmetros (learning_rate, max_depth e outros) e usa boosting sequencial, não bagging.

**Fonte:** Aula de Ensemble Models, pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-2
Área 4 · Árvores, Redes e Ensemble Models III

Qual das alternativas abaixo representa uma característica que diferencia o XGBoost de uma Random Forest tradicional?

- a) O XGBoost incorpora termos de regularização em sua função objetivo, o que ajuda a controlar o overfitting durante o treinamento sequencial das árvores.
- b) O XGBoost treina suas árvores de forma independente e em paralelo, enquanto a Random Forest treina de forma sequencial.
- c) O XGBoost só pode ser aplicado a problemas de regressão, enquanto a Random Forest é utilizada exclusivamente em problemas de classificação.
- d) O XGBoost não permite o uso de hiperparâmetros, enquanto a Random Forest exige ajuste manual extensivo.

**Resposta certa:** a) O XGBoost incorpora termos de regularização em sua função objetivo, o que ajuda a controlar o overfitting durante o treinamento sequencial das árvores.

**Explicação:** A resposta é a primeira: a função objetivo do XGBoost soma o erro nos dados a uma penalidade de complexidade (regularização L1 e L2), que ajuda a controlar o overfitting. O treino paralelo e independente é da Random Forest, enquanto o XGBoost é sequencial. Ele serve para regressão e classificação e tem muitos hiperparâmetros.

**Fonte:** Aula de Ensemble Models, pág. 43 e pág. 47

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-3
Área 4 · Árvores, Redes e Ensemble Models III

No XGBoost, o hiperparâmetro learning_rate controla o "tamanho do passo" em cada rodada de boosting. Sobre esse hiperparâmetro, assinale a alternativa CORRETA:

- a) O learning_rate controla o peso da contribuição de cada nova árvore para a previsão final; valores baixos exigem mais árvores para atingir bom desempenho, enquanto valores altos podem fazer o modelo oscilar sem convergir.
- b) Um learning_rate muito alto sempre garante convergência mais rápida e melhor desempenho final.
- c) O learning_rate deve ser fixado obrigatoriamente em 1,0 para garantir a estabilidade do treinamento.
- d) O learning_rate não influencia a contribuição de cada árvore ao modelo final, apenas o número de estimadores.

**Resposta certa:** a) O learning_rate controla o peso da contribuição de cada nova árvore para a previsão final; valores baixos exigem mais árvores para atingir bom desempenho, enquanto valores altos podem fazer o modelo oscilar sem convergir.

**Explicação:** A resposta é a primeira. O learning_rate define o peso de cada nova árvore na previsão final: valor baixo faz ajustes pequenos e cuidadosos (mais lento, pedindo mais árvores), e valor alto dá passos grandes que podem passar do ponto e ficar oscilando. Não existe garantia de que valor alto converge mais rápido, nem obrigação de usar 1,0.

**Fonte:** Aula de Ensemble Models, pág. 44 e pág. 29

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-4
Área 4 · Árvores, Redes e Ensemble Models III

Considere as seguintes afirmações sobre os hiperparâmetros de amostragem do XGBoost:

I — O hiperparâmetro subsample define a fração das observações de treinamento utilizada para construir cada árvore; valores menores que 1 introduzem aleatoriedade e podem ajudar a controlar o overfitting.

II — O hiperparâmetro colsample_bytree define o número máximo de níveis de cada árvore, aumentando a diversidade entre as árvores do ensemble.

III — Valores muito baixos de colsample_bytree são sempre benéficos, pois quanto menor a fração de variáveis, melhor será o desempenho do modelo.

Assinale a alternativa CORRETA:
Considere as seguintes afirmações sobre os hiperparâmetros de amostragem do XGBoost:
I — O hiperparâmetro subsample define a fração das observações de treinamento utilizada para construir cada árvore; valores menores que 1 introduzem aleatoriedade e podem ajudar a controlar o overfitting.
II — O hiperparâmetro colsample_bytree define o número máximo de níveis de cada árvore, aumentando a diversidade entre as árvores do ensemble.
III — Valores muito baixos de colsample_bytree são sempre benéficos, pois quanto menor a fração de variáveis, melhor será o desempenho do modelo.
Assinale a alternativa CORRETA:

- a) Somente os enunciados I e III estão corretos.
- b) Somente o enunciado I está correto.
- c) Todos os enunciados estão corretos.
- d) Somente o enunciado III está correto.

**Resposta certa:** b) Somente o enunciado I está correto.

**Explicação:** A resposta é só a I. O subsample é a fração das observações usada em cada árvore e valores menores que 1 colocam aleatoriedade e ajudam contra overfitting. A II erra porque colsample_bytree é a fração das variáveis por árvore, não a profundidade, que é o max_depth. A III erra porque valores muito baixos podem impedir o modelo de encontrar variáveis importantes.

**Fonte:** Aula de Ensemble Models, pág. 44

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-5
Área 4 · Árvores, Redes e Ensemble Models III

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre o hiperparâmetro colsample_bytree do XGBoost:

- a) O colsample_bytree define a taxa de aprendizado aplicada aos pesos das árvores a cada iteração do boosting.
- b) O colsample_bytree define a fração das observações do conjunto de treino selecionadas aleatoriamente para construir cada árvore.
- c) O colsample_bytree define o número máximo de níveis de profundidade que cada árvore pode atingir durante o treinamento.
- d) O colsample_bytree define a fração das variáveis selecionadas aleatoriamente para construir cada árvore.

**Resposta certa:** d) O colsample_bytree define a fração das variáveis selecionadas aleatoriamente para construir cada árvore.

**Explicação:** A resposta é a última: colsample_bytree define a fração das variáveis sorteadas para construir cada árvore, o que aumenta a diversidade entre elas. A fração das observações é o subsample, a profundidade máxima é o max_depth e a taxa de aprendizado é o learning_rate.

**Fonte:** Aula de Ensemble Models, pág. 44

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-6
Área 4 · Árvores, Redes e Ensemble Models III

Considere as seguintes afirmações sobre as regularizações L1 e L2 do XGBoost:

I — A regularização L1 penaliza a soma dos valores absolutos dos pesos das folhas e pode zerar algumas contribuições, funcionando como um mecanismo de simplificação do modelo.

II — A regularização L2 penaliza pesos muito grandes, tipicamente suavizando seus valores em vez de zerá-los, tornando o modelo mais estável.

III — As regularizações L1 e L2 aumentam a complexidade das árvores, favorecendo o overfitting nos dados de treinamento.

Assinale a alternativa CORRETA:
Considere as seguintes afirmações sobre as regularizações L1 e L2 do XGBoost:
I — A regularização L1 penaliza a soma dos valores absolutos dos pesos das folhas e pode zerar algumas contribuições, funcionando como um mecanismo de simplificação do modelo.
II — A regularização L2 penaliza pesos muito grandes, tipicamente suavizando seus valores em vez de zerá-los, tornando o modelo mais estável.
III — As regularizações L1 e L2 aumentam a complexidade das árvores, favorecendo o overfitting nos dados de treinamento.
Assinale a alternativa CORRETA:

- a) Somente o enunciado I está correto.
- b) Todos os enunciados estão corretos.
- c) Somente os enunciados I e II estão corretos.
- d) Somente os enunciados II e III estão corretos.

**Resposta certa:** c) Somente os enunciados I e II estão corretos.

**Explicação:** A resposta é I e II. A L1 penaliza a soma dos valores absolutos dos pesos das folhas e pode zerar contribuições, simplificando o modelo, e a L2 penaliza pesos grandes suavizando-os e deixando o modelo mais estável. A III está errada: a regularização funciona como freio na complexidade, então reduz o overfitting em vez de favorecê-lo.

**Fonte:** Aula de Ensemble Models, pág. 43

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-7
Área 4 · Árvores, Redes e Ensemble Models III

As últimas aulas sobre Árvores e Ensemble Models apresentaram uma progressão didática entre modelos: Decision Tree → Random Forest → XGBoost. Sobre essa sequência, assinale a alternativa CORRETA:

- a) A Decision Tree tende a apresentar desempenho igual ou superior ao dos ensembles em bases de dados mais complexas, sendo por isso utilizada como referência de melhor desempenho.
- b) O XGBoost reduz a necessidade de ajuste de hiperparâmetros em relação à Random Forest, pois já incorpora regularização interna que dispensa a etapa de validação do modelo.
- c) A Decision Tree serve como baseline por sua simplicidade e explicabilidade; a Random Forest, por combinar várias árvores independentes, oferece maior robustez e generalização com pouco ajuste; e o XGBoost busca máxima performance por meio de boosting regularizado, exigindo maior esforço de tuning.
- d) A Random Forest utiliza o mesmo princípio sequencial do XGBoost, treinando árvores para corrigir os erros das árvores anteriores.

**Resposta certa:** c) A Decision Tree serve como baseline por sua simplicidade e explicabilidade; a Random Forest, por combinar várias árvores independentes, oferece maior robustez e generalização com pouco ajuste; e o XGBoost busca máxima performance por meio de boosting regularizado, exigindo maior esforço de tuning.

**Explicação:** A resposta é a terceira, que reflete a progressão da aula: a árvore de decisão como baseline simples e explicável, a Random Forest com robustez sem muito tuning e o XGBoost buscando alta performance, com mais esforço de ajuste. A Random Forest treina árvores em paralelo e independentes, não em sequência, e regularização interna não dispensa a validação.

**Fonte:** Aula de Ensemble Models, pág. 48 e pág. 47

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-8
Área 4 · Árvores, Redes e Ensemble Models III

Um cientista de dados observa que as árvores do seu modelo XGBoost estão muito parecidas entre si, pois praticamente todas utilizam as mesmas variáveis consideradas mais importantes, reduzindo a diversidade do ensemble. Qual ajuste de hiperparâmetro é mais indicado para lidar com esse problema?

- a) Aumentar o n_estimators, adicionando mais árvores em sequência para compensar a repetição de padrões.
- b) Reduzir o max_depth, limitando a profundidade das árvores para evitar que capturem padrões repetidos.
- c) Reduzir o colsample_bytree, diminuindo a fração de variáveis disponíveis para a construção de cada árvore e aumentando a diversidade entre elas.
- d) Aumentar o min_child_weight, exigindo mais informação em cada nó filho antes de aceitar uma divisão.

**Resposta certa:** c) Reduzir o colsample_bytree, diminuindo a fração de variáveis disponíveis para a construção de cada árvore e aumentando a diversidade entre elas.

**Explicação:** A resposta é reduzir o colsample_bytree. Se as árvores usam as mesmas variáveis fortes, limitar a fração de variáveis disponíveis para cada árvore obriga o modelo a explorar outros caminhos e aumenta a diversidade. Mais árvores, menor profundidade e maior min_child_weight controlam tamanho e complexidade, não a repetição das variáveis.

**Fonte:** Aula de Ensemble Models, pág. 44

**Situação:** explicação conferida com o material das aulas

---

### Questão 201533-1-9
Área 4 · Árvores, Redes e Ensemble Models III

Um cientista está treinando um XGBoost e decide aumentar o valor do hiperparâmetro reg_alpha. Qual é o efeito esperado dessa alteração?

- a) Valores maiores de reg_alpha reduzem a taxa de aprendizado do modelo, tornando a convergência do boosting mais lenta e gradual.
- b) Valores maiores de reg_alpha aumentam o número de árvores construídas durante o treinamento, elevando o custo computacional do modelo.
- c) Valores maiores de reg_alpha aumentam a complexidade do modelo, permitindo que ele capture padrões mais sutis nos dados de treino.
- d) Valores maiores de reg_alpha favorecem modelos mais simples e podem reduzir a influência de variáveis pouco relevantes.

**Resposta certa:** d) Valores maiores de reg_alpha favorecem modelos mais simples e podem reduzir a influência de variáveis pouco relevantes.

**Explicação:** A resposta é a última. O reg_alpha é a regularização L1: valores maiores favorecem modelos mais simples e podem zerar a contribuição de padrões fracos ou pouco relevantes. Ele não muda a taxa de aprendizado (learning_rate), não altera o número de árvores (n_estimators) e reduz a complexidade, em vez de aumentá-la.

**Fonte:** Aula de Ensemble Models, pág. 44 e pág. 43

**Situação:** explicação conferida com o material das aulas

---


# Área 5: Estatística, data wrangling, coleta de dados, text mining, redes sociais, pesquisa operacional, séries temporais, gestão de riscos, computação evolucionária, modelagem matemática

## Analytics e Gestão de Riscos I

### Questão 156178-1-1
Área 5 · Analytics e Gestão de Riscos I

Um ativo teve os seguintes retornos esperados em uma semana na B3: 

1,3% 
- 2,8%
2,01%
0,9%
- 0,1% 

Pode-se dizer que sua volatilidade é de:
Um ativo teve os seguintes retornos esperados em uma semana na B3:
Pode-se dizer que sua volatilidade é de:

- a) 1,87%
- b) 1,03%
- c) 0,26%
- d) 3,09%

**Resposta certa:** a) 1,87%

**Explicação:** A resposta é 1,87%, o desvio padrão amostral dos retornos. A média é 1,31 / 5 = 0,262%. A soma dos desvios ao quadrado dá cerca de 14,05, que dividida por n - 1 = 4 resulta em variância de 3,51, e a raiz é 1,87%. Dividindo por n daria 1,68%, que não está entre as opções.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 156178-1-10
Área 5 · Analytics e Gestão de Riscos I

O risco de uma carteira depende de qual fator ?

- a) Do risco e da correlação de cada elemento que a compõe e de sua participação no investimento total.
- b) Da soma dos riscos individuais de cada título.
- c) Da variância dos retornos dos ativos que a compõem.
- d) Do risco individual de cada ativo e da sua participação na carteira.

**Resposta certa:** a) Do risco e da correlação de cada elemento que a compõe e de sua participação no investimento total.

**Explicação:** A resposta é a que combina risco, correlação e participação de cada ativo. A fórmula do risco da carteira usa os pesos, os riscos individuais e a covariância (ou correlação) entre os pares. Somar os riscos individuais ou olhar só o risco e a participação ignora a correlação, que é o que gera o efeito da diversificação.

**Fonte:** Aula de risco e retorno de carteiras, pág. 16

**Situação:** explicação conferida com o material das aulas

---

### Questão 156178-1-2
Área 5 · Analytics e Gestão de Riscos I

Na figura a seguir, estão representadas cinco curvas desenhadas a partir do cálculo do risco de uma carteira composta por dois ativos (A e B) a partir de possíveis valores da correlação (r) entre esses ativos. Qual é a curva que possui maior possibilidade de diversificação?

[imagem: imagens/156178_1_2_0.jpg]

- a) I
- b) III
- c) IV
- d) II

**Resposta certa:** a) I

**Explicação:** Todas as curvas partem de A e chegam a B. Quanto mais a curva se curva para a esquerda, menor o risco da carteira para o mesmo retorno, e a curva I é a mais arqueada, a que chega no menor risco. A V é a reta (correlação +1), sem nenhum ganho de diversificação, então a I é a de maior possibilidade.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 156178-1-3
Área 5 · Analytics e Gestão de Riscos I

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre volatilidade:

- a) A volatilidade é a variância dos retornos contínuos.
- b) A volatilidade é a média dos retornos contínuos ao longo do tempo.
- c) A volatilidade é o desvio padrão dos retornos contínuos.
- d) A volatilidade é o desvio padrão dos preços do ativo.

**Resposta certa:** c) A volatilidade é o desvio padrão dos retornos contínuos.

**Explicação:** A resposta é o desvio padrão dos retornos contínuos, porque volatilidade é a medida de dispersão dos retornos do ativo em torno da média. O desvio padrão é a raiz da variância e volta para a mesma unidade dos retornos, por isso é ele que se usa, e não a variância. Desvio padrão dos preços está errado porque o preço em nível não é estacionário, trabalha-se com os retornos.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 90

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 156178-1-4
Área 5 · Analytics e Gestão de Riscos I

Qual é o comando do google planilhas para buscar cotações de ativos no mercado?

- a) googleplanilha
- b) sparkline
- c) googlecotacao
- d) googlefinance

**Resposta certa:** d) googlefinance

**Explicação:** A resposta é googlefinance, a função nativa do Google Planilhas que busca cotações de ativos, índices e câmbio direto da fonte de mercado, por exemplo =GOOGLEFINANCE("PETR4"). As outras opções não existem como função de cotação: sparkline faz minigráficos dentro da célula.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 156178-1-5
Área 5 · Analytics e Gestão de Riscos I

Considere as seguintes características de risco e retorno esperado dos ativos no gráfico e assinale a alternativa CORRETA:

[imagem: imagens/156178_1_5_0.jpg]

- a) O ativo A é preferível ao ativo B.
- b) O ativo C é preferível ao ativo A.
- c) O ativo B é preferível ao ativo A.
- d) O ativo D é preferível ao ativo C.

**Resposta certa:** a) O ativo A é preferível ao ativo B.

**Explicação:** No gráfico, A e B têm o mesmo retorno esperado, mas A está mais à esquerda, com menor risco (desvio-padrão). Para o mesmo retorno, o investidor prefere o menor risco, então A é preferível a B. O C tem risco parecido com A e retorno bem menor, e o D tem risco maior que o C com o mesmo retorno, então as outras alternativas falham.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 156178-1-6
Área 5 · Analytics e Gestão de Riscos I

Considere uma carteira com dois ativos (A e B). O ativo A possui um retorno esperado de 8% e o ativo B, um retorno esperado de 25%. O risco do ativo A é 5% e o risco do ativo B é 12%. Essa carteira possui R$10.000,00 investidos com 50% no ativo A e 50% no ativo B. Qual será o risco dessa carteira se a correlação entre os ativos for -0,6?

- a) 4,92%.
- b) 3,50%.
- c) 8,50%.
- d) 6,78%.

**Resposta certa:** a) 4,92%.

**Explicação:** A resposta é 4,92%. Com pesos de 50% e correlação de -0,6, a variância da carteira é 0,5²·5² + 0,5²·12² + 2·0,5·0,5·5·12·(-0,6) = 6,25 + 36 - 18 = 24,25. A raiz de 24,25 dá 4,92%. A soma simples dos riscos ponderados daria 8,5%, que ignora a correlação.

**Fonte:** Aula de risco e retorno de carteiras, pág. 16

**Situação:** explicação conferida com o material das aulas

---

### Questão 156178-1-7
Área 5 · Analytics e Gestão de Riscos I

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre risco:

- a) O risco de um ativo é medido pelo desvio padrão dos retornos discretos.
- b) O risco é medido pela média dos retornos de um ativo ao longo do tempo.
- c) O risco é medido pelo coeficiente de variação dos valores de mercado.
- d) O risco é medido pela variância dos preços absolutos de um ativo.

**Resposta certa:** a) O risco de um ativo é medido pelo desvio padrão dos retornos discretos.

**Explicação:** A resposta é o desvio padrão dos retornos, que mede o quanto os retornos de um ativo oscilam em torno da média. A média dos retornos mede o retorno esperado, não o risco, e a variância dos preços absolutos não é a medida usada porque os ativos são comparados por seus retornos.

**Fonte:** Aula de risco e retorno de carteiras, pág. 13

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 156178-1-8
Área 5 · Analytics e Gestão de Riscos I

Considere as seguintes afirmações e assinale a alternativa CORRETA:

I.	A redução do risco de um portfólio somente se processa mediante uma diminuição do retorno esperado, verificando-se uma correlação positiva entre risco e retorno.

II.	 A diversificação do risco de uma carteira ocorre sempre que o índice de correlação dos ativos for superior a -1,0, sendo maior a redução quanto mais positivamente correlacionados estiverem os ativos.

III.	 A seleção de carteiras procura identificar a melhor combinação possível de ativos, obedecendo às preferências do investidor com relação ao risco e retorno esperados.

- a) Somente as afirmações I e II são verdadeiras.
- b) Somente as afirmações II e III são verdadeiras.
- c) Somente a afirmação III é verdadeira.
- d) Somente as afirmações I e III são verdadeiras.

**Resposta certa:** c) Somente a afirmação III é verdadeira.

**Explicação:** A resposta é que só a afirmação III é verdadeira. A I é falsa porque diversificar reduz risco sem necessariamente reduzir o retorno esperado. A II está invertida: a redução é maior quanto mais negativa a correlação, e com correlação perfeita positiva não há ganho. A III descreve corretamente a seleção de carteiras.

**Fonte:** Aula de risco e retorno de carteiras, pág. 16

**Situação:** explicação conferida com o material das aulas

---

### Questão 156178-1-9
Área 5 · Analytics e Gestão de Riscos I

Imagine que você tenha uma carteira de investimentos com dois ativos de correlação perfeita e negativa. Nesse cenário, é possível zerar o risco dessa carteira?

- a) Não, pois nem todo risco é diversificável.
- b) Não, pois a correlação entre ativos não afeta a capacidade de diversificação do risco.
- c) Sim, é possível eliminar 100% do risco através da diversificação adequada.
- d) Sim, pois o risco diversificável aumenta à medida que se adiciona mais ativos à carteira.

**Resposta certa:** a) Não, pois nem todo risco é diversificável.

**Explicação:** O gabarito marca que não, porque nem todo risco é diversificável. Mas com correlação perfeita e negativa (-1) e pesos escolhidos de forma que as oscilações se anulem, a fórmula do risco da carteira chega a zero, ou seja, a resposta "Sim, é possível eliminar 100% do risco" seria a correta em termos matemáticos. O risco sistemático só impede zerar o risco de carteiras reais com correlações maiores que -1.

**Fonte:** Aula de risco e retorno de carteiras, pág. 16

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** Com correlação -1 e pesos adequados o desvio padrão da carteira chega a zero, então a opção "Sim" parece mais correta que o gabarito. Mantive o gabarito da plataforma.

---

## Analytics e Gestão de Riscos II

### Questão 156868-1-1
Área 5 · Analytics e Gestão de Riscos II

Um fator relacionado ao risco de crédito é a perda incorrida. Assinale a alternativa CORRETA sobre a perda incorrida.

- a) A perda incorrida corresponde ao valor máximo que pode ser perdido em condições adversas de mercado.
- b) A perda incorrida corresponde à diferença entre a exposição total e o valor recuperável após execução de garantias.
- c) A perda incorrida corresponde à estimativa de perdas futuras baseada em projeções estatísticas.
- d) A perda incorrida corresponde ao evento de crédito já ocorrido ou em vias de ocorrer.

**Resposta certa:** d) A perda incorrida corresponde ao evento de crédito já ocorrido ou em vias de ocorrer.

**Explicação:** A resposta é que a perda incorrida é o evento de crédito já ocorrido ou em vias de ocorrer. A perda esperada é a outra ponta: trata da probabilidade de ocorrer um evento de crédito no futuro. Por isso a opção sobre estimativa de perdas futuras está trocada.

**Fonte:** Aula de risco de crédito, pág. 26

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-10
Área 5 · Analytics e Gestão de Riscos II

Um dos direcionadores do risco de crédito é a exposição a crédito no default. Assinale a alternativa CORRETA sobre esse direcionador.

- a) Está relacionado à incerteza quanto ao valor da exposição do crédito no momento do default.
- b) Está relacionado à incerteza quanto à probabilidade de ocorrência do evento de inadimplência.
- c) Está relacionado à incerteza quanto ao percentual de perda após a materialização do default.
- d) Está relacionado à incerteza quanto à capacidade de pagamento do devedor antes do default.

**Resposta certa:** a) Está relacionado à incerteza quanto ao valor da exposição do crédito no momento do default.

**Explicação:** A resposta é a incerteza quanto ao valor da exposição do crédito no momento do default. A incerteza sobre a probabilidade de default pertence ao direcionador inadimplência, e a incerteza sobre o percentual perdido após o default pertence à perda dado default (LGD).

**Fonte:** Aula de risco de crédito, pág. 28

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-2
Área 5 · Analytics e Gestão de Riscos II

Qual das alternativas representa o principal conjunto de normas internacionais para gestão de riscos em instituições financeiras?

- a) Acordo de Montreal.
- b) Acordo de Basiléia.
- c) Acordo de Michigan.
- d) Acordo de Ipanema.

**Resposta certa:** b) Acordo de Basiléia.

**Explicação:** A resposta é o Acordo de Basileia, firmado no âmbito do Comitê de Basileia, ligado ao BIS, que reúne bancos centrais e define regras de capital, solvência e alavancagem para instituições financeiras (Basileia I, II e III). Os demais nomes não existem como acordos de gestão de risco.

**Fonte:** Aula de gestão de riscos, pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-3
Área 5 · Analytics e Gestão de Riscos II

Considere o conteúdo discutido em aula e assinale a alternativa CORRETA sobre o conceito de risco de crédito.

- a) O risco de crédito é o risco de perda econômica decorrente do não cumprimento de obrigações contratuais por uma contraparte.
- b) O risco de crédito é o risco decorrente das variações dos preços no mercado.
- c) É o risco decorrente de erros humanos, tecnológicos, sejam intencionais ou não.
- d) O risco de crédito é o risco de perdas causadas por mudanças na legislação ou regulamentação.

**Resposta certa:** a) O risco de crédito é o risco de perda econômica decorrente do não cumprimento de obrigações contratuais por uma contraparte.

**Explicação:** A resposta é a definição de risco de crédito como risco de perda econômica por descumprimento das obrigações contratuais por uma contraparte. As outras alternativas descrevem outros riscos: variação de preços é risco de mercado, erros humanos e tecnológicos são risco operacional, e mudanças de legislação são risco legal.

**Fonte:** Aula de risco de crédito, pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-4
Área 5 · Analytics e Gestão de Riscos II

Avalie as alternativas e assinale a que apresenta direcionadores do risco de crédito.

- a) Exposição à Crédito no default; risco dado default; ganhos no default.
- b) Segurança; inadimplência e perda dado default.
- c) Risco; perda dado default; comprometimento.
- d) Inadimplência; Exposição à Crédito no default; Perda dado default.

**Resposta certa:** d) Inadimplência; Exposição à Crédito no default; Perda dado default.

**Explicação:** A resposta é inadimplência (default), exposição a crédito no default e perda dado default. Esses são os três direcionadores: probabilidade de a contraparte entrar em default, quanto está exposto nesse momento e que percentual não será recuperado. Os outros itens misturam termos que não fazem parte do modelo.

**Fonte:** Aula de risco de crédito, pág. 28

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-5
Área 5 · Analytics e Gestão de Riscos II

Considere os conceitos apresentados em aula e assinale a alternativa CORRETA sobre o Comitê de Basiléia.

- a) É formado por representantes de Bancos Centrais e autoridades de supervisão bancária de diversos países que debatem e estabelecem padrões de regulação.
- b) É formado por seguradoras internacionais que estabelecem requisitos de capital para operações de resseguro.
- c) É formado exclusivamente por bancos comerciais privados que determinam as taxas de juros praticadas no mercado interbancário global.
- d) É formado por empresas de tecnologia financeira (fintechs) que desenvolvem padrões de cibersegurança para o setor bancário.

**Resposta certa:** a) É formado por representantes de Bancos Centrais e autoridades de supervisão bancária de diversos países que debatem e estabelecem padrões de regulação.

**Explicação:** A resposta é que o Comitê da Basileia reúne representantes de bancos centrais e autoridades de supervisão bancária que debatem e formalizam estudos e padrões. Fica na cidade de Basileia, na Suíça. Não é formado por seguradoras, bancos privados ou fintechs.

**Fonte:** Aula de gestão de riscos, pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-6
Área 5 · Analytics e Gestão de Riscos II

Considere os conceitos apresentados em aula e assinale a alternativa CORRETA sobre o Bank for International Settlements (BIS).

- a) O BIS visa promover a cooperação entre os bancos centrais e outras agências na busca de estabilidade monetária e financeira.
- b) O BIS visa fabricar e distribuir cédulas de dinheiro para todos os países do mundo.
- c) O BIS visa construir e administrar aeroportos internacionais em capitais financeiras.
- d) O BIS visa operar redes de supermercados e lojas de varejo em países europeus.

**Resposta certa:** a) O BIS visa promover a cooperação entre os bancos centrais e outras agências na busca de estabilidade monetária e financeira.

**Explicação:** A resposta é a cooperação entre bancos centrais e outras agências em busca de estabilidade monetária e financeira. O BIS, fundado em 1930 e sediado na Basileia, é chamado de banco central dos bancos centrais. Ele não emite cédulas nem administra empresas ou aeroportos.

**Fonte:** Aula de gestão de riscos, pág. 34

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-7
Área 5 · Analytics e Gestão de Riscos II

Um fator relacionado ao risco de crédito é a perda esperada. Assinale a alternativa CORRETA sobre a perda esperada.

- a) A perda esperada corresponde ao percentual da exposição que não poderá ser recuperado após a inadimplência.
- b) A perda esperada corresponde ao evento de crédito já ocorrido ou em vias de ocorrer.
- c) A perda esperada corresponde a probabilidade de ocorrer o evento de crédito futuro.
- d) A perda esperada corresponde ao valor total da exposição no momento do default.

**Resposta certa:** c) A perda esperada corresponde a probabilidade de ocorrer o evento de crédito futuro.

**Explicação:** A resposta, segundo o material da aula, é que a perda esperada está associada à probabilidade de ocorrer o evento de crédito futuro. A perda incorrida é a do evento já ocorrido ou em vias de ocorrer, que aparece na outra alternativa tentadora. Exposição total e percentual não recuperável são outros direcionadores (EAD e LGD).

**Fonte:** Aula de risco de crédito, pág. 26

**Situação:** explicação conferida com o material das aulas

---

### Questão 156868-1-8
Área 5 · Analytics e Gestão de Riscos II

Considere o conteúdo discutido em aula e assinale a alternativa CORRETA sobre o conceito de risco de mercado.

- a) O risco de mercado é o risco decorrente de falhas em processos internos ou sistemas operacionais.
- b) O risco de mercado é o risco de perdas causadas por mudanças na legislação ou regulamentação.
- c) O risco de mercado é o risco decorrente das variações dos preços no mercado.
- d) O risco de mercado é o risco de inadimplência de contrapartes em operações financeiras.

**Resposta certa:** c) O risco de mercado é o risco decorrente das variações dos preços no mercado.

**Explicação:** A resposta é a variação dos preços no mercado. Risco de mercado é a perda por oscilação de preços de ativos, juros, câmbio e outros fatores. Falhas de processos são risco operacional, inadimplência é risco de crédito e mudanças de lei são risco legal.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 156868-1-9
Área 5 · Analytics e Gestão de Riscos II

Avalie as assertivas e assinale a alternativa CORRETA:

I - Risco de crédito representa a possibilidade de inadimplemento da contraparte de qualquer instrumento financeiro, gerando a falta de recebimento para a outra parte.

II - Pode-se dizer que risco é a quantificação da incerteza.

III - No risco de crédito, a perda incorrida corresponde ao evento de crédito já ocorrido ou em vias de ocorrer.
Avalie as assertivas e assinale a alternativa CORRETA:
I - Risco de crédito representa a possibilidade de inadimplemento da contraparte de qualquer instrumento financeiro, gerando a falta de recebimento para a outra parte.
II - Pode-se dizer que risco é a quantificação da incerteza.
III - No risco de crédito, a perda incorrida corresponde ao evento de crédito já ocorrido ou em vias de ocorrer.

- a) Apenas a assertiva II é verdadeira.
- b) Apenas a assertiva I é verdadeira.
- c) Todas as assertivas são verdadeiras.
- d) Apenas a assertiva III é verdadeira.

**Resposta certa:** c) Todas as assertivas são verdadeiras.

**Explicação:** A resposta é que todas as assertivas são verdadeiras. A I e a III batem com as definições de risco de crédito e de perda incorrida da aula (evento já ocorrido ou em vias de ocorrer). A II também está correta: risco é a quantificação da incerteza, conceito usado ao longo da disciplina.

**Fonte:** Aula de risco de crédito, pág. 26

**Situação:** explicação conferida com o material das aulas

---

## Coleta de Dados: Crawlers e Web Scraping

### Questão 190232-1-1
Área 5 · Coleta de Dados: Crawlers e Web Scraping

Assinale a alternativa CORRETA sobre o protocolo HTTP.

- a) É um protocolo de renderização gráfica de uma página web.
- b) É uma linguagem de programação para manipular variáveis categóricas.
- c) É um protocolo que define as regras para troca de informações dentro do modelo cliente-servidor na web.
- d) É um protocolo usado apenas para envio de e-mails.

**Resposta certa:** c) É um protocolo que define as regras para troca de informações dentro do modelo cliente-servidor na web.

**Explicação:** A resposta é que o HTTP define as regras de troca de informações no modelo cliente-servidor da web: o cliente faz a requisição e o servidor responde. Não renderiza páginas (isso é do navegador), não é linguagem de programação e não serve só para e-mail.

**Fonte:** Aula de coleta de dados, pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 190232-1-10
Área 5 · Coleta de Dados: Crawlers e Web Scraping

O BeautifulSoup, apresentado em aula, é mais bem descrito como uma biblioteca que:

- a) Controla um navegador Chrome real para clicar em botões.
- b) Faz requisições HTTP e baixa o HTML da internet.
- c) É utilizada para analisar e extrair informações de arquivos HTML de forma simples.
- d) Substitui completamente a requests, dispensando-a do processo.

**Resposta certa:** c) É utilizada para analisar e extrair informações de arquivos HTML de forma simples.

**Explicação:** A resposta é a que diz que o BeautifulSoup analisa e extrai informações de arquivos HTML. Ele não baixa a página (quem faz a requisição é a requests, que continua sendo necessária) e não controla navegador, função do Selenium.

**Fonte:** Aula de coleta de dados, pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 190232-1-2
Área 5 · Coleta de Dados: Crawlers e Web Scraping

De acordo com o conteúdo apresentado em aula, uma API é mais bem descrita como:

- a) Um arquivo que lista o que os robôs podem ou não acessar.
- b) Um navegador automatizado que clica em botões por você.
- c) Uma página HTML cheia de cores e layout feita para humanos lerem.
- d) Um "balcão de atendimento" feito para programas, que devolve os dados já organizados e prontos para uso.

**Resposta certa:** d) Um "balcão de atendimento" feito para programas, que devolve os dados já organizados e prontos para uso.

**Explicação:** A resposta é a imagem do balcão de atendimento para programas: a API devolve os dados já estruturados, em geral em JSON, sem precisar interpretar uma página feita para humanos. O arquivo que lista o que robôs podem acessar é o robots.txt, e o navegador automatizado que clica em botões é o Selenium.

**Fonte:** Data Science do Zero, pág. 171

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 190232-1-3
Área 5 · Coleta de Dados: Crawlers e Web Scraping

Dentre as bibliotecas Python abaixo, qual delas é amplamente usada para Web Scraping?

- a) BeautifulSoup.
- b) Matplotlib.
- c) Pandas.
- d) NumPy.

**Resposta certa:** a) BeautifulSoup.

**Explicação:** A resposta é BeautifulSoup, biblioteca para analisar HTML e extrair títulos, links e tabelas. Matplotlib serve para gráficos e Pandas e NumPy para manipular e calcular dados, não para extrair informação de páginas.

**Fonte:** Aula de coleta de dados, pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 190232-1-4
Área 5 · Coleta de Dados: Crawlers e Web Scraping

Qual o significado da sigla API utilizada no contexto da aula?

- a) Application Process Integration.
- b) Automated Page Indexing.
- c) Application Programming Interface.
- d) Advanced Programming Instance.

**Resposta certa:** c) Application Programming Interface.

**Explicação:** A resposta é Application Programming Interface, interface de programação de aplicações. É o ponto em que um serviço oferece dados a outros programas de forma estruturada.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 190232-1-5
Área 5 · Coleta de Dados: Crawlers e Web Scraping

Assinale a alternativa que apresenta o objetivo central na aplicação de técnicas de web scraping.

- a) Criar e/ou alterar o conteúdo de sites na internet.
- b) Coletar dados automaticamente de sites da internet.
- c) Criar mecanismos de proteção do navegador contra vírus da web.
- d) Aumentar a velocidade de conexão para download de páginas da web.

**Resposta certa:** b) Coletar dados automaticamente de sites da internet.

**Explicação:** A resposta é coletar dados automaticamente de sites. Na aula, o scraping é o programa assumindo o papel de navegador, acessando e interpretando as páginas sozinho. Criar conteúdo, proteger contra vírus ou acelerar a conexão não fazem parte do conceito.

**Fonte:** Aula de coleta de dados, pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 190232-1-6
Área 5 · Coleta de Dados: Crawlers e Web Scraping

Qual das seguintes afirmações sobre scraping está INCORRETA?

- a) Pode utilizar ferramentas como Selenium e Scrapy.
- b) Permite coletar dados públicos automaticamente.
- c) Pode ser usado quando não há API disponível.
- d) É sempre ilegal em qualquer contexto.

**Resposta certa:** d) É sempre ilegal em qualquer contexto.

**Explicação:** A incorreta é a que diz que scraping é sempre ilegal. A LGPD não cita o termo e manda considerar finalidade, boa-fé e interesse público no tratamento de dados públicos. A legalidade depende de contexto, como termos de serviço, consentimento e intenção. As demais afirmações são verdadeiras.

**Fonte:** Aula de coleta de dados, pág. 44

**Situação:** explicação conferida com o material das aulas

---

### Questão 190232-1-7
Área 5 · Coleta de Dados: Crawlers e Web Scraping

O que viaja pela rede quando o servidor responde a uma requisição é:

- a) O texto bruto (o código HTML), que o navegador depois transforma na página visual.
- b) A página já renderizada, exatamente como aparece na tela do usuário.
- c) Apenas uma imagem da página em formato de foto.
- d) Somente o código de status, sem qualquer conteúdo.

**Resposta certa:** a) O texto bruto (o código HTML), que o navegador depois transforma na página visual.

**Explicação:** A resposta é o texto bruto, o código HTML. O servidor responde com HTML (e CSS e JavaScript associados) e o navegador é quem transforma isso na página visual. Por isso um scraper com requests recebe o código e precisa interpretá-lo, por exemplo com BeautifulSoup.

**Fonte:** Aula de coleta de dados, pág. 35

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 190232-1-8
Área 5 · Coleta de Dados: Crawlers e Web Scraping

O que são DevTools nos navegadores?

- a) Um conjunto de ferramentas para inspeção e depuração de páginas web.
- b) Um antivírus embutido nos navegadores modernos.
- c) Uma extensão paga para criar bancos de dados.
- d) Uma ferramenta usada apenas para alterar cores de sites.

**Resposta certa:** a) Um conjunto de ferramentas para inspeção e depuração de páginas web.

**Explicação:** A resposta é um conjunto de ferramentas para inspecionar, editar e depurar páginas da web em tempo real, embutido nos navegadores modernos. No scraping é usado para achar tags, classes e ids dos elementos que se quer extrair.

**Fonte:** Aula de coleta de dados, pág. 26

**Situação:** explicação conferida com o material das aulas

---

### Questão 190232-1-9
Área 5 · Coleta de Dados: Crawlers e Web Scraping

Considere os conceitos apresentados em aula e assinale a alternativa que define o Web Scraping da maneira CORRETA.

- a) É um método para simular interações humanas com redes sociais.
- b) É o processo de acessar uma API para coletar dados organizados.
- c) É uma técnica para hackear sites e acessar dados confidenciais.
- d) É um processo automatizado de extração de dados diretamente de páginas web.

**Resposta certa:** d) É um processo automatizado de extração de dados diretamente de páginas web.

**Explicação:** A resposta é o processo automatizado de extração de dados direto de páginas web. A alternativa sobre API fala de outra forma de coleta, que já devolve dados organizados, e não é o scraping. Hackear sites também não faz parte da definição.

**Fonte:** Aula de coleta de dados, pág. 21

**Situação:** explicação conferida com o material das aulas

---

## Computação Evolucionária I

### Questão 152213-1-1
Área 5 · Computação Evolucionária I

Considere os conceitos discutidos em aula e assinale a alternativa que apresenta exemplos de hiperparâmetros em Algoritmos Genéticos.

- a) Função de aptidão e operador de mutação.
- b) Crossover uniforme e seleção por torneio.
- c) Cromossomo e fenótipo.
- d) Taxa de mutação e tamanho da população.

**Resposta certa:** d) Taxa de mutação e tamanho da população.

**Explicação:** A resposta é taxa de mutação e tamanho da população, porque hiperparâmetros são os valores que você define antes de rodar o algoritmo e que controlam seu comportamento, como população, taxa de mutação, taxa de cruzamento e número de gerações. Cromossomo e fenótipo são elementos da representação da solução, e a função de aptidão faz parte da definição do problema.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 152213-1-10
Área 5 · Computação Evolucionária I

A metáfora da teoria da evolução natural aplicada aos Algoritmos Genéticos se refere à:

- a) Sobrevivência dos indivíduos mais adaptados, por meio de seleção, cruzamento e mutação.
- b) Recombinação aleatória de pesos para gerar aprendizado supervisionado.
- c) Simulação da seleção artificial por meio de aprendizado por reforço.
- d) Utilização de redes neurais profundas para prever mutações.

**Resposta certa:** a) Sobrevivência dos indivíduos mais adaptados, por meio de seleção, cruzamento e mutação.

**Explicação:** A resposta é a sobrevivência dos mais adaptados por seleção, cruzamento e mutação, que é a analogia com a evolução natural: a população evolui por gerações, com os melhores combinados e variados. Aprendizado supervisionado, reforço e redes neurais profundas não fazem parte dessa metáfora.

**Fonte:** Aula de Algoritmos Genéticos, pág. 5 e pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 152213-1-2
Área 5 · Computação Evolucionária I

Em relação à Metáfora da teoria da evolução natural apresentada em aula, qual alternativa associa corretamente os termos aos elementos dos Algoritmos Genéticos?

- a) Cromossomo = função objetivo; Gene = indivíduo; Alelo = população; Genótipo = crossover.
- b) Genótipo = saída do algoritmo; Fenótipo = vetor de hiperparâmetros.
- c) Gene = posição no cromossomo; Alelo = valor assumido; Fenótipo = solução interpretada no problema.
- d) Gene = população; Alelo = número da geração.

**Resposta certa:** c) Gene = posição no cromossomo; Alelo = valor assumido; Fenótipo = solução interpretada no problema.

**Explicação:** A resposta é gene como posição no cromossomo, alelo como valor assumido e fenótipo como a solução interpretada no problema. Na aula o genótipo é a sequência de valores do cromossomo e o fenótipo é o que ela significa no problema, como as proporções da mistura. As outras alternativas trocam os conceitos, por exemplo chamando gene de população.

**Fonte:** Aula de Algoritmos Genéticos, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 152213-1-3
Área 5 · Computação Evolucionária I

Em relação ao processo de cruzamento (crossover) em Algoritmos Genéticos, é correto afirmar que:

- a) Consiste na combinação de genes de dois pais para gerar novos indivíduos.
- b) Serve para introduzir diversidade aleatória na população.
- c) Substitui a função de mutação completamente.
- d) Garante que todos os indivíduos sejam idênticos.

**Resposta certa:** a) Consiste na combinação de genes de dois pais para gerar novos indivíduos.

**Explicação:** A resposta é que o cruzamento combina genes de dois pais para gerar novos indivíduos. Na aula ele aparece como a mistura de duas soluções, por exemplo duas receitas ou duas mochilas. Introduzir diversidade aleatória é papel da mutação, e o cruzamento nem a substitui nem deixa todos os indivíduos idênticos.

**Fonte:** Aula de Algoritmos Genéticos, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 152213-1-4
Área 5 · Computação Evolucionária I

Em Computação Evolucionária, o que mede a função de aptidão (fitness)?

- a) A qualidade de cada indivíduo com base na função objetivo.
- b) A taxa de eliminação de soluções ruins da população.
- c) O formato e a estrutura do cromossomo.
- d) A distância euclidiana entre indivíduos da população.

**Resposta certa:** a) A qualidade de cada indivíduo com base na função objetivo.

**Explicação:** A resposta é a qualidade de cada indivíduo com base na função objetivo. A aula define o fitness como a qualidade da solução, e as métricas de avaliação tratam o fitness como o valor da função objetivo. Ele não mede a estrutura do cromossomo, a taxa de eliminação nem distância entre indivíduos.

**Fonte:** Aula de Algoritmos Genéticos, pág. 5 e pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 152213-1-5
Área 5 · Computação Evolucionária I

O número de gerações é um hiperparâmetro utilizado em Algoritmos Genéticos. Assinale a alternativa correta sobre o número de gerações.

- a) O número de gerações deve ser sempre igual ao tamanho da população para garantir convergência.
- b) O número de gerações determina automaticamente a qualidade da solução encontrada.
- c) O número de gerações é um hiperparâmetro que define um critério de parada do algoritmo.
- d) O número de gerações representa o número de operadores genéticos aplicados simultaneamente.

**Resposta certa:** c) O número de gerações é um hiperparâmetro que define um critério de parada do algoritmo.

**Explicação:** A resposta é que o número de gerações é um hiperparâmetro que define um critério de parada, porque o algoritmo repete o ciclo de seleção, cruzamento e mutação até atingir esse limite. Mais gerações não garantem qualidade da solução por si só, não precisam ser iguais ao tamanho da população e não têm relação com a quantidade de operadores.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 152213-1-6
Área 5 · Computação Evolucionária I

Dentre as alternativas abaixo, assinale aquela que contém operadores genéticos utilizados nos Algoritmos Genéticos.

- a) Aprendizado supervisionado, Regressão e Classificação.
- b) Classificação, Agrupamento e Redução de dimensionalidade.
- c) Crossover e Mutação.
- d) Mutação, Validação cruzada e Normalização.

**Resposta certa:** c) Crossover e Mutação.

**Explicação:** A resposta é crossover e mutação, que são os operadores genéticos que geram novas soluções a partir da população atual. A aula mostra cruzamento e mutação junto com a seleção como os passos que produzem novas gerações. Regressão, classificação, agrupamento e validação cruzada são termos de aprendizado de máquina.

**Fonte:** Aula de Algoritmos Genéticos, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 152213-1-7
Área 5 · Computação Evolucionária I

Considere os conceitos discutidos em aula sobre os Algoritmos Genéticos e assinale a alternativa INCORRETA:

- a) A codificação é a forma como os genes são representados.
- b) Se o critério de parada for atendido, volta à avaliação. Se não for atendido, retorna a melhor solução.
- c) A função fitness mede a qualidade de cada indivíduo com base na função objetivo.
- d) A taxa de Mutação é a probabilidade de um gene sofrer mutação ao longo da evolução.

**Resposta certa:** b) Se o critério de parada for atendido, volta à avaliação. Se não for atendido, retorna a melhor solução.

**Explicação:** A incorreta é a que diz que, se o critério de parada for atendido, volta à avaliação, e se não for, retorna a melhor solução. Está invertida: atendido o critério, o AG para e devolve a melhor solução; se não, o ciclo continua com nova geração e nova avaliação. As outras três afirmações descrevem corretamente codificação, fitness e taxa de mutação.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 152213-1-8
Área 5 · Computação Evolucionária I

Qual das alternativas representa corretamente os principais elementos presentes na estrutura de modelos matemáticos?

- a) Dados de treinamento, função de perda e métricas de avaliação.
- b) Hiperparâmetros, operadores genéticos e população inicial.
- c) Variáveis de decisão, função objetivo e restrições.
- d) Parâmetros de entrada, algoritmos de busca e critérios de convergência.

**Resposta certa:** c) Variáveis de decisão, função objetivo e restrições.

**Explicação:** A resposta é variáveis de decisão, função objetivo e restrições, os três elementos de um modelo de pesquisa operacional. As variáveis são as incógnitas que a solução determina, a função objetivo mede o que se quer maximizar ou minimizar e as restrições limitam os valores possíveis. As demais alternativas misturam itens de aprendizado de máquina ou de algoritmos genéticos.

**Fonte:** Pesquisa Operacional (Belfiore e Fávero), pág. 13

**Situação:** explicação conferida com o material das aulas

---

### Questão 152213-1-9
Área 5 · Computação Evolucionária I

Analise as afirmativas a seguir, considerando a analogia entre termos biológicos e elementos dos Algoritmos Genéticos, e assinale a alternativa correta.

I. Cromossomo é a representação de uma possível solução (geralmente como vetor de genes).

II. Gene é um elemento básico do cromossomo. Ele representa um traço ou parte da solução.

III. Alelo é o valor específico que um gene pode assumir.

IV. Fenótipo é o conjunto de soluções (indivíduos) em uma geração.

V. Genótipo é um cromossomo dentro da população.
Analise as afirmativas a seguir, considerando a analogia entre termos biológicos e elementos dos Algoritmos Genéticos, e assinale a alternativa correta.
I. Cromossomo é a representação de uma possível solução (geralmente como vetor de genes).
II. Gene é um elemento básico do cromossomo. Ele representa um traço ou parte da solução.
III. Alelo é o valor específico que um gene pode assumir.
IV. Fenótipo é o conjunto de soluções (indivíduos) em uma geração.
V. Genótipo é um cromossomo dentro da população.

- a) Todas as afirmativas são verdadeiras.
- b) Apenas I e V são falsas.
- c) Apenas IV e V são verdadeiras.
- d) Apenas I, II e III são verdadeiras.

**Resposta certa:** d) Apenas I, II e III são verdadeiras.

**Explicação:** A resposta é que apenas I, II e III são verdadeiras. Cromossomo é a solução, gene é uma parte dela e alelo é o valor que o gene assume. A IV está errada porque o conjunto de soluções em uma geração é a população, não o fenótipo, que é o significado da solução no problema. A V também erra: genótipo é a sequência de valores do cromossomo.

**Fonte:** Aula de Algoritmos Genéticos, pág. 5 e pág. 6

**Situação:** explicação conferida com o material das aulas

---

## Computação Evolucionária II

### Questão 152542-1-1
Área 5 · Computação Evolucionária II

Qual das seguintes afirmações descreve corretamente o papel da função de fitness na computação evolucionária?

- a) Realiza a mutação de indivíduos, alterando aleatoriamente o genoma para garantir a diversidade genética.
- b) É utilizada para selecionar os indivíduos mais aptos da população, escolhendo quais terão a chance de se reproduzir.
- c) Determina o quão adequada é uma solução para o problema, guiando a seleção natural.
- d) É responsável por codificar a solução do problema em um formato binário.

**Resposta certa:** c) Determina o quão adequada é uma solução para o problema, guiando a seleção natural.

**Explicação:** A resposta é a que diz que a função de fitness determina o quão adequada é uma solução, guiando a seleção. Ela só mede a qualidade do indivíduo pela função objetivo. Quem seleciona é o operador de seleção, que usa esse valor, e a mutação e a codificação são outras etapas.

**Fonte:** Aula de Algoritmos Genéticos, pág. 5

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-10
Área 5 · Computação Evolucionária II

Considere o problema do caixeiro viajante apresentado em aula e assinale a alternativa CORRETA:

- a) O problema do caixeiro viajante busca encontrar o número ideal de caixeiros para visitar todas as cidades.
- b) O problema do caixeiro viajante busca encontrar o roteiro de vendas mais longo possível para um caixeiro.
- c) O problema do caixeiro viajante busca encontrar o menor caminho para visitar um conjunto de cidades e retornar ao ponto de partida.
- d) O problema do caixeiro viajante busca encontrar a composição de itens que maximiza o peso da mochila.

**Resposta certa:** c) O problema do caixeiro viajante busca encontrar o menor caminho para visitar um conjunto de cidades e retornar ao ponto de partida.

**Explicação:** A resposta é encontrar o menor caminho que visita um conjunto de cidades e retorna ao ponto de partida. O problema busca o roteiro de menor custo que passa por cada cidade uma única vez e volta à origem. Mochila é outro problema, e não se trata de definir número de caixeiros nem o roteiro mais longo.

**Fonte:** Pesquisa Operacional (Belfiore e Fávero), pág. 479

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-2
Área 5 · Computação Evolucionária II

Considere os conceitos relacionados a otimização multiobjetivo e assinale a alternativa CORRETA sobre o Método da Fronteira de Pareto.

- a) O Método da Fronteira de Pareto elimina o conjunto de todas as soluções que foram rejeitadas.
- b) O Método da Fronteira de Pareto envolve a geração de um conjunto de soluções não-dominadas que formam a fronteira de Pareto, onde nenhuma outra solução é melhor em todos os objetivos.
- c) No Método da Fronteira de Pareto, sempre encontra-se a melhor solução individual de todas as gerações.
- d) O Método da Fronteira de Pareto realiza a mistura de dois indivíduos no problema da mochila.

**Resposta certa:** b) O Método da Fronteira de Pareto envolve a geração de um conjunto de soluções não-dominadas que formam a fronteira de Pareto, onde nenhuma outra solução é melhor em todos os objetivos.

**Explicação:** A resposta é a que descreve a geração de soluções não dominadas que formam a fronteira de Pareto, em que nenhuma outra solução é melhor em todos os objetivos. Não se trata de descartar soluções rejeitadas, de achar a melhor solução individual de todas as gerações ou de misturar indivíduos na mochila.

**Fonte:** Aula de Algoritmos Genéticos (otimização multiobjetivo), pág. 42

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-3
Área 5 · Computação Evolucionária II

O desvio padrão do fitness é uma das métricas de avaliação de um Algoritmo Genético (AG). O que representa um baixo desvio padrão no contexto dos AGs?

- a) População diversificada.
- b) Mistura de dois indivíduos.
- c) Melhor fitness.
- d) Convergência.

**Resposta certa:** d) Convergência.

**Explicação:** A resposta é convergência. Um desvio padrão baixo do fitness significa que os indivíduos têm valores parecidos, ou seja, a população deixou de ser diversa e convergiu, o que é esperado nas gerações finais. Alto desvio indica população diversificada, útil no começo da busca.

**Fonte:** Aula de Algoritmos Genéticos (métricas de avaliação), pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-4
Área 5 · Computação Evolucionária II

A modelagem de problemas em algoritmos evolucionários requer a definição de uma representação adequada. No contexto do Problema do Caixeiro Viajante, qual das alternativas abaixo descreve corretamente uma representação evolutiva clássica para as soluções?

- a) Um valor escalar que armazena a distância total do percurso.
- b) Um vetor binário, onde cada gene assume 0 ou 1.
- c) Uma sequência de números inteiros que representam a ordem das cidades a serem visitadas.
- d) Uma matriz de adjacência representando as conexões entre as cidades.

**Resposta certa:** c) Uma sequência de números inteiros que representam a ordem das cidades a serem visitadas.

**Explicação:** A resposta é a sequência de números inteiros que representa a ordem das cidades visitadas. No caixeiro viajante cada solução é uma permutação das cidades, e o fitness é a distância total desse percurso. Um vetor binário serve para a mochila, e a distância é o valor avaliado, não a representação da solução.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 152542-1-5
Área 5 · Computação Evolucionária II

Um dos aspectos centrais da computação evolucionária é:

- a) Resolver problemas de otimização de forma inspirada na natureza.
- b) Criar modelos de inteligência artificial que replicam o cérebro humano.
- c) Prever o comportamento de espécies em ecossistemas.
- d) Desenvolver novas tecnologias de DNA sintético.

**Resposta certa:** a) Resolver problemas de otimização de forma inspirada na natureza.

**Explicação:** A resposta é resolver problemas de otimização de forma inspirada na natureza. A computação evolucionária reúne algoritmos de busca heurística baseados na evolução natural das espécies, como os algoritmos genéticos. Não busca replicar o cérebro, prever ecossistemas nem produzir DNA sintético.

**Fonte:** Pesquisa Operacional (Belfiore e Fávero), pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-6
Área 5 · Computação Evolucionária II

Qual a principal diferença entre um problema de otimização de objetivo único e um problema de otimização multiobjetivo?

- a) Problemas de objetivo único têm apenas uma solução, enquanto os multiobjetivos não.
- b) Um problema de objetivo único não pode ser resolvido com algoritmos genéticos.
- c) Problemas multiobjetivo buscam otimizar várias funções simultaneamente, que podem estar em conflito.
- d) Problemas multiobjetivo são sempre mais fáceis de resolver.

**Resposta certa:** c) Problemas multiobjetivo buscam otimizar várias funções simultaneamente, que podem estar em conflito.

**Explicação:** A resposta é que problemas multiobjetivo otimizam várias funções ao mesmo tempo, e elas podem estar em conflito, como custo e qualidade. Por isso em geral não há uma única solução ótima, e sim um conjunto de soluções de compromisso. Não são mais fáceis, e os AGs também resolvem o caso de objetivo único.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 152542-1-7
Área 5 · Computação Evolucionária II

A taxa de convergência é uma das métricas de avaliação de um Algoritmo Genético (AG). Assinale a alternativa CORRETA sobre a taxa de convergência.

- a) Avalia o quão rápido o AG converge para uma solução ótima (ou próxima do ótimo).
- b) É o número de avaliações da função objetivo.
- c) Corresponde à média do valor da função objetivo na população.
- d) Corresponde ao valor da função objetivo da melhor solução encontrada.

**Resposta certa:** a) Avalia o quão rápido o AG converge para uma solução ótima (ou próxima do ótimo).

**Explicação:** A resposta é que a taxa de convergência avalia o quão rápido o AG chega a uma solução ótima ou próxima do ótimo, em geral medida em número de gerações. As outras alternativas descrevem outras métricas: número de avaliações da função objetivo, fitness médio e melhor fitness.

**Fonte:** Aula de Algoritmos Genéticos (métricas de avaliação), pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-8
Área 5 · Computação Evolucionária II

O fitness médio é uma das métricas de avaliação de um Algoritmo Genético (AG). Assinale a alternativa CORRETA sobre o fitness médio.

- a) Avalia o quão rápido o AG converge para uma solução ótima (ou próxima do ótimo).
- b) Corresponde ao valor da função objetivo da melhor solução encontrada.
- c) É o número de avaliações da função objetivo.
- d) Corresponde à média do valor da função objetivo na população.

**Resposta certa:** d) Corresponde à média do valor da função objetivo na população.

**Explicação:** A resposta é a média do valor da função objetivo na população. O fitness médio resume a população inteira, ao passo que o melhor fitness olha só o melhor indivíduo e a taxa de convergência mede a velocidade com que o AG se aproxima do ótimo.

**Fonte:** Aula de Algoritmos Genéticos (métricas de avaliação), pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-1-9
Área 5 · Computação Evolucionária II

O cruzamento em algoritmos genéticos tem como principal objetivo:

- a) Reduzir o número de indivíduos na população.
- b) Introduzir uma nova solução completamente aleatória.
- c) Avaliar a qualidade de cada indivíduo.
- d) Propagar características de boas soluções entre as gerações.

**Resposta certa:** d) Propagar características de boas soluções entre as gerações.

**Explicação:** A resposta é propagar características de boas soluções entre as gerações. Ao combinar dois pais já selecionados pelo fitness, o cruzamento passa adiante partes boas de cada um. Soluções totalmente aleatórias vêm da mutação, e avaliar a qualidade é função do fitness.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 152542-2-3
Área 5 · Computação Evolucionária II

Qual é o papel da mutação em um algoritmo genético?

- a) Selecionar os indivíduos mais aptos para a próxima geração.
- b) Aumentar a diversidade genética para evitar que o algoritmo estacione em ótimos locais.
- c) Aumentar o tamanho da população a cada geração.
- d) Combinar o material genético de dois indivíduos pais para formar um novo.

**Resposta certa:** b) Aumentar a diversidade genética para evitar que o algoritmo estacione em ótimos locais.

**Explicação:** A resposta é aumentar a diversidade genética para evitar que o algoritmo estacione em ótimos locais. A mutação altera genes ao acaso e leva a busca para regiões novas, enquanto a seleção escolhe os mais aptos e o cruzamento combina os pais.

**Fonte:** Pesquisa Operacional (Belfiore e Fávero), pág. 451

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-2-4
Área 5 · Computação Evolucionária II

No Problema da Mochila apresentado em aula, qual é o principal objetivo?

- a) Atribuir tarefas a trabalhadores da forma mais eficiente.
- b) Encontrar o caminho mais curto entre vários pontos.
- c) Maximizar o valor total dos itens dentro de uma mochila, sem exceder sua capacidade.
- d) Distribuir o peso de forma uniforme entre vários contêineres.

**Resposta certa:** c) Maximizar o valor total dos itens dentro de uma mochila, sem exceder sua capacidade.

**Explicação:** A resposta é maximizar o valor total dos itens na mochila sem exceder a capacidade. Cada objeto tem utilidade e peso, e a restrição é que a soma dos pesos não ultrapasse o limite. Caminho mais curto é o caixeiro viajante e alocação de tarefas é o problema de designação.

**Fonte:** Pesquisa Operacional (Belfiore e Fávero), pág. 393

**Situação:** explicação conferida com o material das aulas

---

### Questão 152542-2-9
Área 5 · Computação Evolucionária II

O desvio padrão do fitness é uma das métricas de avaliação de um Algoritmo Genético (AG). O que se pode concluir diante de um alto desvio padrão do fitness?

- a) Pode-se concluir que o AG convergiu rapidamente.
- b) Pode-se concluir que a população é diversificada.
- c) Pode-se concluir que a solução ótima foi encontrada.
- d) Pode-se concluir que o melhor fitness foi encontrado.

**Resposta certa:** b) Pode-se concluir que a população é diversificada.

**Explicação:** A resposta é que um alto desvio padrão do fitness indica população diversificada, pois os indivíduos têm valores bem diferentes entre si. É o comportamento esperado nas gerações iniciais. Quando o desvio fica baixo, a população convergiu. Ele sozinho não diz que o ótimo foi achado.

**Fonte:** Aula de Algoritmos Genéticos (métricas de avaliação), pág. 30

**Situação:** explicação conferida com o material das aulas

---

## Data Wrangling I

### Questão 184595-1-1
Área 5 · Data Wrangling I

Qual das funções do Python apresentadas a seguir permite criar uma variável categórica por meio da identificação dos quartis de uma variável métrica de referência?

- a) .astype( )
- b) .reset_index( )
- c) .sort_values( )
- d) pd.qcut( )

**Resposta certa:** d) pd.qcut( )

**Explicação:** A resposta é pd.qcut(), que divide uma variável métrica em faixas por quantis, e com q=4 gera as categorias dos quartis. O astype muda o tipo da variável, o reset_index reinicia o índice e o sort_values apenas ordena.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-10
Área 5 · Data Wrangling I

Certas funções do pacote “pandas”, no Python, permitem que seja utilizado o argumento inplace=True. Assinale a alternativa que apresenta a correta finalidade de usar tal argumento.

- a) Duplicar o objeto que foi tratado, mantendo a versão original para referência.
- b) Alterar o nome do objeto na lista de objetos que foram gerados na análise.
- c) Realizar o print das alterações no console, mas sem que seja gerado novo objeto.
- d) Sobrescrever as alterações realizadas no mesmo objeto que foi originalmente utilizado.

**Resposta certa:** d) Sobrescrever as alterações realizadas no mesmo objeto que foi originalmente utilizado.

**Explicação:** A resposta é sobrescrever as alterações no próprio objeto original. Com inplace=True a função modifica o DataFrame existente e não devolve cópia, enquanto sem ele é preciso atribuir o resultado a um objeto. Não duplica o objeto nem apenas imprime as mudanças.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-2
Área 5 · Data Wrangling I

Para selecionar uma parte do banco de dados de um DataFrame, de modo que as variáveis e/ou observações sejam selecionadas com base em sua posição numérica, utiliza-se a função:

- a) .iloc
- b) .sort
- c) .search
- d) .show

**Resposta certa:** a) .iloc

**Explicação:** A resposta é .iloc, que seleciona linhas e colunas pela posição numérica (integer location). O .loc faz o mesmo por rótulos. As outras opções não são métodos do pandas para seleção.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-3
Área 5 · Data Wrangling I

Assinale a alternativa que apresenta a finalidade da função .assign( ) do “pandas” no Python.

- a) Excluir as colunas de um DataFrame com base em uma lista de nomes.
- b) Selecionar observações do DataFrame com base em posições numéricas.
- c) Adicionar variáveis a um DataFrame, mantendo as colunas existentes.
- d) Renomear, ao mesmo tempo, todas as variáveis existentes no DataFrame.

**Resposta certa:** c) Adicionar variáveis a um DataFrame, mantendo as colunas existentes.

**Explicação:** A resposta é adicionar variáveis ao DataFrame mantendo as colunas existentes. O .assign() devolve um DataFrame com as novas colunas criadas a partir de expressões. Excluir colunas é função do .drop() e selecionar por posição é do .iloc.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-4
Área 5 · Data Wrangling I

Dentre as funções do Python listadas a seguir, assinale aquela que permite que sejam obtidas as informações de todas as variáveis do DataFrame chamado “banco_dados” para a observação localizada na posição de índice 40.

- a) banco_dados.iloc[:,40]
- b) banco_dados.iloc[40,]
- c) banco_dados.iloc[40,40]
- d) banco_dados.iloc[0,40]

**Resposta certa:** b) banco_dados.iloc[40,]

**Explicação:** A resposta é banco_dados.iloc[40,], que pega a linha de posição 40 e todas as colunas. No iloc o primeiro argumento é a linha e o segundo é a coluna. Por isso iloc[:,40] traz a coluna 40, e iloc[40,40] traz só uma célula.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-5
Área 5 · Data Wrangling I

Para identificar as variáveis do DataFrame do Python cujos nomes iniciam-se com um prefixo comum utiliza-se a função:

- a) .columns.beginning( )
- b) .columns.str.startswith( )
- c) .columns.selectwith( )
- d) .columns.str.endswith( )

**Resposta certa:** b) .columns.str.startswith( )

**Explicação:** A resposta é .columns.str.startswith(), que testa se cada nome de coluna começa com o prefixo informado e devolve valores booleanos, úteis para selecionar colunas. O .str.endswith() faz o mesmo para o final do nome. Beginning e selectwith não existem.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-6
Área 5 · Data Wrangling I

Dentre as funções do Python listadas a seguir, assinale a alternativa que contém uma função adequada para organizar em ordem decrescente as informações do DataFrame com base em uma variável nomeada de 'var'.

- a) .sort_values(by=['var'], ascending=False)
- b) .normalize(by=['var'], ascending=True)
- c) .organizer(by=['var'], ascending=False)
- d) .sort_values(by=['var'], ascending=True)

**Resposta certa:** a) .sort_values(by=['var'], ascending=False)

**Explicação:** A resposta é .sort_values(by=['var'], ascending=False), em que ascending=False ordena do maior para o menor. Com ascending=True a ordem seria crescente, e normalize e organizer não são métodos de ordenação.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-7
Área 5 · Data Wrangling I

Dentre as funções do Python listadas a seguir, assinale a alternativa que contém uma função que tem a finalidade principal de adicionar uma nova variável ao DataFrame e manter as demais já existentes no objeto.

- a) .drop( )
- b) .assign( )
- c) .sort_values( )
- d) .set_option( )

**Resposta certa:** b) .assign( )

**Explicação:** A resposta é .assign(), que cria uma nova variável e mantém as demais. O .drop() remove linhas ou colunas, o .sort_values() só ordena e o .set_option() ajusta opções de exibição.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-8
Área 5 · Data Wrangling I

Em relação às organizações de um DataFrame do Python por meio da função .sort_values( ), assinale a alternativa correta.

- a) A função permite exclusivamente uma variável como critério de organização do DataFrame.
- b) Somente variáveis categóricas podem ser utilizadas como critério de organização.
- c) Somente variáveis métricas podem ser utilizadas como critério de organização.
- d) É possível realizar a organização com base em mais de um critério, ou seja, mais de uma variável no mesmo comando.

**Resposta certa:** d) É possível realizar a organização com base em mais de um critério, ou seja, mais de uma variável no mesmo comando.

**Explicação:** A resposta é que dá para ordenar por mais de uma variável no mesmo comando. Basta passar uma lista em by, como by=['a','b'], e a segunda variável desempata a primeira. Pode-se ordenar tanto por variáveis métricas quanto por categóricas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 184595-1-9
Área 5 · Data Wrangling I

Dentre as funções do Python listadas a seguir, assinale a alternativa que contém uma função adequada para visualizar as informações gerais sobre o DataFrame.

- a) .info( )
- b) .check( )
- c) .drop( )
- d) .del( )

**Resposta certa:** a) .info( )

**Explicação:** A resposta é .info(), que mostra o resumo do DataFrame: número de linhas, nomes das colunas, tipos e contagem de valores não nulos. O .drop() remove dados, e .check() e .del() não são métodos do pandas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Data Wrangling II

### Questão 185675-1-1
Área 5 · Data Wrangling II

Para que seja possível extrair as frequências relativas observadas de uma variável categórica contida em um DataFrame do pandas, deve-se incluir o comando:

- a) .value_counts(percent=True)
- b) .agg(normalize=False)
- c) .unique(normalize=True)
- d) .value_counts(normalize=True)

**Resposta certa:** d) .value_counts(normalize=True)

**Explicação:** A resposta é .value_counts(normalize=True), que devolve as proporções de cada categoria em vez das contagens. O argumento percent não existe no value_counts, e unique não aceita normalize.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-10
Área 5 · Data Wrangling II

Dentre as funções do Python listadas a seguir, assinale a alternativa que contém uma função adequada para extrair estatísticas descritivas de um DataFrame do “pandas”.

- a) .drop( )
- b) .assign( )
- c) .describe( )
- d) .rename( )

**Resposta certa:** c) .describe( )

**Explicação:** A resposta é .describe(). Em um DataFrame ela devolve contagem, média, desvio padrão, mínimo, quartis e máximo das variáveis numéricas. O .drop() remove linhas ou colunas, o .assign() cria colunas e o .rename() muda nomes, nenhum deles calcula estatísticas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-2
Área 5 · Data Wrangling II

Qual das funções do Python descritas a seguir permite verificar quais são as categorias de uma variável categórica e a contagem observada em cada categoria?

- a) .corr( )
- b) .value_counts( )
- c) .iloc( )
- d) .sort_values( )

**Resposta certa:** b) .value_counts( )

**Explicação:** A resposta é .value_counts(), que lista as categorias de uma variável e quantas vezes cada uma aparece. O .corr() calcula correlações, o .iloc seleciona por posição e o .sort_values ordena.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-3
Área 5 · Data Wrangling II

Assinale a alternativa que apresenta o argumento lógico do Python que possibilita que seja indicado o “não” em uma função que tem o objetivo de selecionar linhas do DataFrame.

- a) |
- b) !=
- c) ==
- d) ~

**Resposta certa:** d) ~

**Explicação:** A resposta é ~. No pandas, a condição de filtro vira uma série de verdadeiros e falsos, e o til inverte esse resultado: df[~(df['x'] > 3)] devolve as linhas que não atendem ao critério. O | é o operador de "ou", != compara diferença e == compara igualdade, nenhum deles nega uma condição inteira.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-4
Área 5 · Data Wrangling II

Caso o intuito seja obter uma tabela de frequências cruzadas para duas variáveis categóricas de um banco de dados no Python, a função que atingirá tal objetivo, dentre as listadas a seguir, é:

- a) pd.crosstab( )
- b) np.gentab( )
- c) np.count( )
- d) pd.table( )

**Resposta certa:** a) pd.crosstab( )

**Explicação:** A resposta é pd.crosstab(). Ela cruza duas variáveis categóricas e devolve a tabela de frequências cruzadas, ou tabela de contingência, com a contagem de cada combinação de categorias. As outras opções (np.gentab, np.count, pd.table) não existem com essa finalidade em pandas ou numpy.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-5
Área 5 · Data Wrangling II

Em relação ao procedimento de agrupamento do banco de dados por meio do .groupby() do Python, assinale a alternativa correta.

- a) É possível realizar o agrupamento considerando mais de uma variável como critério de grupo.
- b) É um objeto com a finalidade única de visualização, isto é, não permite realização de análises.
- c) O banco de dados agrupado não permite a extração de estatísticas descritivas das variáveis.
- d) O agrupamento só pode ser realizado com base em apenas uma variável de cada vez.

**Resposta certa:** a) É possível realizar o agrupamento considerando mais de uma variável como critério de grupo.

**Explicação:** A resposta é que o groupby aceita mais de uma variável como critério, bastando passar uma lista de colunas, como df.groupby(['a','b']). O objeto agrupado serve para análise: dá para aplicar mean(), count(), describe() e agg() em cada grupo, então as demais alternativas descrevem limitações que não existem.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-6
Área 5 · Data Wrangling II

Um analista verificou que o DataFrame contém muitos valores faltantes (nan). Considerando que a decisão foi de excluir qualquer observação que apresente nan em qualquer uma das variáveis, a função do Python que atinge tal objetivo é:

- a) .cut(lines=[ ])
- b) .drop(columns=[ ])
- c) .exclude( )
- d) .dropna( )

**Resposta certa:** d) .dropna( )

**Explicação:** A resposta é .dropna(). Sem argumentos, ela remove toda linha que tenha NaN em qualquer coluna, que é exatamente o caso pedido. O .drop(columns=[]) retira colunas pelo nome, não linhas com faltantes, e .cut e .exclude não servem para isso.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-7
Área 5 · Data Wrangling II

Assinale a alternativa que apresenta os operadores utilizados no Python para filtrar as observações de um DataFrame que atendam, respectivamente, aos seguintes critérios:

i: que indique “ou”

ii: que seja “diferente”

iii: que indique “menor”
Assinale a alternativa que apresenta os operadores utilizados no Python para filtrar as observações de um DataFrame que atendam, respectivamente, aos seguintes critérios:
i: que indique “ou”
ii: que seja “diferente”
iii: que indique “menor”

- a) i: & , ii: <> , iii: <
- b) i: < , ii: >= , iii: &
- c) i: == , ii: != , iii: /
- d) i: | , ii: != , iii: <

**Resposta certa:** d) i: | , ii: != , iii: <

**Explicação:** A resposta é | para "ou", != para "diferente" e < para "menor". Em filtros de pandas, & é o "e" e | é o "ou", e cada condição vai entre parênteses. O <> do Python 2 não vale no pandas atual, e == é igualdade, não diferença.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 185675-1-8
Área 5 · Data Wrangling II

Qual das funções do Python identificadas a seguir permite unir informações que estão em dois DataFrames separados de modo que seja utilizada uma variável “chave” para a junção das informações?

- a) .agg( )
- b) .groupby( )
- c) .assign( )
- d) .merge( )

**Resposta certa:** d) .merge( )

**Explicação:** A resposta é .merge(). Ela junta dois DataFrames a partir de uma ou mais colunas-chave em comum, como num join de SQL. O .groupby() e o .agg() resumem dados dentro de uma única tabela, e o .assign() só cria colunas novas.

**Fonte:** Aula de Data Wrangling, pág. 4

**Situação:** explicação conferida com o material das aulas

---

### Questão 185675-1-9
Área 5 · Data Wrangling II

Assinale a alternativa que apresenta o operador lógico do Python que possibilita que seja filtrada a interseção entre dois critérios de seleção de observações.

- a) ==
- b) &
- c) !=
- d) >=

**Resposta certa:** b) &

**Explicação:** A resposta é &. Ele combina dois critérios e mantém só as linhas que atendem aos dois ao mesmo tempo, ou seja, a interseção. Em pandas cada condição precisa ficar entre parênteses, como df[(df.a > 1) & (df.b < 5)]. Os demais são operadores de comparação, não de combinação.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Data Wrangling III

### Questão 187211-1-1
Área 5 · Data Wrangling III

Assinale a alternativa que apresenta uma função do Python que permite, com base nas posições dos caracteres, extrair parte do texto de uma variável textual.

- a) .str.select()
- b) pd.qcut()
- c) .find()
- d) .str.slice()

**Resposta certa:** d) .str.slice()

**Explicação:** A resposta é .str.slice(). Ele corta o texto pela posição dos caracteres, por exemplo .str.slice(0, 3) pega os três primeiros. O .find() só informa em que posição um trecho aparece, e .str.select() não existe. O pd.qcut() cria faixas de uma variável numérica.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-10
Área 5 · Data Wrangling III

Assinale a alternativa que apresenta uma função do Python que permite que seja verificado se determinado elemento de uma variável do DataFrame está contido em uma lista a ser especificada.

- a) isin()
- b) for()
- c) inside()
- d) in()

**Resposta certa:** a) isin()

**Explicação:** A resposta é isin(). Aplicado a uma coluna, devolve True nas linhas cujo valor está na lista informada, como df['uf'].isin(['SP','MG']), e serve para filtrar. As opções for(), inside() e in() não são métodos de séries do pandas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-2
Área 5 · Data Wrangling III

Assinale a alternativa que apresenta uma função do “pandas” que permite que uma variável do DataFrame seja transformada para o tipo “data” quando ela contiver incorretamente informações de data armazenadas como texto.

- a) pd.date()
- b) pd.to_datetime()
- c) pd.chagedate()
- d) pd.to_date()

**Resposta certa:** b) pd.to_datetime()

**Explicação:** A resposta é pd.to_datetime(). Ela converte uma coluna de texto com datas para o tipo datetime, e a partir daí dá para extrair ano, mês ou dia da semana. As outras funções (pd.date, pd.chagedate, pd.to_date) não existem no pandas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-3
Área 5 · Data Wrangling III

Dentre as opções listadas a seguir, assinale a alternativa que contém o parâmetro adequado para ser usado na função pd.read_excel e que permite indicar como estão codificados os valores faltantes no arquivo a ser importado.

- a) na=
- b) missing_values=
- c) na_specify=
- d) na_values=

**Resposta certa:** d) na_values=

**Explicação:** A resposta é na_values=. É o parâmetro de pd.read_excel (e de read_csv) em que se informa quais valores do arquivo devem virar NaN, como "-", "NA" ou 999. Os outros nomes não são parâmetros dessa função.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-4
Área 5 · Data Wrangling III

Assinale a alternativa correta. No Python, a função pd.concat( ) pode ser utilizada com a finalidade de gerar:

- a) um DataFrame único que une observações provenientes de DataFrames separados.
- b) estatísticas descritivas das variáveis de um objeto agrupado por meio de critérios específicos.
- c) um DataFrame com estrutura alterada em termos de inserção de informações das linhas em colunas.
- d) dois DataFrames separados com informações que estavam consolidadas em objeto único.

**Resposta certa:** a) um DataFrame único que une observações provenientes de DataFrames separados.

**Explicação:** A resposta é que pd.concat() gera um único DataFrame empilhando observações de DataFrames separados, com as mesmas colunas, um embaixo do outro. Ela não faz junção por chave, que é papel do merge, nem calcula estatísticas por grupo, nem separa um objeto em dois.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-5
Área 5 · Data Wrangling III

Dentre as alternativas a seguir, assinale aquela que contém uma função do Python que permite selecionar todas as variáveis que estão nas posições de 0 a 5 de um DataFrame, obtendo todas as linhas existentes no mesmo. Considere que o DataFrame chama-se “df”.

- a) df.iloc[ : , 0:6]
- b) df.iloc[ : , 1:5]
- c) df.iloc[ , 0:6]
- d) df.iloc[ , 0:5]

**Resposta certa:** a) df.iloc[ : , 0:6]

**Explicação:** A resposta é df.iloc[:, 0:6]. O iloc seleciona por posição, o primeiro argumento são as linhas (os dois pontos pedem todas) e o segundo, as colunas. O fatiamento exclui o limite final, então 0:6 traz as posições 0 a 5. As opções com vírgula sem os dois pontos são sintaxe inválida, e 1:5 deixaria a coluna 0 de fora.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-6
Área 5 · Data Wrangling III

Assinale a alternativa que apresenta uma função que tem a finalidade de selecionar apenas as observações que não sejam missing values no Python. Considere que o DataFrame chama-se “df” e a variável em análise chama-se “var”.

- a) df[~ df['var'].isna()]
- b) df[~ var.isna()]
- c) [var.df].isna()
- d) df.is_missing()

**Resposta certa:** a) df[~ df['var'].isna()]

**Explicação:** A resposta é df[~df['var'].isna()]. O .isna() marca com True os valores faltantes, o til inverte a marcação e o df[...] fica só com as linhas em que a variável está preenchida. As demais opções têm sintaxe inexistente ou não indexam o DataFrame.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-7
Área 5 · Data Wrangling III

Assinale a alternativa que contém a função do Python que pode ser aplicada a um DataFrame agrupado e que permite que sejam obtidas as contagens observadas dos elementos de dada variável.

- a) .shift()
- b) .count()
- c) .mean()
- d) .sum()

**Resposta certa:** b) .count()

**Explicação:** A resposta é .count(). Aplicada a um DataFrame agrupado, ela devolve quantas observações não faltantes cada grupo tem em cada variável. O .sum() e o .mean() calculam soma e média dos valores, e o .shift() apenas desloca a série no tempo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-8
Área 5 · Data Wrangling III

Assinale a alternativa que contém uma função do “pandas” que permite que seja realizada uma mudança estrutural no DataFrame no sentido de colocar informações que estão em linhas para colunas.

- a) pd.rename()
- b) pd.copy()
- c) pd.reset_index()
- d) pd.pivot()

**Resposta certa:** d) pd.pivot()

**Explicação:** A resposta é pd.pivot(). Ela reorganiza a tabela do formato longo para o largo: os valores de uma variável que estavam em linhas viram colunas. O rename muda nomes, o copy duplica o objeto e o reset_index só refaz o índice, nenhum altera essa estrutura.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 187211-1-9
Área 5 · Data Wrangling III

Para adicionar novas variáveis ao DataFrame do “pandas” mantendo as outras colunas já existentes, a função adequada do Python, dentre as alternativas a seguir, é:

- a) .gen()
- b) .assign()
- c) .add_columns()
- d) .drop()

**Resposta certa:** b) .assign()

**Explicação:** A resposta é .assign(). Ela cria uma ou mais colunas novas e devolve o DataFrame com todas as colunas que já existiam. O .drop() faz o contrário, remove colunas, e .gen() e .add_columns() não existem no pandas (o gen é comando do Stata).

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Data Wrangling IV

### Questão 188875-1-1
Área 5 · Data Wrangling IV

Assinale a alternativa correta. A função do Git “push” é utilizada para:

- a) Acrescentar arquivos a um índice de arquivos em uma área de preparação.
- b) Enviar os commits de um repositório local para um repositório remoto.
- c) Registar as alterações do arquivo, capturando o estado do projeto naquele momento.
- d) Atualizar o conteúdo de um repositório remoto no repositório local.

**Resposta certa:** b) Enviar os commits de um repositório local para um repositório remoto.

**Explicação:** A resposta é que o git push envia os commits do repositório local para o remoto, como o GitHub. O registro das alterações é o commit, a inclusão no índice é o add e trazer o conteúdo do remoto para o local é o pull.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-10
Área 5 · Data Wrangling IV

Para realizar a cópia inicial de um repositório remoto para um repositório local, pode ser utilizada a seguinte função no Git:

- a) push.
- b) commit.
- c) add.
- d) clone.

**Resposta certa:** d) clone.

**Explicação:** A resposta é clone. O git clone faz a cópia inicial de um repositório remoto para a máquina local, com todo o histórico. O push envia commits, o commit registra alterações e o add coloca arquivos na área de preparação.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-2
Área 5 · Data Wrangling IV

Considere as afirmações a seguir sobre o Git:

I. É um software que pode ser utilizado para o controle de versões de arquivos.

II. Possibilita que sejam sincronizados os arquivos de um repositório local com um repositório remoto.

III. Pode ser utilizado para realizar trabalhos em equipes específicas, pois permite controlar o acesso ao repositório somente para algumas pessoas indicadas.

Classifique-as em verdadeiro (V) ou falso (F) e marque a alternativa que contém a sequência correta para a ordem I, II e III:
Considere as afirmações a seguir sobre o Git:
I. É um software que pode ser utilizado para o controle de versões de arquivos.
II. Possibilita que sejam sincronizados os arquivos de um repositório local com um repositório remoto.
III. Pode ser utilizado para realizar trabalhos em equipes específicas, pois permite controlar o acesso ao repositório somente para algumas pessoas indicadas.
Classifique-as em verdadeiro (V) ou falso (F) e marque a alternativa que contém a sequência correta para a ordem I, II e III:

- a) V, V, F.
- b) V, V, V.
- c) F, F, V.
- d) V, F, F.

**Resposta certa:** b) V, V, V.

**Explicação:** A resposta é V, V, V. O Git é um sistema de controle de versões, sincroniza repositório local e remoto com push e pull, e as plataformas que hospedam o remoto, como o GitHub, permitem repositório privado com acesso só para colaboradores escolhidos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-3
Área 5 · Data Wrangling IV

Dentre as funções apresentadas a seguir, assinale a alternativa que contém uma função do Python utilizada para a substituição de determinados elementos presentes em uma varável por outros elementos especificados.

- a) read()
- b) replace()
- c) drop()
- d) astype()

**Resposta certa:** b) replace()

**Explicação:** A resposta é replace(). Em pandas, df['var'].replace({'a': 'b'}) troca valores específicos de uma variável por outros. O astype muda o tipo da coluna, o drop remove linhas ou colunas e o read lê arquivos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-4
Área 5 · Data Wrangling IV

Assinale a alternativa correta. A função Git “add” é utilizada para:

- a) Criar uma ramificação nova em um projeto existente.
- b) Realizar a cópia de um repositório que esteja publicamente disponível.
- c) Atualizar o conteúdo de um repositório remoto no repositório local.
- d) Acrescentar arquivos a um índice de arquivos em uma área de preparação.

**Resposta certa:** d) Acrescentar arquivos a um índice de arquivos em uma área de preparação.

**Explicação:** A resposta é que o git add inclui arquivos no índice, a área de preparação (staging), deixando-os prontos para o próximo commit. Criar ramificação é git branch, copiar um repositório público é git clone e atualizar o local com o remoto é git pull.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-5
Área 5 · Data Wrangling IV

Dentre as funções do Python listadas a seguir, assinale a alternativa que contém uma função adequada para criar a categorização de uma variável métrica especificando detalhadamente os critérios para a geração de cada categoria.

- a) astype()
- b) np.where()
- c) .replace()
- d) .value_counts()

**Resposta certa:** b) np.where()

**Explicação:** A resposta é np.where(). Com ele, a categoria sai de uma condição escrita por você, como np.where(df.idade >= 18, 'adulto', 'menor'), e com np.select dá para encadear várias faixas. O replace troca valores já existentes, o astype muda tipo e o value_counts só conta frequências.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-6
Área 5 · Data Wrangling IV

A respeito da função .str.extractall() da biblioteca “pandas”, assinale a alternativa correta.

- a) É a função utilizada para filtrar as observações com base em critérios lógicos e matemáticos.
- b) Faz a limpeza do DataFrame extraindo todas as observações que estejam duplicadas.
- c) Utilizada para excluir todas as variáveis de uma DataFrame que atendam ao critério dado.
- d) É utilizada para obter elementos de uma string usando como base o critério nela especificado.

**Resposta certa:** d) É utilizada para obter elementos de uma string usando como base o critério nela especificado.

**Explicação:** A resposta é a que diz que o .str.extractall() obtém partes de um texto a partir de um critério, que normalmente é uma expressão regular. Ele devolve todas as ocorrências do padrão em cada string. Não filtra linhas, não remove duplicatas e não exclui variáveis.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-7
Área 5 · Data Wrangling IV

Assinale a alternativa correta. A função do Git “pull” é utilizada para:

- a) Acrescentar arquivos a um índice de arquivos em uma área de preparação.
- b) Realizar a cópia de um repositório que esteja publicamente disponível.
- c) Atualizar o conteúdo de um repositório remoto no repositório local.
- d) Enviar os commits de um repositório local para um repositório remoto.

**Resposta certa:** c) Atualizar o conteúdo de um repositório remoto no repositório local.

**Explicação:** A resposta é que o git pull atualiza o repositório local com o conteúdo do remoto. É o caminho contrário do push, que envia commits. Acrescentar ao índice é o add e copiar um repositório pela primeira vez é o clone.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-8
Área 5 · Data Wrangling IV

Em um DataFrame há uma variável que contém somente números, mas está incorretamente identificada como texto. Assinale a alternativa que apresenta uma função do Python que pode realizar a transformação da variável para o tipo numérica.

- a) .change('number')
- b) as.number
- c) df.int('var')
- d) .astype('float')

**Resposta certa:** d) .astype('float')

**Explicação:** A resposta é .astype('float'). O astype converte o tipo de uma coluna, aqui de texto para número decimal (também serviria 'int' se só houver inteiros). As demais opções não são sintaxe do pandas: as.number é do R e .change e df.int não existem.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 188875-1-9
Área 5 · Data Wrangling IV

Em relação ao GitHub, assinale a alternativa INCORRETA.

- a) Tem sua estrutura organizada em repositórios para o gerenciamento de projetos.
- b) Pode ser utilizado para organizar e publicar o portfólio de projetos em Data Science.
- c) Não é possível configurar um repositório para mantê-lo com acesso privado.
- d) Pode ser utilizado para hospedar arquivos de projetos e verificar alterações em versões.

**Resposta certa:** c) Não é possível configurar um repositório para mantê-lo com acesso privado.

**Explicação:** A afirmação incorreta é a de que não dá para ter repositório privado. O GitHub permite repositórios privados, com acesso só para quem for convidado. As outras três descrevem usos reais: repositórios como estrutura, portfólio de projetos e hospedagem com histórico de versões.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Fundamentos de Estatística e Introdução à Programação com Python

### Questão 146962-1-1
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que apresenta corretamente o resultado de executar o comando numeros = pd.Series([1,2,3,4,5]) no Python:
Assinale a alternativa que apresenta corretamente o resultado de executar o comando numeros = pd.Series([1,2,3,4,5]) no Python:

- a) Gera um DataFrame de números com 5 colunas.
- b) Gera um banco de dados de números com 5 colunas por 5 linhas.
- c) Gera um objeto com o nome pd.Series.
- d) Gera uma série do pandas contendo números.

**Resposta certa:** d) Gera uma série do pandas contendo números.

**Explicação:** A resposta é que pd.Series([1,2,3,4,5]) gera uma série do pandas com esses números, uma estrutura unidimensional com índice. Ela tem uma coluna só, e DataFrame é a estrutura tabular com várias colunas. Por isso as alternativas com 5 colunas ou 5 por 5 estão erradas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 146962-1-10
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Dentre as alternativas a seguir, assinale aquela que apresenta uma função que tem o objetivo de excluir variáveis do banco de dados.

- a) .drop(columns=[ ])
- b) .info( )
- c) .head( )
- d) .exclude( )

**Resposta certa:** a) .drop(columns=[ ])

**Explicação:** A resposta é .drop(columns=[]). Basta listar os nomes das colunas a excluir. O .info() mostra tipos e contagem de não nulos, o .head() exibe as primeiras linhas e .exclude() não é método de DataFrame.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 146962-1-2
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que preenche corretamente as lacunas a seguir. 

“A assimetria e a curtose são medidas de _____ e podem ser aplicadas às variáveis _____.”
Assinale a alternativa que preenche corretamente as lacunas a seguir.
“A assimetria e a curtose são medidas de _____ e podem ser aplicadas às variáveis _____.”

- a) posição; qualitativas.
- b) dispersão; quantitativas.
- c) dispersão; qualitativas.
- d) forma; quantitativas.

**Resposta certa:** d) forma; quantitativas.

**Explicação:** A resposta é forma; quantitativas. Assimetria e curtose descrevem o formato da distribuição, e só fazem sentido para variáveis numéricas. Posição é média, mediana e quartis, e dispersão é variância e desvio padrão.

**Fonte:** Aula de Introdução à Programação Python, pág. 9

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-1-3
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que apresenta corretamente o objetivo de executar o comando import pandas as pd no Python.

- a) Instalar o pacote pd no python.
- b) Importar o pacote pd e atribuir o apelido pandas.
- c) Instalar o elemento pd pertencente ao pacote pandas.
- d) Importar o pacote pandas e atribuir apelido pd.

**Resposta certa:** d) Importar o pacote pandas e atribuir apelido pd.

**Explicação:** A resposta é que import pandas as pd importa o pacote pandas e dá a ele o apelido pd, para escrever pd.read_excel() em vez de pandas.read_excel(). Quem instala o pacote é o pip, o import só carrega algo que já está instalado.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 146962-1-4
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Com base em uma tabela de contingência entre duas variáveis categóricas, o valor da estatística qui-quadrado da tabela e seu p-valor são utilizados para:

- a) Analisar os resíduos para cada par de categorias das variáveis em análise.
- b) Identificar os totais de cada categoria da variável em linha.
- c) Analisar se existe associação estatisticamente significativa entre as variáveis.
- d) Identificar os totais de cada categoria da variável em coluna.

**Resposta certa:** c) Analisar se existe associação estatisticamente significativa entre as variáveis.

**Explicação:** A resposta é analisar se há associação estatisticamente significativa entre as duas variáveis. Na hipótese nula as variáveis se associam de forma aleatória, e quando o qui-quadrado passa do valor crítico (p-valor pequeno) rejeita-se isso. Totais de linhas e colunas são as marginais e os resíduos são outra etapa.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 470

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-1-5
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Sobre os objetos do tipo DataFrame da biblioteca pandas do Python, assinale a alternativa correta:

- a) Não podem ser exportados para o computador, pois o objeto não permite salvá-lo.
- b) São objetos que permitem apenas a inserção de elementos textuais em sua composição.
- c) Não é possível extrair estatísticas descritivas das variáveis contidas nos DataFrame.
- d) São objetos que possuem uma estrutura tabular organizados em linhas e colunas.

**Resposta certa:** d) São objetos que possuem uma estrutura tabular organizados em linhas e colunas.

**Explicação:** A resposta é que o DataFrame é uma estrutura tabular, com variáveis nas colunas e observações nas linhas. Ele aceita colunas numéricas, de texto e de datas, permite estatísticas descritivas (describe) e pode ser exportado, por exemplo com to_excel ou to_csv.

**Fonte:** Aula de Introdução à Programação Python, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-1-6
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que apresenta uma estatística descritiva que pode ser corretamente aplicada a uma variável qualitativa.

- a) Média aritmética.
- b) Coeficiente de variação.
- c) Desvio padrão.
- d) Tabela de frequências.

**Resposta certa:** d) Tabela de frequências.

**Explicação:** A resposta é tabela de frequências. Variáveis qualitativas só têm categorias, então são resumidas por contagens e percentuais. Média, desvio padrão e coeficiente de variação exigem valores numéricos mensuráveis.

**Fonte:** Aula de Introdução à Programação Python, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-1-7
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Sobre o coeficiente de correlação de Pearson, assinale a alternativa CORRETA:

- a) Quanto mais próximo de 0, mais fortemente correlacionadas são as variáveis.
- b) Seus valores podem variar entre os limites 0 e +1.
- c) Seus valores podem variar entre os limites -1 e +1.
- d) Pode ser aplicado para pares de variáveis qualitativas e quantitativas.

**Resposta certa:** c) Seus valores podem variar entre os limites -1 e +1.

**Explicação:** A resposta é que o coeficiente de Pearson varia entre -1 e +1. Ele mede a relação linear entre duas variáveis métricas, e quanto mais perto de um dos extremos, mais forte a correlação. Valores perto de 0 indicam ausência de relação linear, e não se aplica a variáveis qualitativas.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 412

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-1-8
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Em relação aos tipos de variáveis de um banco de dados, assinale a alternativa correta.

- a) Variáveis quantitativas são aquelas que têm seus valores representados por categorias.
- b) Para variáveis quantitativas, a única análise descritiva disponível é a tabela de frequências.
- c) É correto obter a média, mediana e o desvio padrão dos valores de variáveis qualitativas.
- d) Em variáveis categóricas, podemos obter as frequências observadas de suas categorias.

**Resposta certa:** d) Em variáveis categóricas, podemos obter as frequências observadas de suas categorias.

**Explicação:** A resposta é que em variáveis categóricas se obtêm as frequências observadas das categorias. Variáveis qualitativas não admitem média nem desvio padrão, e variáveis quantitativas são numéricas, não categorias, e têm muito mais ferramentas do que a tabela de frequências.

**Fonte:** Aula de Introdução à Programação Python, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-1-9
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

O p-valor de um teste estatístico é definido como:

- a) A probabilidade associada ao valor da estatística de teste calculada.
- b) O nível de confiança do teste, isto é, 1 menos o nível de significância.
- c) A probabilidade de cometer o erro do tipo 1, ou seja, o nível de significância.
- d) O valor crítico da distribuição que define a região de não rejeição da hipótese nula.

**Resposta certa:** a) A probabilidade associada ao valor da estatística de teste calculada.

**Explicação:** A resposta é a probabilidade associada ao valor calculado da estatística de teste. É a probabilidade de obter um resultado tão extremo quanto o observado se a hipótese nula for verdadeira. Compara-se com o nível de significância, mas o p-valor não é o nível de significância nem o valor crítico.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 312

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-2-1
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que apresenta corretamente o comando do pacote pandas utilizado para importar arquivos com extensão .xlsx no Python.

- a) pd.plan( ).
- b) pd.read_excel( ).
- c) pd.read_new_file( ).
- d) pd.read_csv( ).

**Resposta certa:** b) pd.read_excel( ).

**Explicação:** A resposta é pd.read_excel(). Ela lê arquivos .xlsx e devolve um DataFrame. O pd.read_csv() é para arquivos de texto separados por vírgula, e pd.plan() e pd.read_new_file() não existem.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 146962-2-2
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que apresenta corretamente o objetivo de executar o comando pip install pandas no Python.

- a) Instalar o pacote pip no python.
- b) Importar o pacote pandas e atribuir um apelido a ele.
- c) Instalar o pacote pandas no python.
- d) Atribuir o apelido pip ao pacote pandas ao importá-lo.

**Resposta certa:** c) Instalar o pacote pandas no python.

**Explicação:** A resposta é que pip install pandas instala o pacote pandas no Python. O pip é o gerenciador de pacotes, e não o que está sendo instalado. Importar com apelido é outro comando, o import pandas as pd.

**Fonte:** Data Science do Zero, pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 146962-2-9
Área 5 · Fundamentos de Estatística e Introdução à Programação com Python

Assinale a alternativa que apresenta corretamente a definição da mediana de uma variável.

- a) É a soma de todos os valores da variável dividido pela quantidade de observações somadas.
- b) É o elemento que relaciona o desvio padrão e a média da distribuição de uma variável.
- c) É o elemento da distribuição da variável que divide as observações em quatro partes iguais.
- d) É o elemento central da distribuição de uma variável que esteja com seus valores ordenados de forma crescente.

**Resposta certa:** d) É o elemento central da distribuição de uma variável que esteja com seus valores ordenados de forma crescente.

**Explicação:** A resposta é o elemento central da distribuição ordenada. Ordenando os valores do menor para o maior, a mediana é o que fica na posição do meio, com metade das observações abaixo e metade acima (é o segundo quartil). A alternativa da soma dividida pelo número de observações descreve a média, e a que fala em quatro partes iguais descreve os quartis.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 67

**Situação:** explicação conferida com o material das aulas

---

## Modelagem Matemática e Estruturação de Problemas Complexos I

### Questão 158476-1-1
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

O Analytic Hierarchy Process (AHP) é um método para auxiliar pessoas na tomada de decisões complexas. Mais do que determinar qual a decisão correta, o AHP ajuda as pessoas a escolher e a justificar a sua escolha. Baseado em matemática e psicologia, ele foi desenvolvido na década de 1970 pelo Professor:

- a) Thomas Saaty.
- b) George Dantzig.
- c) Marcos dos Santos.
- d) Alan Turing.

**Resposta certa:** a) Thomas Saaty.

**Explicação:** A resposta é Thomas Saaty. O AHP foi desenvolvido por ele na década de 1970, na Wharton School da Universidade da Pensilvânia, com base em matemática e psicologia (escala psicométrica). Dantzig é ligado ao simplex e Turing à computação.

**Fonte:** Aula de Método AHP, pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-10
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

O Método Analytic Hierarchy Process (AHP) baseia-se, fundamentalmente, em:

- a) Matemática e Química.
- b) Matemática e Física.
- c) Matemática e Psicologia (Escala Psicométrica).
- d) Economia e Finanças.

**Resposta certa:** c) Matemática e Psicologia (Escala Psicométrica).

**Explicação:** A resposta é matemática e psicologia (escala psicométrica). A escala fundamental de Saaty é uma escala psicométrica, e o AHP converte julgamentos verbais em números por meio de álgebra matricial. Química, física, economia e finanças não são a base do método.

**Fonte:** Aula de Método AHP, pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-2
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

O método AHP trabalha com comparações par a par de variáveis, utilizando a Escala Fundamental de Saaty. A partir dessas comparações, obtém-se a Matriz de Ponderações (ou de Julgamentos). Nessa matriz, toda a diagonal principal é preenchida com o valor:

- a) 1
- b) 0
- c) 2
- d) 3

**Resposta certa:** a) 1

**Explicação:** A resposta é 1. Na diagonal principal cada critério é comparado com ele mesmo, e na escala de Saaty a igualdade vale 1. A matriz ainda é recíproca, então o resto é preenchido com os valores da escala e seus inversos.

**Fonte:** Aula de Método AHP, pág. 54

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-3
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

No método AHP, para que os julgamentos do decisor sejam considerados “consistentes”, devemos ter:

- a) C.R. ≥ 10%
- b) C.R. ≤ 10%
- c) C.R. > 50%
- d) C.R. ≤ 20%

**Resposta certa:** b) C.R. ≤ 10%

**Explicação:** A resposta é C.R. ≤ 10%. A razão de consistência é CR = CI/RI, e Saaty considera aceitável o julgamento quando ela fica em até 10%. Acima disso o decisor deve rever as comparações par a par.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 158476-1-4
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

A Escala Fundamental de Saaty trabalha com graus de importância que vão:

- a) De 1 a 9.
- b) De 1 a 5.
- c) De 0 a 100.
- d) De 0 a 10.

**Resposta certa:** a) De 1 a 9.

**Explicação:** A resposta é de 1 a 9. A escala fundamental vai de 1 (igualdade) a 9 (extremamente mais importante), com valores pares intermediários, e usa o inverso (1/2 a 1/9) para o sentido contrário.

**Fonte:** Aula de Escala Fundamental de Saaty, pág. 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-5
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

Problemas de tomada de decisão multicritério são caracterizados por:

- a) Uma Matriz Laplaciana que deve ter seus valores normalizados.
- b) Uma Série Temporal que deve ser convertida em uma matriz.
- c) Uma Matriz de Decisão, que é composta de alternativas e critérios ponderados de acordo com o tomador de decisão em questão.
- d) Uma Matriz de Transição proveniente de um Grafo.

**Resposta certa:** c) Uma Matriz de Decisão, que é composta de alternativas e critérios ponderados de acordo com o tomador de decisão em questão.

**Explicação:** A resposta é a Matriz de Decisão, composta de alternativas e critérios ponderados conforme o decisor. É isso que caracteriza os problemas de decisão multicritério (MCDM). As demais opções (matriz laplaciana, série temporal, matriz de transição) não têm relação com o tema.

**Fonte:** Aula de Métodos Multicritério, pág. 20

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-6
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

Sabe-se que o método AHP trabalha com comparações paritárias a partir da Escala Fundamental de Saaty. Um dos axiomas do método AHP é o “Axioma da Reciprocidade”. De acordo com esse axioma se uma comparação aij=5, então a comparação aji necessariamente deve ser igual a:

- a) 0,2
- b) 2
- c) -5
- d) 0,5

**Resposta certa:** a) 0,2

**Explicação:** A resposta é 0,2. Pelo axioma da reciprocidade, aji = 1/aij, então se aij = 5 temos aji = 1/5 = 0,2. A aula mostra o mesmo com aij = 3 e aji = 1/3.

**Fonte:** Aula de Matriz de Ponderações (AHP), pág. 55

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-7
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

Um critério monotônico de custo é aquele que:

- a) Pode ser de minimização ou maximização dependendo do problema em análise.
- b) Quanto maior o seu valor, pior é o seu desempenho. Por isso ele é um critério de minimização.
- c) Quanto menor seu valor, pior é o seu desempenho. Por isso ele é um critério de maximização.
- d) Quanto maior o seu valor, melhor é o seu desempenho. Por isso ele é um critério de maximização.

**Resposta certa:** b) Quanto maior o seu valor, pior é o seu desempenho. Por isso ele é um critério de minimização.

**Explicação:** A resposta é a que diz que quanto maior o valor, pior o desempenho, e por isso o critério é de minimização. Esse é o critério de custo. Na aula, o critério de lucro é aquele em que quanto maior, melhor (maximização), e o monotônico de custo é o oposto.

**Fonte:** Aula de Avaliação com dados quantitativos, pág. 82

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 158476-1-8
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

O artigo seminal do Método AHP foi publicado no ano de:

- a) 1977
- b) 1991
- c) 1968
- d) 1984

**Resposta certa:** a) 1977

**Explicação:** A resposta é 1977, ano do artigo seminal de Saaty, A scaling method for priorities in hierarchical structures, no Journal of Mathematical Psychology. O AHP foi desenvolvido na década de 1970.

**Fonte:** Aula de Artigo seminal sobre o AHP, pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-1-9
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

Assinale a opção que preenche corretamente a lacuna da sentença a seguir: “Saaty fornece os valores de RI para matrizes quadradas de ordem 1 até_____”.

- a) 10
- b) 15
- c) 9
- d) 7

**Resposta certa:** b) 15

**Explicação:** A resposta é 15. A tabela de Saaty para o índice randômico (RI) vai das matrizes de ordem 1 a 15, com RI de 0, 0, 0,58, 0,9, 1,12 e assim por diante até 1,59 na ordem 15.

**Fonte:** Aula de Teste de Consistência (AHP), pág. 41

**Situação:** explicação conferida com o material das aulas

---

### Questão 158476-2-3
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

No Método AHP, por que devemos normalizar a Matriz de Decisão?

- a) Para que se possa utilizar a Curva Normal Padronizada.
- b) Para que se possa realizar a comparação par a par entre os critérios.
- c) Para calcular o Índice Randômico de cada matriz quadrada.
- d) Para tornar todos os elementos da matriz adimensionais, ou seja, sem unidades de medida, já que o método AHP é um método de agregação.

**Resposta certa:** d) Para tornar todos os elementos da matriz adimensionais, ou seja, sem unidades de medida, já que o método AHP é um método de agregação.

**Explicação:** A resposta é tornar os elementos adimensionais. Os critérios têm unidades diferentes (reais, megapixels, horas), e como o AHP agrega tudo em uma nota final, é preciso tirar as unidades antes de somar. Normalizar não tem a ver com curva normal, comparação par a par ou índice randômico.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 158476-2-5
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

Um decisor, ao se deparar com um problema complexo, decidiu modelá-lo com o método AHP. Usando a Escala Fundamental de Saaty, ao comparar dois critérios, ele estabeleceu o valor um 1 (um). Isso quer dizer que:

- a) Um critério é muito menos importante que o outro.
- b) Ambos os critérios são igualmente importantes.
- c) Um critério é absolutamente mais importante que o outro.
- d) Um critério é muito mais importante que o outro.

**Resposta certa:** b) Ambos os critérios são igualmente importantes.

**Explicação:** A resposta é que ambos os critérios são igualmente importantes. Na escala fundamental de Saaty, o valor 1 corresponde a igualdade. Os valores 3, 5, 7 e 9 indicam importância crescente de um sobre o outro.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 158476-2-9
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

Das sentenças a seguir, assinale a única alternativa INCORRETA:

- a) A Pesquisa Operacional é uma ciência que pode ser aplicada para a solução de problemas reais da sociedade.
- b) A Pesquisa Operacional pode ser utilizada no gerenciamento de sistemas complexos.
- c) A Pesquisa Operacional lança mão de uma abordagem empírica, ou seja, não trabalha com métodos estritamente científicos.
- d) A Pesquisa Operacional é uma abordagem científica.

**Resposta certa:** c) A Pesquisa Operacional lança mão de uma abordagem empírica, ou seja, não trabalha com métodos estritamente científicos.

**Explicação:** A incorreta é a que diz que a Pesquisa Operacional é empírica e não usa métodos estritamente científicos. A PO é uma abordagem científica, que usa modelagem matemática e métodos analíticos para apoiar decisões e resolver problemas reais em sistemas complexos, o que torna as outras três afirmações verdadeiras.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 158476-3-4
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos I

No processo de agregação do método AHP, já na etapa final do método, devemos multiplicar:

- a) A Matriz de Julgamentos pelo Vetor Prioridade dos Critérios.
- b) A Razão de Consistência pelo valor de Lâmbda.
- c) A Matriz de Julgamentos pelo Índice Randômico.
- d) A Matriz de Decisão Normalizada pelo Vetor Prioridade dos Critérios.

**Resposta certa:** d) A Matriz de Decisão Normalizada pelo Vetor Prioridade dos Critérios.

**Explicação:** A resposta é multiplicar a matriz de decisão normalizada pelo vetor prioridade dos critérios. Na agregação, as prioridades das alternativas em cada critério são ponderadas pelos pesos dos critérios e somadas (soma de wj·aij). Ponderar a matriz de julgamentos pelo vetor prioridade é um passo anterior, da análise de consistência (cálculo do lâmbda).

**Fonte:** Aula de Estrutura axiomática do AHP, pág. 47

**Situação:** explicação conferida com o material das aulas

---

## Modelagem Matemática e Estruturação de Problemas Complexos II

### Questão 159075-1-1
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

No Método AHP-Gaussiano, por que a Matriz de Decisão precisa ser normalizada?

- a) Para que se possa calcular o Laplaciano da matriz de decisão.
- b) Para que se possa calcular uma média geométrica em cada linha da matriz.
- c) Para que exista a matriz inversa da matriz de decisão.
- d) Para que todos os valores da matriz se tornem adimensionais.

**Resposta certa:** d) Para que todos os valores da matriz se tornem adimensionais.

**Explicação:** A resposta é que a normalização deixa todos os valores adimensionais. As alternativas são medidas em unidades diferentes em cada critério, e só depois de tirar as unidades é possível agregar os critérios numa nota única. Não é por exigência de média geométrica, inversa ou laplaciano.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 159075-1-10
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

O Método AHP-Gaussiano apresenta uma nova abordagem em relação ao método original, baseada em uma:

- a) Nova razão de consistência, que deve ser maior ou igual a 20%.
- b) Escala de 0 a 10 para atribuição dos pesos dos critérios.
- c) Matriz de ponderações proveniente da comparação paritária entre os critérios.
- d) Análise de sensibilidade proveniente do fator gaussiano.

**Resposta certa:** d) Análise de sensibilidade proveniente do fator gaussiano.

**Explicação:** A resposta é "análise de sensibilidade proveniente do fator gaussiano". É isso que o AHP-Gaussiano acrescenta ao método original. A matriz de comparação paritária e a escala de Saaty já existem no AHP clássico, e a razão de consistência de 20% ou mais não faz sentido, já que quanto menor a razão, melhor a consistência.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 159075-1-2
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

Como referência, a primeira vez que o método AHP-Gaussiano apareceu foi:

- a) No Simpósio de Excelência em Gestão e Tecnologia (SEGeT 2021).
- b) No Simpósio Brasileiro de Pesquisa Operacional (SBPO 2016).
- c) No Encontro Nacional de Engenharia de Produção (ENEGEP 2019).
- d) No Encontro da ANPAD (EnANPAD 2015).

**Resposta certa:** b) No Simpósio Brasileiro de Pesquisa Operacional (SBPO 2016).

**Explicação:** O gabarito indica o SBPO 2016, mas nenhum trecho recebido traz a origem do AHP-Gaussiano, e a referência é um dado bibliográfico que não dá para deduzir. O que a aula traz é o AHP clássico e os dados do professor, sem essa informação.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** Dado bibliográfico (onde o AHP-Gaussiano apareceu primeiro) sem apoio nos trechos recebidos.

---

### Questão 159075-1-3
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

No método AHP-Gaussiano, o fator gaussiano é calculado da seguinte maneira:

- a) Dividindo-se o desvio padrão pela média das alternativas dentro de cada critério.
- b) Dividindo-se a média pela amplitude das alternativas dentro de cada critério.
- c) Dividindo-se a variância pela média das alternativas dentro de cada critério.
- d) Dividindo-se a moda pela amplitude das alternativas dentro de cada critério.

**Resposta certa:** a) Dividindo-se o desvio padrão pela média das alternativas dentro de cada critério.

**Explicação:** A resposta é dividir o desvio padrão pela média das alternativas dentro de cada critério. É o coeficiente de variação, que mede a dispersão relativa e dá mais peso aos critérios em que as alternativas mais se diferenciam. Variância sobre média, média sobre amplitude e moda sobre amplitude não têm esse sentido.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 159075-1-4
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

Todas as opções a seguir indicam “pontos fortes” do Método AHP-Gaussiano, exceto:

- a) É um método novo, publicado no ano de 2021.
- b) Aplicável em inúmeros problemas gerenciais do cotidiano.
- c) Existem várias ferramentas computacionais gratuitas que viabilizam a utilização do método.
- d) Exige maior esforço cognitivo do tomador de decisão.

**Resposta certa:** d) Exige maior esforço cognitivo do tomador de decisão.

**Explicação:** A resposta é "Exige maior esforço cognitivo do tomador de decisão" porque isso é uma fraqueza, não uma força. A ideia do AHP-Gaussiano é justamente reduzir o esforço do decisor em relação ao AHP clássico, que depende de muitas comparações par a par. As outras três opções (método recente, ampla aplicabilidade e ferramentas gratuitas) são vantagens.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 159075-1-6
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

Com relação aos pontos fortes do método AHP-Gaussiano, podemos afirmar que:

I.	É um método que nos possibilita trabalhar com um grande volume de dados.

II.	Exige menor esforço cognitivo por parte do decisor.

III.	Trabalha com a Escala Fundamental de Saaty.

Assinale a opção CORRETA:
Com relação aos pontos fortes do método AHP-Gaussiano, podemos afirmar que:
I.	É um método que nos possibilita trabalhar com um grande volume de dados.
II.	Exige menor esforço cognitivo por parte do decisor.
III.	Trabalha com a Escala Fundamental de Saaty.
Assinale a opção CORRETA:

- a) Todos os enunciados estão corretos.
- b) Os enunciados I e III estão corretos.
- c) Somente o enunciado I está correto.
- d) Somente os enunciados I e II estão corretos.

**Resposta certa:** d) Somente os enunciados I e II estão corretos.

**Explicação:** A resposta é "Somente I e II estão corretas". O AHP-Gaussiano consegue lidar com muitos dados e pede menos esforço do decisor, porque dispensa as comparações paritárias do AHP clássico. O item III é a armadilha: a Escala Fundamental de Saaty é do AHP original (pág. 30 da aula), e o Gaussiano a dispensa.

**Fonte:** Aula de Método AHP, pág. 30

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 159075-1-7
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

Assinale a opção que preenche corretamente a sentença a seguir:

“O Método AHP-Gaussiano apresenta uma nova abordagem ao método original, baseada em uma análise de sensibilidade proveniente do _________”.
Assinale a opção que preenche corretamente a sentença a seguir:
“O Método AHP-Gaussiano apresenta uma nova abordagem ao método original, baseada em uma análise de sensibilidade proveniente do _________”.

- a) Fator Gaussiano.
- b) Valor de Lâmbda.
- c) Índice de Consistência.
- d) Laplaciano da Matriz.

**Resposta certa:** a) Fator Gaussiano.

**Explicação:** A resposta é "Fator Gaussiano". A novidade do AHP-Gaussiano em relação ao AHP original é uma análise de sensibilidade feita a partir desse fator, que gera os pesos dos critérios. Valor de lâmbda e índice de consistência pertencem ao AHP clássico, e o laplaciano da matriz não faz parte do método.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 159075-1-8
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

Considerando o Método AHP-Gaussiano, o processo de agregação consiste em:

- a) Multiplicar a Matriz de Decisão Normalizada pelo Vetor de Pesos dos Critérios.
- b) Somar a Matriz de Decisão Normalizada com o Vetor de Pesos dos Critérios.
- c) Agregar a Matriz de Decisão com a Matriz de Julgamentos de Saaty.
- d) Calcular a Matriz Inversa da Matriz de Decisão.

**Resposta certa:** a) Multiplicar a Matriz de Decisão Normalizada pelo Vetor de Pesos dos Critérios.

**Explicação:** A resposta é multiplicar a matriz de decisão normalizada pelo vetor de pesos dos critérios. Na agregação, cada prioridade da alternativa é ponderada pelo peso do critério correspondente e depois somada (soma de w_j vezes a_ij). Isso é um produto matricial, e não uma soma da matriz com o vetor.

**Fonte:** Aula de Método AHP, estrutura axiomática, pág. 47

**Situação:** explicação conferida com o material das aulas

---

### Questão 159075-1-9
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

O Método AHP-Gaussiano foi publicado no ano de 2021, na forma de um artigo científico, no periódico:

- a) Revista Pesquisa Operacional.
- b) IEEE Acess.
- c) International Journal of the Analytic Hierarchy Process (IJAHP).
- d) Scientometrics.

**Resposta certa:** c) International Journal of the Analytic Hierarchy Process (IJAHP).

**Explicação:** A resposta é o International Journal of the Analytic Hierarchy Process (IJAHP). A lista de leituras da aula traz o artigo de Dos Santos, Costa e Gomes (2021) sobre a seleção de navios de guerra com uma nova abordagem para o AHP, publicado nesse periódico.

**Fonte:** Aula de Método AHP, sugestões de leitura, pág. 118

**Situação:** explicação conferida com o material das aulas

---

### Questão 159075-2-1
Área 5 · Modelagem Matemática e Estruturação de Problemas Complexos II

No Método AHP-Gaussiano, deve-se normalizar o Fator Gaussiano para que:

- a) Os pesos dos critérios estejam em porcentagem, ou seja, o somatório dos pesos dos critérios seja igual a 100%.
- b) Todos os valores do vetor de pesos sejam maiores que 1.
- c) O vetor de pesos seja invertível.
- d) Se possa utilizar a Escala Fundamental de Saaty.

**Resposta certa:** a) Os pesos dos critérios estejam em porcentagem, ou seja, o somatório dos pesos dos critérios seja igual a 100%.

**Explicação:** A resposta é a que fala em pesos em porcentagem. Normalizar o fator gaussiano divide cada valor pela soma de todos, então os pesos dos critérios passam a somar 100%, ou 1. Normalizar não deixa os valores maiores que 1 (ficam entre 0 e 1) e não tem relação com invertibilidade nem com a escala de Saaty.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Pesquisa Operacional e Modelos de Otimização I

### Questão 196910-1-1
Área 5 · Pesquisa Operacional e Modelos de Otimização I

Em um modelo de Programação Linear Inteira (PLI), as variáveis de decisão devem assumir:

- a) Apenas valores inteiros, como 0, 1 ou 2.
- b) Valores contínuos ou inteiros, dependendo da variável.
- c) Apenas valores contínuos, como 0,73 ou 1,06.
- d) Apenas valores resultantes de funções trigonométricas.

**Resposta certa:** a) Apenas valores inteiros, como 0, 1 ou 2.

**Explicação:** A resposta é apenas valores inteiros. Na Programação Linear Inteira (PLI) todas as variáveis de decisão são números inteiros (0, 1, 2...). Valores como 0,73 ou 1,06 aparecem na versão mista (PLIM), que mistura contínuas e inteiras, e a PL comum trabalha só com contínuas.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-10
Área 5 · Pesquisa Operacional e Modelos de Otimização I

Considere o modelo matemático abaixo referente ao exemplo do corte de bobinas de aço abordado em aula e assinale a alternativa CORRETA:

Maximizar Z = 0,3x + 0,5y

x ≤ 4000
y ≤ 6000
3x + 2y ≤ 18000
x, y ≥ 0

- a) As inequações x ≤ 4000 e y ≤ 6000 representam a função objetivo do problema.
- b) x e y representam as variáveis de decisão do problema.
- c) Z representa uma restrição de disponibilidade de recursos do problema.
- d) Os coeficientes 0,3 e 0,5 representam as variáveis de decisão do problema.

**Resposta certa:** b) x e y representam as variáveis de decisão do problema.

**Explicação:** A resposta é que x e y são as variáveis de decisão: são os metros de fita de aço produzidos em cada máquina, o que o modelo precisa descobrir. Z é a função objetivo (lucro), x ≤ 4000 e y ≤ 6000 são restrições de capacidade, e 0,3 e 0,5 são só os coeficientes de lucro.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 74 e pág. 42

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-2
Área 5 · Pesquisa Operacional e Modelos de Otimização I

Um Modelo Matemático é definido como uma representação de uma realidade que utiliza:

- a) Expressões matemáticas.
- b) Simulações computacionais em tempo real.
- c) Gráficos e tabelas exclusivamente, sem uso de equações.
- d) Descrições verbais detalhadas do problema estudado.

**Resposta certa:** a) Expressões matemáticas.

**Explicação:** A resposta é expressões matemáticas. Um modelo é uma representação simplificada da realidade, e quando essa representação é feita com equações e inequações ele passa a ser um modelo matemático. Simulação, gráficos sem equação ou texto descritivo não caracterizam esse tipo de modelo.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-3
Área 5 · Pesquisa Operacional e Modelos de Otimização I

A Pesquisa Operacional (PO) teve origem histórica associada a qual contexto?

- a) À criação de softwares de gestão empresarial na década de 1980.
- b) Ao contexto da Segunda Guerra Mundial, com foco em otimizar o uso de recursos militares limitados em operações estratégicas e táticas.
- c) Ao movimento de padronização da produção industrial promovido por Henry Ford no início do século XX.
- d) Ao desenvolvimento de sistemas de IA na contabilidade em grandes corporações americanas no início do século XX.

**Resposta certa:** b) Ao contexto da Segunda Guerra Mundial, com foco em otimizar o uso de recursos militares limitados em operações estratégicas e táticas.

**Explicação:** A resposta é a Segunda Guerra Mundial. A PO nasceu quando cientistas foram chamados a aplicar métodos quantitativos em problemas militares de natureza estratégica e tática, para alocar de forma eficiente recursos escassos. As outras opções (software de gestão, Ford, IA na contabilidade) não têm relação com a origem do campo.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 9

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-4
Área 5 · Pesquisa Operacional e Modelos de Otimização I

Um Modelo de Otimização tem como principal característica o uso de técnicas matemáticas para:
Um Modelo de Otimização tem como principal característica o uso de técnicas matemáticas para:

- a) Prever eventos futuros de forma totalmente aleatória.
- b) Identificar a melhor solução (ótima) possível para um problema.
- c) Armazenar todas as soluções possíveis de um problema, sem compará-las.
- d) Descrever qualitativamente as causas de um problema.

**Resposta certa:** b) Identificar a melhor solução (ótima) possível para um problema.

**Explicação:** A resposta é identificar a melhor solução (ótima) possível para o problema. Modelo de otimização é um modelo matemático feito justamente para buscar o ótimo, maximizando ou minimizando uma função objetivo dentro das restrições. Ele não prevê eventos aleatórios nem só descreve causas.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-5
Área 5 · Pesquisa Operacional e Modelos de Otimização I

A restrição "Toneladas embarcadas ≥ Mínimo a ser embarcado" representa um exemplo de restrição de:

- a) Desempenho mínimo.
- b) Limitação de quantidade de recursos.
- c) Conservação.
- d) Variável de decisão.

**Resposta certa:** a) Desempenho mínimo.

**Explicação:** A resposta é desempenho mínimo. A restrição obriga a atingir uma meta ou quantidade mínima, e o sinal ≥ é a marca disso: toneladas embarcadas têm de ser pelo menos o mínimo a embarcar. A limitação de recursos é a que usa ≤, ou seja, não pode gastar mais do que o disponível.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-6
Área 5 · Pesquisa Operacional e Modelos de Otimização I

De acordo com a definição apresentada em aula, um Modelo pode ser descrito como:

- a) Um relatório final que documenta os resultados de uma pesquisa operacional.
- b) Um conjunto de dados históricos coletados sobre um problema específico.
- c) Uma representação explícita e simplificada de uma realidade, usada para compreender, modificar, administrar e controlar essa realidade.
- d) Uma cópia idêntica e completa de uma realidade, sem qualquer simplificação.

**Resposta certa:** c) Uma representação explícita e simplificada de uma realidade, usada para compreender, modificar, administrar e controlar essa realidade.

**Explicação:** A resposta é a representação explícita e simplificada de uma realidade, usada para compreender, modificar, administrar e controlar essa realidade. A palavra chave é simplificada: um modelo não é cópia idêntica da realidade, nem um relatório, nem apenas um banco de dados históricos.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-7
Área 5 · Pesquisa Operacional e Modelos de Otimização I

A restrição "número de unidades entrando = número de unidades saindo" é classificada como uma restrição de:

- a) Limitação de quantidade de recursos.
- b) Conservação.
- c) Disponibilidade máxima.
- d) Desempenho mínimo.

**Resposta certa:** b) Conservação.

**Explicação:** A resposta é conservação. Quando o que entra tem de ser igual ao que sai (unidades entrando = unidades saindo), a restrição só garante o balanço do fluxo. As de limitação de recursos e de disponibilidade máxima usam ≤, e a de desempenho mínimo usa ≥.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-8
Área 5 · Pesquisa Operacional e Modelos de Otimização I

Qual das opções abaixo representa um exemplo de equação encontrada em um modelo de Programação Não Linear (PNL)?

- a) 5x1 − 2x2 + 10 (combinação linear com termo constante).
- b) 2x1 + 3x2 (soma de variáveis com coeficientes constantes).
- c) 3x1x2 (multiplicação de variáveis).
- d) x1 (variável isolada, sem coeficiente).

**Resposta certa:** c) 3x1x2 (multiplicação de variáveis).

**Explicação:** A resposta é 3x1x2. Na PNL aparecem multiplicação entre variáveis, polinômios (como x1 ao quadrado) e funções como seno e cosseno. As demais opções são combinações lineares: soma de variáveis com coeficientes constantes, e o termo constante ou a variável isolada não quebram a linearidade.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 196910-1-9
Área 5 · Pesquisa Operacional e Modelos de Otimização I

Considere os conceitos discutidos em aula e assinale a alternativa INCORRETA:

- a) O primeiro passo em modelagem matemática de otimização é formular o problema, isto é, definir claramente o problema.
- b) As restrições são equações ou inequações que limitam os valores das variáveis de decisão.
- c) Em Programação Linear (PL), todas as equações devem ser não-lineares.
- d) A função objetivo é a equação que representa a medida de desempenho a ser maximizada ou minimizada.

**Resposta certa:** c) Em Programação Linear (PL), todas as equações devem ser não-lineares.

**Explicação:** A incorreta é a que diz que em PL todas as equações devem ser não-lineares. É o contrário: na Programação Linear a função objetivo e as restrições são expressões lineares, no formato c1x1 + c2x2 + ... + cnxn. Equações não-lineares caracterizam a PNL.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 23

**Situação:** explicação conferida com o material das aulas

---

## Pesquisa Operacional e Modelos de Otimização II

### Questão 198241-1-1
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Sobre o método de Enumeração para solução de modelos de otimização, é correto afirmar que:

- a) Só pode ser aplicado a problemas com exatamente duas variáveis de decisão.
- b) É o método mais indicado para problemas com infinitas combinações possíveis de solução.
- c) Percorre exclusivamente os vértices da região factível para encontrar a solução ótima.
- d) Torna-se inviável para problemas com infinitas combinações possíveis de solução.

**Resposta certa:** d) Torna-se inviável para problemas com infinitas combinações possíveis de solução.

**Explicação:** A resposta é que a enumeração se torna inviável quando há infinitas combinações possíveis. Como x e y são contínuas, existem infinitos pares candidatos e não dá para testar um por um. Percorrer só os vértices é o que o Simplex faz, e não há limite de duas variáveis para enumerar.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 10

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-10
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Sobre o Método Simplex para solução de modelos de programação linear, é correto afirmar que:

- a) É viável apenas para problemas com duas variáveis de decisão.
- b) Não pode ser aplicado quando há mais de uma restrição no modelo.
- c) Percorre os vértices da região factível para encontrar a melhor solução.
- d) Consiste em testar todas as combinações possíveis de solução, uma a uma.

**Resposta certa:** c) Percorre os vértices da região factível para encontrar a melhor solução.

**Explicação:** A resposta é que o Simplex percorre os vértices da região factível até a função objetivo não poder mais ser melhorada. Ele serve para qualquer número de variáveis e de restrições, e justamente evita testar todas as combinações uma a uma.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 56 e pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-2
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Julgue os itens sobre o método Simplex e assinale a alternativa CORRETA:

( ) O método Simplex é aplicável mesmo quando há mais de duas variáveis e múltiplas restrições.
( ) O método Simplex garante que a função objetivo será maximizada ou minimizada mesmo fora da região factível.
( ) O Simplex percorre os vértices da região factível em busca da solução ótima.
( ) A função objetivo é irrelevante no processo iterativo do Simplex.

- a) V, F, V, F
- b) V, F, F, F
- c) F, F, V, V
- d) V, V, F, F

**Resposta certa:** a) V, F, V, F

**Explicação:** A sequência é V, F, V, F. O Simplex vale para qualquer número de variáveis e restrições e anda pelos vértices da região factível até a função objetivo não poder mais melhorar. Ele nunca sai da região factível, e a função objetivo é o que guia cada iteração, então não é irrelevante.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 56; Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 88

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-3
Área 5 · Pesquisa Operacional e Modelos de Otimização II

A respeito da representação gráfica de um modelo de programação linear com duas variáveis de decisão, é correto afirmar que:

- a) A região factível é composta pelo conjunto de soluções que satisfazem simultaneamente todas as restrições.
- b) A região factível é o ponto em que todas as retas das restrições se cruzam.
- c) A função objetivo não pode ser representada graficamente em modelos lineares.
- d) A solução ótima ocorre sempre fora da região factível.

**Resposta certa:** a) A região factível é composta pelo conjunto de soluções que satisfazem simultaneamente todas as restrições.

**Explicação:** A resposta é que a região factível é o conjunto de soluções que atendem a todas as restrições ao mesmo tempo, inclusive as de não negatividade. Não é um ponto, e a solução ótima é a melhor solução dentro dessa região, nunca fora dela. A função objetivo também pode ser desenhada, como retas paralelas.

**Fonte:** Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 75

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-4
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Em relação ao uso da biblioteca PuLP em Python para resolver problemas de otimização linear, assinale a afirmativa correta:

- a) O método LpProblem é usado apenas para modelos de minimização.
- b) A biblioteca PuLP não permite imposição de restrições, sendo apenas para análise gráfica.
- c) As variáveis de decisão devem ser definidas com LpVariable, podendo incluir limites.
- d) A função objetivo deve ser inserida antes das variáveis de decisão.

**Resposta certa:** c) As variáveis de decisão devem ser definidas com LpVariable, podendo incluir limites.

**Explicação:** A resposta é que as variáveis de decisão são criadas com LpVariable, e podem receber limite inferior e superior (lowBound, upBound) e o tipo (contínua, inteira ou binária). O LpProblem aceita maximização e minimização, o PuLP impõe restrições com prob += ... e o modelo é definido antes das variáveis ou da função objetivo.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 36

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-5
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Considere o trecho de código abaixo escrito com a biblioteca PuLP em Python para resolver um modelo de programação linear. Com base no código abaixo, assinale a alternativa CORRETA:

[imagem: imagens/198241_1_5_0.jpg]

- a) O modelo é de minimização e considera duas variáveis inteiras.
- b) A restrição de mão de obra é expressa pela desigualdade 3x+2y≥18000.
- c) A biblioteca utilizada exige variáveis discretas por padrão.
- d) O modelo considera maximizar o lucro com duas variáveis contínuas.

**Resposta certa:** d) O modelo considera maximizar o lucro com duas variáveis contínuas.

**Explicação:** O código usa LpProblem com LpMaximize e a função objetivo 0.3*x + 0.5*y, que é um lucro a maximizar. As variáveis x e y são criadas só com lowBound=0, sem cat='Integer', então são contínuas (o padrão do PuLP). A restrição de mão de obra é 3x + 2y <= 18000, e não >=.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-6
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Julgue os itens a seguir como verdadeiros (V) ou falsos (F) e assinale a alternativa CORRETA:

( ) O Solver do Excel permite resolver problemas de programação linear de forma gráfica.
( ) O pacote PuLP em Python permite modelar e resolver problemas de otimização por meio de programação.
( ) Softwares como o Solver e o PuLP dispensam a necessidade de o usuário definir corretamente a função objetivo e as restrições do modelo.

- a) F, V, F
- b) F, F, V
- c) V, V, V
- d) V, F, F

**Resposta certa:** a) F, V, F

**Explicação:** A sequência é F, V, F. O Solver é um suplemento do Excel que resolve com algoritmos (Simplex para PL), não de forma gráfica. O PuLP permite modelar e resolver em Python. Nenhum dos dois dispensa o usuário de definir corretamente função objetivo e restrições, pois eles só executam o modelo que você escreve.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 28; Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 131

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-7
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Sobre o Método Gráfico para solução de modelos de programação linear, é correto afirmar que:

- a) É viável apenas para problemas com duas variáveis de decisão.
- b) Pode ser aplicado a problemas com qualquer número de variáveis de decisão.
- c) É o método utilizado por softwares para resolver problemas de grande porte.
- d) Consiste em enumerar todas as combinações possíveis de solução.

**Resposta certa:** a) É viável apenas para problemas com duas variáveis de decisão.

**Explicação:** A resposta é a que limita o método gráfico a duas variáveis, pois cada variável vira um eixo do plano. A literatura admite três variáveis com bem mais complexidade, mas de qualquer forma ele não serve para qualquer número de variáveis nem para problemas de grande porte, e enumerar tudo não é o que o método faz.

**Fonte:** Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 75

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-8
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Em relação ao uso do Solver no Excel para resolver modelos de programação linear, é INCORRETO afirmar que:

- a) O Solver é adequado apenas para problemas com duas variáveis.
- b) O Solver permite definir a função objetivo e as restrições do modelo.
- c) O Solver utiliza métodos como o Simplex para encontrar soluções ótimas.
- d) É necessário instalar o suplemento Solver nas opções do Excel.

**Resposta certa:** a) O Solver é adequado apenas para problemas com duas variáveis.

**Explicação:** A incorreta é que o Solver só serve para duas variáveis. O Solver é um suplemento do Excel (que precisa ser ativado), permite definir objetivo e restrições e usa Simplex em PL, GRG2 em não linear. É mais indicado para problemas de pequeno porte, mas não tem limite de duas variáveis, ao contrário do método gráfico.

**Fonte:** Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 131

**Situação:** explicação conferida com o material das aulas

---

### Questão 198241-1-9
Área 5 · Pesquisa Operacional e Modelos de Otimização II

Considere os conceitos relacionados ao método Simplex e assinale a alternativa CORRETA:

- a) O método Simplex calcula todas as soluções possíveis e escolhe a de menor custo.
- b) O método Simplex percorre pontos aleatórios da região factível até encontrar um ótimo local.
- c) O método Simplex explora os vértices da região factível em busca da solução que otimiza a função objetivo.
- d) O método Simplex só é aplicável a modelos com duas variáveis de decisão.

**Resposta certa:** c) O método Simplex explora os vértices da região factível em busca da solução que otimiza a função objetivo.

**Explicação:** A resposta é que o Simplex explora os vértices da região factível em busca da solução que otimiza a função objetivo. Ele não calcula todas as soluções (isso seria enumeração), não anda em pontos aleatórios e vale para qualquer número de variáveis, não só duas.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 56

**Situação:** explicação conferida com o material das aulas

---

## Pesquisa Operacional e Modelos de Otimização III

### Questão 198832-1-1
Área 5 · Pesquisa Operacional e Modelos de Otimização III

A Pesquisa Operacional pode ser definida como uma abordagem que utiliza métodos científicos e matemáticos para apoiar a tomada de decisão. Assinale a alternativa CORRETA sobre os elementos de um modelo de otimização.

- a) Restrições são as condições ou limitações que uma solução deve respeitar, enquanto as variáveis de decisão representam os valores fixos e conhecidos do problema, definidos antes da resolução do modelo.
- b) A função objetivo representa as limitações de recursos disponíveis, enquanto as restrições indicam o que se deseja maximizar ou minimizar no modelo.
- c) As variáveis de decisão são valores fixos fornecidos pelo problema, enquanto os parâmetros são os valores que o modelo busca determinar na solução ótima.
- d) Restrições são as condições ou limitações que uma solução deve respeitar, enquanto a função objetivo é a medida (a ser maximizada ou minimizada) usada para comparar as soluções viáveis.

**Resposta certa:** d) Restrições são as condições ou limitações que uma solução deve respeitar, enquanto a função objetivo é a medida (a ser maximizada ou minimizada) usada para comparar as soluções viáveis.

**Explicação:** A resposta é a que define as restrições como condições a respeitar e a função objetivo como a medida maximizada ou minimizada para comparar as soluções viáveis. As outras trocam os papéis: as variáveis de decisão são justamente o que o modelo busca determinar, e os valores fixos são os parâmetros.

**Fonte:** Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 75

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-10
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Considere o problema de otimização inteira abaixo e assinale a alternativa CORRETA.

Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.
Considere o problema de otimização inteira abaixo e assinale a alternativa CORRETA.
Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.

- a) A função objetivo é maximizar apenas as unidades em capa mole das caixas leves.
- b) A função objetivo é minimizar a quantidade de livros entregues (acondicionados em caixas diferentes).
- c) A função objetivo é maximizar a quantidade de livros entregues (acondicionados em caixas diferentes).
- d) A função objetivo é maximizar o número total de caixas enviadas pelo CD, sem considerar a quantidade de livros em cada uma.

**Resposta certa:** c) A função objetivo é maximizar a quantidade de livros entregues (acondicionados em caixas diferentes).

**Explicação:** A resposta é maximizar a quantidade de livros entregues. Cada caixa leve traz 6 livros e cada mista 7, e o CD quer atender da melhor forma possível a demanda, o que leva à função Q = 6L + 7M a maximizar. Não é contar só caixas, nem só capa mole, nem minimizar.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 198832-1-2
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Além do método gráfico, problemas de programação linear inteira podem ser resolvidos por outros métodos, dentre eles:

- a) Algoritmo Branch-and-Bound.
- b) Método AHP (Analytic Hierarchy Process)
- c) Método Simplex.
- d) Método K-means.

**Resposta certa:** a) Algoritmo Branch-and-Bound.

**Explicação:** A resposta é o Branch-and-Bound, que é o método exato clássico para programação inteira: resolve o problema relaxado (sem exigir inteiros) e vai ramificando até achar o melhor inteiro. O Simplex tenta, mas sozinho devolve soluções fracionárias, e AHP e K-means não são métodos de otimização linear.

**Fonte:** Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 370

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-3
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Considere o problema de otimização inteira abaixo e assinale a alternativa que apresenta a solução ótima a partir da resolução pelo método gráfico.

Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.
Considere o problema de otimização inteira abaixo e assinale a alternativa que apresenta a solução ótima a partir da resolução pelo método gráfico.
Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.

- a) Serão 60 livros entregues, acondicionados em 10 caixas leves e nenhuma caixa mista.
- b) Serão 64 livros entregues, acondicionados em 6 caixas leves e 4 caixas mistas.
- c) Serão 65 livros entregues, acondicionados em 5 caixas leves e 5 caixas mistas.
- d) Serão 71 livros entregues, acondicionados em 6 caixas leves e 5 caixas mistas.

**Resposta certa:** c) Serão 65 livros entregues, acondicionados em 5 caixas leves e 5 caixas mistas.

**Explicação:** A resposta é 65 livros. Com L caixas leves (6 capa mole) e M mistas (7 livros), L + M ≤ 10, M ≤ 7, capa mole 40 + 6L + 2M ≥ 80 e capa dura 65 + 5M ≥ 80 (M ≥ 3). Maximizando 6L + 7M, M = 6 ou 7 deixa a capa mole abaixo de 80; L = 5 e M = 5 dá 6·5 + 2·5 = 40 e Q = 30 + 35 = 65.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 198832-1-4
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Considere o problema de otimização inteira abaixo e sua respectiva modelagem matemática. Em seguida, assinale a alternativa que apresenta a restrição de livros de capa mole.

Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.

Modelagem matemática:

Maximizar ?? = 6?? + 7?? (?? é a Quantidade de caixas leves e ?? é a Quantidade de caixas mistas)

sujeito a: 
?? +??≤ 10 
?? ≤7 
6?? +2?? ≥ 40 
?? ≥ 3 
??, ?? ∈ Z+
Considere o problema de otimização inteira abaixo e sua respectiva modelagem matemática. Em seguida, assinale a alternativa que apresenta a restrição de livros de capa mole.
Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.
Modelagem matemática:
Maximizar ?? = 6?? + 7?? (?? é a Quantidade de caixas leves e ?? é a Quantidade de caixas mistas)
sujeito a: 
?? +??≤ 10 
?? ≤7 
6?? +2?? ≥ 40 
?? ≥ 3 
??, ?? ∈ Z+

- a) Minimizar Q = 6L + 7M
- b) 6L + 2M ≥ 40
- c) Maximizar Q = 6L + 7M
- d) L + M ≤ 10

**Resposta certa:** b) 6L + 2M ≥ 40

**Explicação:** A resposta é 6L + 2M ≥ 40. Capa mole só vem das caixas leves (6 cada) e das mistas (2 cada), e a livraria já tem 40 e precisa de pelo menos 80, então faltam 40: 6L + 2M ≥ 40. L + M ≤ 10 é o total de caixas, e as duas que começam com Minimizar ou Maximizar são a função objetivo.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 54

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-5
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Muitas vezes, resolver os problemas graficamente não é viável pelo alto número de variáveis e restrições. Assinale a alternativa que apresenta pacotes e softwares para resolução de problemas de otimização.

- a) TensorFlow e Scikit-learn.
- b) MATLAB e Matplotlib.
- c) Solver e PuLP.
- d) SPSS e Power BI.

**Resposta certa:** c) Solver e PuLP.

**Explicação:** A resposta é Solver e PuLP. Quando o problema tem muitas variáveis e restrições, resolver no gráfico não é viável, e se usam o Solver do Excel e pacotes como o PuLP, que implementam o Simplex. TensorFlow, Scikit-learn, Matplotlib, SPSS e Power BI não são ferramentas de otimização.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 28

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-6
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Considere o modelo matemático abaixo e assinale a alternativa INCORRETA:

Minimizar ?? = 0,3?? + 0,5??

Sujeito a:

?? ≤ 4000
?? ≤ 6000
3?? + 2?? ≤ 18000
??, ?? ≥ 0
Considere o modelo matemático abaixo e assinale a alternativa INCORRETA:
Minimizar ?? = 0,3?? + 0,5??
Sujeito a:
?? ≤ 4000
?? ≤ 6000
3?? + 2?? ≤ 18000
??, ?? ≥ 0

- a) Um método que pode ser utilizado para encontrar a solução ótima é o Simplex.
- b) Como o problema tem duas variáveis de decisão, pode ser resolvido pelo método gráfico.
- c) A função objetivo é Minimizar Z = 0,3x + 0,5y.
- d) Como o problema é de minimização, o ideal é que as variáveis de decisão assumam valores negativos.

**Resposta certa:** d) Como o problema é de minimização, o ideal é que as variáveis de decisão assumam valores negativos.

**Explicação:** A incorreta é a que diz que na minimização o ideal seria ter variáveis negativas. O modelo exige x, y ≥ 0, então valores negativos nem são permitidos. As outras são corretas: o Simplex serve, duas variáveis permitem o método gráfico e a função objetivo é de fato Minimizar Z = 0,3x + 0,5y.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 9

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-7
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Considere o problema de otimização inteira abaixo e sua respectiva modelagem matemática. Em seguida, assinale a alternativa que apresenta a restrição do total de caixas.

Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.

Modelagem matemática:

Maximizar ?? = 6?? + 7?? (?? é a Quantidade de caixas leves e ?? é a Quantidade de caixas mistas)

sujeito a: 
?? +??≤ 10 
?? ≤7 
6?? +2?? ≥ 40 
?? ≥ 3 
??, ?? ∈ Z+
Considere o problema de otimização inteira abaixo e sua respectiva modelagem matemática. Em seguida, assinale a alternativa que apresenta a restrição do total de caixas.
Problema: Uma livraria venderá um novo livro que está sendo lançado em duas versões, com capa mole e capa dura, tendo recebido 40 cópias na primeira versão e 65 cópias da segunda. Entretanto, precisa de pelo menos 80 cópias de cada versão para atender pedidos já feitos e, se possível, cópias adicionais para atender a demanda dos interessados na abertura da loja. Um Centro de Distribuição (CD) precisa planejar as entregas para atender da melhor forma possível a demanda da livraria, sendo possível enviar até 10 caixas de livros para atender a essa demanda em que cada caixa de livro do tipo leve possui 6 unidades em capa mole. O CD também possui 7 caixas de livros mistas, sendo que cada caixa é composta por 5 unidades em capa dura e 2 unidades em capa mole.
Modelagem matemática:
Maximizar ?? = 6?? + 7?? (?? é a Quantidade de caixas leves e ?? é a Quantidade de caixas mistas)
sujeito a: 
?? +??≤ 10 
?? ≤7 
6?? +2?? ≥ 40 
?? ≥ 3 
??, ?? ∈ Z+

- a) L, M ∈ Z+
- b) L + M ≤ 10
- c) M ≥ 3
- d) M ≤ 7

**Resposta certa:** b) L + M ≤ 10

**Explicação:** A resposta é L + M ≤ 10. O enunciado diz que dá para enviar até 10 caixas no total, então a soma de leves e mistas fica limitada em 10. M ≤ 7 é só o limite de caixas mistas disponíveis, M ≥ 3 vem da capa dura e L, M ∈ Z+ é o domínio das variáveis.

**Fonte:** Aula de Pesquisa Operacional (11/08), pág. 54

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-8
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Assinale a alternativa CORRETA sobre o método Simplex:

- a) Percorre todos os pontos internos da região factível, calculando a função objetivo em cada um deles até encontrar o valor ótimo.
- b) Encontra a solução ótima apenas em problemas com duas variáveis de decisão, sendo substituído pelo método gráfico em dimensões maiores.
- c) Garante encontrar a solução ótima apenas em problemas de programação inteira, não sendo aplicável a problemas de programação linear contínua.
- d) Percorre os vértices da região factível até que a função objetivo não possa ser melhorada considerando as restrições do modelo.

**Resposta certa:** d) Percorre os vértices da região factível até que a função objetivo não possa ser melhorada considerando as restrições do modelo.

**Explicação:** A resposta é que o Simplex percorre os vértices da região factível até a função objetivo não poder mais ser melhorada, respeitando as restrições. Ele não varre os pontos internos, não se limita a duas variáveis (o gráfico é que tem esse limite) e é feito justamente para PL contínua.

**Fonte:** Aula de Pesquisa Operacional (18/08), pág. 56

**Situação:** explicação conferida com o material das aulas

---

### Questão 198832-1-9
Área 5 · Pesquisa Operacional e Modelos de Otimização III

Assinale a alternativa CORRETA sobre o conceito de região factível no método gráfico:

- a) É o conjunto formado apenas pelos vértices da área delimitada pelas restrições, excluindo os demais pontos internos e das arestas.
- b) É o conjunto de todos os pontos que satisfazem a função objetivo, independentemente de atenderem às restrições do modelo.
- c) É o ponto único em que a função objetivo atinge seu valor ótimo, respeitando todas as restrições do modelo.
- d) É o conjunto de todos os pontos (soluções) que satisfazem simultaneamente todas as restrições do modelo, incluindo as condições de não negatividade das variáveis.

**Resposta certa:** d) É o conjunto de todos os pontos (soluções) que satisfazem simultaneamente todas as restrições do modelo, incluindo as condições de não negatividade das variáveis.

**Explicação:** A resposta é o conjunto de todos os pontos que satisfazem ao mesmo tempo todas as restrições, incluindo a não negatividade. Não são só os vértices, não depende da função objetivo e não é um ponto único: o ótimo é um ponto escolhido dentro dessa região.

**Fonte:** Pesquisa Operacional para Cursos de Engenharia (Belfiore e Fávero), pág. 75

**Situação:** explicação conferida com o material das aulas

---

## Social Network Analysis I

### Questão 153880-1-1
Área 5 · Social Network Analysis I

Avalie a rede abaixo e responda: qual é o degree do nó A?

[imagem: imagens/153880_1_1_0.jpg]

- a) 2
- b) 4
- c) 3
- d) 1

**Resposta certa:** c) 3

**Explicação:** Na figura, o nó A está ligado a D, a B e a C, ou seja, 3 links. Em rede não direcionada o degree é só a contagem de links do nó, então o degree de A é 3. O C é uma folha pendurada em A, mas conta do mesmo jeito.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-10
Área 5 · Social Network Analysis I

Quantos nós possui a rede abaixo?

[imagem: imagens/153880_1_10_0.jpg]

- a) 5
- b) 4
- c) 6
- d) 7

**Resposta certa:** d) 7

**Explicação:** Contando as letras na figura, aparecem A, B, C, D, E, F e G, ou seja, 7 nós. Os links são 7: D-E, D-B, D-A, E-F, F-G, A-B e A-C. A pergunta é pelos nós, então são 7.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-2
Área 5 · Social Network Analysis I

Sobre a rede em questão, qual o Clustering Coefficient do nó B?

[imagem: imagens/153880_1_2_0.jpg]

- a) 0,14
- b) 0,45
- c) 0,33
- d) 0,25

**Resposta certa:** c) 0,33

**Explicação:** Os vizinhos de B são A, C e D. Entre eles só existe o link C-D, então há 1 ligação de 3 possíveis (3 x 2 / 2 = 3 pares). Clustering = 1/3 = 0,33.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-3
Área 5 · Social Network Analysis I

Sobre a rede em questão, qual é o degree ponderado do nó B?

[imagem: imagens/153880_1_3_0.jpg]

- a) 3
- b) 6
- c) 10
- d) 4

**Resposta certa:** c) 10

**Explicação:** O degree ponderado é a soma dos pesos dos links do nó. B se liga a A com peso 3, a C com peso 4 e a D com peso 3, então 3 + 4 + 3 = 10. O degree simples de B seria 3, que é a pegadinha da alternativa.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-4
Área 5 · Social Network Analysis I

Quantos nós possui a rede abaixo?

[imagem: imagens/153880_1_4_0.jpg]

- a) 5
- b) 7
- c) 6
- d) 4

**Resposta certa:** a) 5

**Explicação:** A figura mostra os nós A, B, C, D e E, ou seja, 5 vértices. Os links são 5: A-B, B-C, B-D, C-D e C-E. A pergunta é pelos nós, então a resposta é 5.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-5
Área 5 · Social Network Analysis I

Sobre a rede em questão, qual é o closeness do nó B?

[imagem: imagens/153880_1_5_0.jpg]

- a) 2,25
- b) 3
- c) 2
- d) 1,25

**Resposta certa:** d) 1,25

**Explicação:** Aqui o closeness é a distância média de B até os demais nós. B chega a A, C e D em 1 passo e a E em 2 passos (B-C-E). Soma = 1 + 1 + 1 + 2 = 5, dividido por 4 destinos dá 1,25.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-6
Área 5 · Social Network Analysis I

Considere os tópicos discutidos em aula e assinale a alternativa CORRETA sobre o conceito de comunidades em Social Network Analysis.

- a) As comunidades são subgrupos que necessariamente possuem conexões diretas com todos os outros subgrupos da rede.
- b) As comunidades são sempre formadas por nós que possuem exatamente o mesmo grau de conectividade.
- c) As comunidades são identificadas exclusivamente por meio da análise de centralidade de proximidade (closeness centrality).
- d) As comunidades são grupos de nós que estão mais fortemente ligados entre si do que com o resto da rede.

**Resposta certa:** d) As comunidades são grupos de nós que estão mais fortemente ligados entre si do que com o resto da rede.

**Explicação:** A resposta é que comunidades são grupos de nós mais fortemente ligados entre si do que com o resto da rede. A detecção de comunidades particiona a rede de modo que os links dentro do grupo sejam mais fortes que os links entre grupos. Não exige mesmo grau nem se limita ao closeness.

**Fonte:** Aula de Social Network Analysis, pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-7
Área 5 · Social Network Analysis I

Considere os conceitos discutidos em aula sobre Social Network Analysis e assinale a alternativa CORRETA sobre o degree ponderado:

- a) O degree ponderado é calculado apenas pela soma simples do número de conexões, ignorando completamente os pesos.
- b) O degree ponderado é uma generalização do degree que leva em conta o peso dos links, quando existente.
- c) O degree ponderado representa o número máximo de conexões possíveis que um nó pode ter em uma rede, considerando as limitações topológicas.
- d) O degree ponderado mede a distância média entre um nó e todos os outros nós da rede, ponderada pelos pesos das arestas.

**Resposta certa:** b) O degree ponderado é uma generalização do degree que leva em conta o peso dos links, quando existente.

**Explicação:** A resposta é que o degree ponderado generaliza o degree levando em conta o peso dos links, quando há pesos. Ignorar os pesos seria o degree simples, o máximo de conexões possíveis não é essa métrica e a distância média é o closeness.

**Fonte:** Aula de Social Network Analysis, pág. 26

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-8
Área 5 · Social Network Analysis I

Sobre a rede em questão, qual é o degree ponderado do nó A?

[imagem: imagens/153880_1_8_0.jpg]

- a) 10
- b) 2
- c) 3
- d) 5

**Resposta certa:** c) 3

**Explicação:** O nó A tem um único link, o que vai até B, com peso 3. O degree ponderado é a soma dos pesos, então é 3. Coincide com o degree simples só porque A tem um link, de peso 3.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 153880-1-9
Área 5 · Social Network Analysis I

Considere os conceitos discutidos em aula sobre Social Network Analysis e assinale a alternativa CORRETA sobre a métrica degree.

- a) É o número de vezes que determinado nó aparece no meio do caminho mais curto entre dois outros nós.
- b) Degree é a quantidade de links que um determinado nó possui (para uma rede undirected).
- c) É a média de passos que determinado nó dá para chegar me qualquer outro nó da Rede.
- d) É a densidade da rede do qual o determinado nó se conecta.

**Resposta certa:** b) Degree é a quantidade de links que um determinado nó possui (para uma rede undirected).

**Explicação:** A resposta é que o degree é a quantidade de links de um nó, em rede não direcionada. As outras alternativas descrevem outras métricas: o meio do caminho mais curto é a betweenness, a média de passos é o closeness e a densidade é uma estatística da rede inteira.

**Fonte:** Aula de Social Network Analysis, pág. 25

**Situação:** explicação conferida com o material das aulas

---

## Social Network Analysis II

### Questão 154253-1-1
Área 5 · Social Network Analysis II

Imaginando que cada “Id” da imagem abaixo seja um computador de uma rede interna de uma empresa, qual seria o computador que se fosse apagado impactaria fortemente na transmissão de arquivos?

[imagem: imagens/154253_1_1_0.jpg]

- a) J
- b) A
- c) H
- d) G

**Resposta certa:** c) H

**Explicação:** Na tabela do Gephi, o H tem o maior Betweenness Centrality, 14,0, contra 8,333 de C e F, 8,0 de I e 3,667 de D. Betweenness mede por quantos caminhos mais curtos o nó passa, então tirar o H é o que mais atrapalha a transmissão de arquivos. O grau dele é só 3, o que mostra que o que pesa aqui é a posição de ponte e não o número de conexões.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-10
Área 5 · Social Network Analysis II

Considere os conceitos discutidos em aula sobre as comunidades no contexto de Social Network Analysis e assinale a alternativa CORRETA:

- a) Uma comunidade é formada por indivíduos que se conectam intensamente entre si, mas que podem se conectar entre comunidades.
- b) Uma comunidade se forma por entidades parecidas entre si.
- c) Uma entidade que pertence a uma comunidade não pode se conectar com indivíduos de outras comunidades.
- d) Uma comunidade não se conecta com outra comunidade pois são indivíduos muito diferentes entre si.

**Resposta certa:** a) Uma comunidade é formada por indivíduos que se conectam intensamente entre si, mas que podem se conectar entre comunidades.

**Explicação:** A resposta é a que diz que a comunidade é formada por indivíduos muito conectados entre si, mas que podem se ligar a outras comunidades. Na definição de aula, os links dentro da comunidade são mais fortes que os links entre comunidades, e não inexistentes. Por isso é errado dizer que não há conexão entre elas.

**Fonte:** Aula de Social Network Analysis II (detecção de comunidades), pág. 18

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-2
Área 5 · Social Network Analysis II

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre a métrica de densidade do grafo:

- a) A densidade do grafo é uma medida da rede.
- b) É a soma dos menores caminhos dividido pela quantidade de menores caminho.
- c) Consiste no número de nós do grafo.
- d) A densidade do grafo é uma medida do nó.

**Resposta certa:** a) A densidade do grafo é uma medida da rede.

**Explicação:** A resposta é que a densidade é uma medida da rede, e não de um nó. Ela é o número de links dividido pelo total de links possíveis no grafo completo, então descreve o quanto a rede inteira está conectada. A alternativa da soma dos menores caminhos descreve o comprimento médio do caminho, outra métrica.

**Fonte:** Aula de Social Network Analysis (métricas da rede), pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-3
Área 5 · Social Network Analysis II

Considere as métricas da rede discutidas em aula e assinale a alternativa CORRETA sobre a excentricidade:

- a) Consiste na distância do nó em questão até o nó mais distante dele na rede (dentre os menores caminhos, o maior).
- b) Indica o número de vezes que um nó aparece no caminho mais curto entre outros pares de nós.
- c) Representa a soma das distâncias do nó em questão para todos os outros nós da rede.
- d) Corresponde ao número total de conexões diretas que um nó possui na rede.

**Resposta certa:** a) Consiste na distância do nó em questão até o nó mais distante dele na rede (dentre os menores caminhos, o maior).

**Explicação:** A resposta é a distância do nó até o nó mais distante dele, tomando o maior entre os menores caminhos. Essa é a definição de excentricidade, e dela saem o raio (menor excentricidade) e o diâmetro (maior). O número de conexões diretas é o grau, e as vezes em que o nó aparece nos caminhos mais curtos é a intermediação.

**Fonte:** Aula de Social Network Analysis (métricas da rede), pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-4
Área 5 · Social Network Analysis II

Imaginando que cada “Id” da imagem abaixo seja um computador de uma rede interna de uma empresa, qual seria o computador que se fosse apagado não impactaria em nada na rede?

[imagem: imagens/154253_1_4_0.jpg]

- a) F
- b) A
- c) C
- d) H

**Resposta certa:** b) A

**Explicação:** Na tabela, o A tem betweenness 0,0 e clustering coefficient 1,0: seus 3 vizinhos já são ligados entre si, então ele não é ponte de nenhum caminho mais curto. Tirar o A não muda a rota de ninguém. Das opções, F (8,333), C (8,333) e H (14,0) têm betweenness alta e a remoção deles pesaria bem mais.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-5
Área 5 · Social Network Analysis II

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre a Modularidade no contexto das comunidades em Social Network Analysis.

- a) Modularidade é o número máximo de comunidades que podem ser identificadas em uma rede utilizando algoritmos de detecção automática.
- b) Modularidade é a fração entre os links que estão dentro da comunidade menos a fração esperada se os links fossem distribuídos aleatoriamente (se a comunidade fosse criada aleatoriamente).
- c) Modularidade indica o grau de sobreposição entre as comunidades, medindo quantos nós pertencem a múltiplas comunidades simultaneamente.
- d) Modularidade representa a densidade média de conexões entre diferentes comunidades da rede.

**Resposta certa:** b) Modularidade é a fração entre os links que estão dentro da comunidade menos a fração esperada se os links fossem distribuídos aleatoriamente (se a comunidade fosse criada aleatoriamente).

**Explicação:** A resposta é a que define modularidade como a fração de links dentro da comunidade menos a fração esperada se os links fossem distribuídos ao acaso. Ela mede a qualidade da divisão em comunidades e é a métrica mais usada para detectá-las. Não conta comunidades nem mede sobreposição.

**Fonte:** Aula de Social Network Analysis II (detecção de comunidades), pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-6
Área 5 · Social Network Analysis II

A métrica Closeness pode ser impactada pelo peso?

- a) Sim, pois por mais que um nó de uma comunidade não se comunica com entidades de outra comunidade este valor pode ser diferente ao calcular dessa forma.
- b) Sim, em uma rede com pesos pode-se calcular a quantidade de links levando em consideração os pesos, ou não. Mas uma vez que leve em consideração, o número de links levará em conta o peso desse link.
- c) Não, pois um nó de uma comunidade não se comunica com entidades de outra comunidade.
- d) Sim, em uma rede com pesos pode-se calcular a média de passos que um indivíduo dá para chegar em qualquer outro na rede levando em consideração os pesos, ou não. Sendo assim, uma vez que leve em consideração, os menores caminhos serão sempre os caminhos de menores pesos.

**Resposta certa:** d) Sim, em uma rede com pesos pode-se calcular a média de passos que um indivíduo dá para chegar em qualquer outro na rede levando em consideração os pesos, ou não. Sendo assim, uma vez que leve em consideração, os menores caminhos serão sempre os caminhos de menores pesos.

**Explicação:** A resposta é que sim: o closeness usa a distância média até os demais nós, calculada pelos menores caminhos. Numa rede com pesos, dá para considerar o peso ou ignorá-lo, e quando se considera, o menor caminho passa a ser o de menor peso total. Isso muda o valor, o que derruba a alternativa do não.

**Fonte:** Aula de Social Network Analysis (centralidade closeness), pág. 37

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 154253-1-7
Área 5 · Social Network Analysis II

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre o software Gephi:

- a) É uma plataforma interativa de visualização e exploração de redes e sistemas complexos, incluindo grafos dinâmicos e hierárquicos.
- b) É um software proprietário desenvolvido pela IBM para análise estatística de redes sociais corporativas.
- c) É uma linguagem de programação especializada em processamento de grandes volumes de dados de redes sociais.
- d) É uma extensão do Microsoft Excel voltada para criação de matrizes de adjacência e cálculo de métricas básicas de rede.

**Resposta certa:** a) É uma plataforma interativa de visualização e exploração de redes e sistemas complexos, incluindo grafos dinâmicos e hierárquicos.

**Explicação:** A resposta é que o Gephi é uma plataforma interativa de visualização e exploração de redes e sistemas complexos, inclusive grafos dinâmicos e hierárquicos. É software livre, escrito em Java e roda em Windows, Linux e Mac. Não é produto da IBM, nem linguagem de programação, nem extensão do Excel.

**Fonte:** Aula de Social Network Analysis (Gephi), pág. 40

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-8
Área 5 · Social Network Analysis II

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA.

- a) Closeness é o número de conexões que determinado ponto possui.
- b) Diâmetro da rede é o nó que faz ponte entre dois mundos. Ou seja, se ele some, dois universos deixam de se conectar.
- c) Raio é o mínimo de passos que se daria, na rede em questão, para sair de um ponto e chegar em qualquer outro ponto na rede.
- d) Clustering coeficiente é o mínimo de passos que se daria, na rede em questão, para sair de um ponto e chegar em qualquer outro ponto na rede.

**Resposta certa:** c) Raio é o mínimo de passos que se daria, na rede em questão, para sair de um ponto e chegar em qualquer outro ponto na rede.

**Explicação:** A resposta é a do raio, que é a menor excentricidade da rede, ou seja, o menor alcance máximo que algum nó precisa percorrer para chegar a todos os outros. Closeness não é contagem de conexões (isso é grau), e o nó que faz ponte entre dois mundos não é o diâmetro. O clustering é outra coisa.

**Fonte:** Aula de Social Network Analysis (métricas da rede), pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 154253-1-9
Área 5 · Social Network Analysis II

Considere os conceitos discutidos em aula e assinale a alternativa INCORRETA.

- a) Excentricidade é a maior quantidade de passos que um determinado individuo dá para chegar em qualquer outro, a partir dos menores caminhos.
- b) Degree Ponderado é o número de conexões que determinado ponto possui, levando em conta o peso do relacionamento.
- c) Betweenness é o número de vezes que determinado nó aparece no meio do caminho mais curto entre dois outros nós.
- d) Degree in é o número de conexões que determinado nó faz (sai de um nó específico e chega em algum outro nó).

**Resposta certa:** d) Degree in é o número de conexões que determinado nó faz (sai de um nó específico e chega em algum outro nó).

**Explicação:** A alternativa incorreta é a do degree in. Ele conta os links que chegam ao nó, e não os que saem dele. Quem conta os links que saem é o out-degree, e o degree total é a soma dos dois. As demais definições (excentricidade, degree ponderado e betweenness) estão certas.

**Fonte:** Aula de Social Network Analysis (centralidade de grau), pág. 25

**Situação:** explicação conferida com o material das aulas

---

## Séries Temporais I

### Questão 181673-1-1
Área 5 · Séries Temporais I

As séries temporais podem ser classificadas em discretas e contínuas. Qual a diferença central entre elas?

- a) As séries discretas são aquelas em que as observações ocorrem em instantes específicos e separados no tempo, enquanto as séries contínuas são aquelas em que as observações são registradas de forma ininterrupta ao longo de um intervalo de tempo.
- b) As séries discretas são aquelas coletadas em períodos curtos de tempo, como dias ou semanas, enquanto as séries contínuas são aquelas coletadas em períodos longos de tempo, como meses ou anos.
- c) As séries discretas são aquelas que não apresentam tendência nem sazonalidade, enquanto as séries contínuas são aquelas que possuem pelo menos um desses componentes identificável ao longo do tempo.
- d) As séries discretas são aquelas cujos valores observados são necessariamente números inteiros, enquanto as séries contínuas são aquelas cujos valores observados podem assumir qualquer número real dentro de um intervalo.

**Resposta certa:** a) As séries discretas são aquelas em que as observações ocorrem em instantes específicos e separados no tempo, enquanto as séries contínuas são aquelas em que as observações são registradas de forma ininterrupta ao longo de um intervalo de tempo.

**Explicação:** A resposta é que a série discreta tem observações em instantes fixos e separados, e a contínua é registrada de forma ininterrupta num intervalo. A diferença está na forma de coleta, e não no tamanho do período, na presença de sazonalidade ou em valores inteiros ou reais.

**Fonte:** Aula de Séries Temporais (classificação das séries), pág. 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-10
Área 5 · Séries Temporais I

O mercado de trabalho de uma cidade turística litorânea registra, todo ano no verão, um aumento expressivo na oferta de empregos no setor de hotelaria e comércio. Essa variação é classificada como:

- a) Uma variação sazonal, pois o verão é uma estação que se repete anualmente e, com ela, tipicamente ocorre um acréscimo na oferta de empregos.
- b) Uma variação irregular, pois se trata de um evento imprevisível e não recorrente, causado por fatores aleatórios que afetam o mercado de trabalho pontualmente.
- c) Uma variação cíclica, pois está associada a flutuações irregulares da economia, como expansões e recessões, que não seguem um padrão fixo de periodicidade.
- d) Uma variação de tendência, pois reflete um crescimento contínuo e persistente na oferta de empregos ao longo de vários anos.

**Resposta certa:** a) Uma variação sazonal, pois o verão é uma estação que se repete anualmente e, com ela, tipicamente ocorre um acréscimo na oferta de empregos.

**Explicação:** A resposta é variação sazonal. O aumento de vagas acontece todo verão, num padrão que se repete dentro do ano. Ciclo seria uma oscilação econômica sem periodicidade fixa, tendência seria um crescimento persistente por vários anos e irregular seria um evento pontual.

**Fonte:** Aula de Séries Temporais (componentes da série), pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-2
Área 5 · Séries Temporais I

Na modelagem de séries temporais, a sigla ETS representa, nessa ordem, os componentes:

- a) Sazonal, Erro, Tendência
- b) Tendência, Sazonal, Erro
- c) Erro, Sazonal, Tendência
- d) Erro, Tendência, Sazonal

**Resposta certa:** d) Erro, Tendência, Sazonal

**Explicação:** A resposta é Erro, Tendência, Sazonal, nessa ordem, que é a leitura de ETS (Error, Trend, Seasonal). No pacote, cada letra recebe um código: A aditivo, M multiplicativo, N nenhum e Z automático. Por isso um modelo como AAA tem erro, tendência e sazonalidade aditivos.

**Fonte:** Aula de Séries Temporais (modelo ETS), pág. 51

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-3
Área 5 · Séries Temporais I

Os valores a seguir representam as cotações da saca de 60 kg de café. O valor da média móvel de 3 períodos, estimada com base nos três dias mais recentes, para o próximo período é:

[imagem: imagens/181673_1_3_0.jpg]

- a) 1.117,61
- b) 1.100,01
- c) 1.093,67
- d) 1.123,95

**Resposta certa:** c) 1.093,67

**Explicação:** A média móvel de 3 períodos usa as três cotações mais recentes da tabela: 1.111,82 (24/04), 1.076,43 (25/04) e 1.092,76 (26/04). A soma é 3.281,01, e dividindo por 3 dá 1.093,67, que é a previsão do próximo período.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-4
Área 5 · Séries Temporais I

A técnica de decomposição de uma série temporal é fundamental para identificar padrões subjacentes aos dados. Ao isolar o componente de sazonalidade, o analista está buscando identificar:

- a) Mudanças bruscas causadas por eventos atípicos e inesperados (outliers).
- b) A direção de longo prazo, indicando se os dados crescem ou decrescem ao longo dos anos.
- c) Flutuações periódicas que se repetem em intervalos regulares, como meses ou trimestres.
- d) O componente aleatório ou "ruído", que não pode ser explicado por modelos matemáticos.

**Resposta certa:** c) Flutuações periódicas que se repetem em intervalos regulares, como meses ou trimestres.

**Explicação:** A resposta é flutuações periódicas que se repetem em intervalos regulares, como meses ou trimestres. É isso que a sazonalidade representa na decomposição. A direção de longo prazo é a tendência, os picos atípicos são outliers e o ruído é o componente aleatório.

**Fonte:** Aula de Séries Temporais (componentes da série), pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-5
Área 5 · Séries Temporais I

Muitas séries temporais apresentam, junto a uma tendência, variações cíclicas e sazonais. Por quais razões essas variações podem aparecer em séries temporais?

- a) Essas variações surgem somente quando a série temporal possui distribuição normal, refletindo a simetria natural dos dados em torno da média.
- b) Essas variações ocorrem exclusivamente devido a erros de medição e ruídos aleatórios introduzidos durante a coleta dos dados.
- c) Essas variações são causadas apenas pela tendência de longo prazo da série, que se desdobra em componentes de curto prazo ao longo do tempo.
- d) Essas variações podem ocorrer devido a fatores como clima, ciclos econômicos, hora do dia, entre outros.

**Resposta certa:** d) Essas variações podem ocorrer devido a fatores como clima, ciclos econômicos, hora do dia, entre outros.

**Explicação:** A resposta é que essas variações surgem por fatores como clima, ciclos econômicos e hora do dia. Não dependem de a série ser normal, nem são só erro de medição, nem decorrem apenas da tendência. Se elas podem ser observadas, levá-las em conta melhora a previsão, e daí vêm os métodos de decomposição.

**Fonte:** Aula de Séries Temporais (tendência, ciclos e sazonalidade), pág. 26

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-6
Área 5 · Séries Temporais I

O MAPE (Erro Absoluto Percentual Médio) é uma das métricas mais utilizadas para avaliar a performance de modelos de previsão. Sua principal vantagem em relação ao RMSE (Raiz do Erro Quadrático Médio) é:

- a) A capacidade de penalizar erros grandes de forma quadrática.
- b) A facilidade de interpretação, pois expressa o erro em termos percentuais, permitindo comparar a precisão entre diferentes séries.
- c) Garantir que o modelo não apresente viés (bias) de superestimação.
- d) O fato de ser uma medida absoluta expressa na mesma unidade dos dados originais.

**Resposta certa:** b) A facilidade de interpretação, pois expressa o erro em termos percentuais, permitindo comparar a precisão entre diferentes séries.

**Explicação:** A resposta é a facilidade de interpretação. O MAPE expressa o erro como porcentagem do valor real, então permite comparar a precisão entre séries de escalas diferentes. O RMSE fica na unidade dos dados e penaliza mais os erros grandes, e nenhum dos dois garante ausência de viés.

**Fonte:** Aula de Séries Temporais (estatísticas de erro), pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-7
Área 5 · Séries Temporais I

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre sazonalidade em séries temporais:

- a) Sazonalidade corresponde ao movimento de longo prazo de uma série temporal, refletindo o crescimento ou declínio persistente de uma variável ao longo de vários anos, independentemente de variações de curto prazo.
- b) Sazonalidade corresponde a flutuações irregulares e imprevisíveis que ocorrem em intervalos variáveis de tempo, sem periodicidade definida, geralmente associadas a choques externos como crises econômicas ou eventos climáticos extremos.
- c) Sazonalidade corresponde a flutuações regulares que ocorrem dentro de um período fixo de tempo (um dia, uma semana, um mês, etc.), formando um padrão que se repete ao longo do tempo.
- d) Sazonalidade corresponde a oscilações de média duração, geralmente entre dois e dez anos, associadas a ciclos econômicos de expansão e recessão, que não necessariamente se repetem em intervalos regulares de tempo.

**Resposta certa:** c) Sazonalidade corresponde a flutuações regulares que ocorrem dentro de um período fixo de tempo (um dia, uma semana, um mês, etc.), formando um padrão que se repete ao longo do tempo.

**Explicação:** A resposta é a que descreve sazonalidade como flutuações regulares dentro de um período fixo (dia, semana, mês), formando um padrão que se repete. Movimento de longo prazo é tendência, e oscilações de média duração sem período fixo são os ciclos. Variações irregulares são o componente aleatório.

**Fonte:** Aula de Séries Temporais (sazonalidade), pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-8
Área 5 · Séries Temporais I

Considerando a série temporal de vendas mensais de um determinado produto, apresentada na tabela abaixo, qual é a previsão para maio do Ano 2 pelo método da média móvel de 3 períodos?

[imagem: imagens/181673_1_8_0.jpg]

- a) 29
- b) 32
- c) 24
- d) 19

**Resposta certa:** c) 24

**Explicação:** Para maio do Ano 2, a média móvel de 3 períodos usa os três meses anteriores do Ano 2: fevereiro 17, março 26 e abril 29. A soma é 72, e 72 dividido por 3 dá 24.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 181673-1-9
Área 5 · Séries Temporais I

Sobre os modelos de previsão de séries temporais, analise as afirmativas a seguir e as classifique em verdadeiras (V) ou falsas (F).

I – O nome média móvel é utilizado porque, a cada período, a observação mais antiga é substituída pela mais recente, calculando-se uma média nova;

II – O método de Suavização Exponencial Simples se aplicado a uma série que apresenta tendência linear positiva (ou negativa), fornece previsões que subestimam (ou superestimam) continuamente os valores reais. Para evitar esse erro sistemático, um dos métodos aplicáveis é a Suavização Exponencial de Holt;

III – Os métodos de Suavização Exponencial Sazonal de Holt Winterss (HW) são mais adequados à análise de séries temporais com padrão de comportamento mais geral.

Assim, a classificação CORRETA fica:

- a) V – F – F
- b) V – V – F
- c) V – V – V
- d) F – F – F

**Resposta certa:** c) V – V – V

**Explicação:** As três afirmativas são verdadeiras. A média móvel é assim chamada porque a observação mais antiga sai e a mais recente entra a cada período. A suavização simples erra de forma sistemática diante de tendência linear, e o método de Holt corrige isso. Holt-Winters acrescenta a sazonalidade, servindo a séries com comportamento mais geral.

**Fonte:** Aula de Séries Temporais (Holt e Holt-Winters), pág. 45

**Situação:** explicação conferida com o material das aulas

---

## Séries Temporais II

### Questão 182475-1-1
Área 5 · Séries Temporais II

Qual o significado dos parâmetros p, d e q respectivamente nos Modelos ARIMA?

- a) Ordem da parte autorregressiva, grau de diferenciação e ordem da média móvel.
- b) Grau de diferenciação, ordem da média móvel e ordem da parte autorregressiva.
- c) Ordem da média móvel, ordem da parte autorregressiva e grau de diferenciação.
- d) Constante de suavização, número de períodos sazonais e tamanho da janela de previsão.

**Resposta certa:** a) Ordem da parte autorregressiva, grau de diferenciação e ordem da média móvel.

**Explicação:** A resposta é ordem da parte autorregressiva, grau de diferenciação e ordem da média móvel, nessa ordem. No ARIMA(p,d,q), p vem da PACF, d vem do teste de estacionariedade (quantas diferenciações) e q vem da ACF.

**Fonte:** Aula de Séries Temporais (modelos ARIMA), pág. 56

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-10
Área 5 · Séries Temporais II

Considere os conceitos relacionados à séries temporais discutidos em aula e assinale a alternativa CORRETA:

- a) As variações sazonais correspondem a um certo grau de regularidade a longo prazo no comportamento das séries temporais.
- b) A tendência descreve um movimento de longo prazo dos dados, podendo indicar uma direção crescente ou decrescente ao longo do tempo.
- c) As variações cíclicas representam regularidades de variações na série em períodos curtos de tempo, geralmente dentro de um ano.
- d) As variações irregulares ou aleatórias correspondem a movimentos ascendentes e decrescentes revelando a direção da série.

**Resposta certa:** b) A tendência descreve um movimento de longo prazo dos dados, podendo indicar uma direção crescente ou decrescente ao longo do tempo.

**Explicação:** A resposta é que a tendência é o movimento de longo prazo, com direção crescente ou decrescente. Sazonalidade é padrão regular dentro do ano e ciclo é flutuação de longo prazo sem período fixo, então as outras alternativas trocam os conceitos. Variações aleatórias não revelam direção.

**Fonte:** Aula de Séries Temporais (componentes da série), pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-2
Área 5 · Séries Temporais II

O que define o modelo de previsão NAIVE?

- a) A exclusão total dos componentes de erro para focar apenas na tendência.
- b) O cálculo da média ponderada de todos os dados históricos desde o início da série.
- c) A utilização de algoritmos de aprendizado profundo para identificar padrões ocultos.
- d) A premissa de que o valor do próximo período será exatamente igual ao último valor observado.

**Resposta certa:** d) A premissa de que o valor do próximo período será exatamente igual ao último valor observado.

**Explicação:** A resposta é a premissa de que o próximo valor será igual ao último observado. O NAIVE simplesmente projeta o último valor para o futuro. Não usa média ponderada de todo o histórico nem aprendizado profundo.

**Fonte:** Aula de Séries Temporais (métodos simples), pág. 37

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-3
Área 5 · Séries Temporais II

Um modelo de previsão da forma
, tendo apenas um parâmetro a ser estimado, alfa, se refere a um modelo:

[imagem: imagens/182475_1_3_0.png]

- a) De Suavização Exponencial Simples
- b) De Suavização Exponencial de Holt
- c) Auto Regressivo Integrado de Médias Móveis
- d) De Suavização Exponencial de Holt-Winters

**Resposta certa:** a) De Suavização Exponencial Simples

**Explicação:** Um modelo com só um parâmetro a estimar, o alfa, é a suavização exponencial simples. Holt acrescenta o parâmetro beta da tendência e Holt-Winters acrescenta o gama da sazonalidade, e o ARIMA usa p, d e q. A equação aparece na figura, mas a escolha segue da contagem de parâmetros.

**Fonte:** Aula de Séries Temporais (suavização exponencial simples), pág. 43

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 182475-1-4
Área 5 · Séries Temporais II

Qual é a característica central de séries temporais estacionárias?

- a) Possuem sazonalidade bem definida, com picos e vales que se repetem em intervalos fixos ao longo do ano.
- b) Apresentam uma tendência claramente crescente ou decrescente ao longo do tempo, com variância estável entre os períodos.
- c) Sua média e variância permanecem constantes ao longo do tempo.
- d) Seus valores futuros podem ser previstos com exatidão, pois o padrão da série se repete de forma regular a cada período.

**Resposta certa:** c) Sua média e variância permanecem constantes ao longo do tempo.

**Explicação:** A resposta é que a média e a variância ficam constantes ao longo do tempo. Esse é o critério de estacionariedade, e a covariância entre dois períodos depende só da defasagem entre eles. Tendência e sazonalidade, por mudarem a média, tiram a série dessa condição.

**Fonte:** Aula de Séries Temporais (teste de estacionariedade), pág. 67

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-5
Área 5 · Séries Temporais II

Na decomposição clássica de uma série temporal, a Sazonalidade representa:

- a) O componente puramente aleatório, errático e imprevisível da série.
- b) A média ponderada de todos os erros quadráticos acumulados no modelo.
- c) Uma variação de longo prazo que indica a direção estrutural dos dados.
- d) Flutuações regulares dentro de um período fixo de tempo, representando um padrão que se repete (picos e vales) geralmente com ciclo inferior a um ano.

**Resposta certa:** d) Flutuações regulares dentro de um período fixo de tempo, representando um padrão que se repete (picos e vales) geralmente com ciclo inferior a um ano.

**Explicação:** A resposta é a que descreve sazonalidade como flutuações regulares num período fixo, um padrão de picos e vales que se repete, em geral dentro de um ano. O componente aleatório é o erro, e a variação de longo prazo que dá a direção dos dados é a tendência.

**Fonte:** Aula de Séries Temporais (componentes da série), pág. 23

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-6
Área 5 · Séries Temporais II

Uma transportadora apresentou as quantidades de cargas transportadas em cada um dos últimos três meses que foram, respectivamente igual a 110, 126 e 124 toneladas. Utilizando o método de média móvel de três meses, calcule a previsão para o quarto mês:

- a) 130
- b) 120
- c) 127
- d) 116

**Resposta certa:** b) 120

**Explicação:** A média móvel de três meses é a média dos três últimos valores. Conta: (110 + 126 + 124) / 3 = 360 / 3 = 120 toneladas. Usar só o último mês (124) seria o NAIVE, que ignora os outros dois.

**Fonte:** Aula de Séries Temporais (média móvel), pág. 52

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 182475-1-7
Área 5 · Séries Temporais II

Qual das alternativas abaixo apresenta uma estatística utilizada para medir o erro de previsão em séries temporais?

- a) MAPE
- b) SARIMA
- c) AIC
- d) BIC

**Resposta certa:** a) MAPE

**Explicação:** A resposta é o MAPE, o erro percentual absoluto médio, que compara previsto e realizado. SARIMA é um modelo, enquanto AIC e BIC são critérios de seleção de modelos, e não medem o erro da previsão.

**Fonte:** Aula de Séries Temporais (estatísticas de erro), pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-8
Área 5 · Séries Temporais II

Assinale a alternativa CORRETA sobre os modelos ARIMA (Box-Jenkins)?

- a) Os parâmetros p, d e q representam, respectivamente, o número de períodos sazonais, a constante de suavização e o tamanho da janela de média móvel.
- b) Requer que a série seja estacionária, sendo a diferenciação o recurso utilizado pelo modelo para lidar com séries que não apresentam essa propriedade.
- c) É indicado exclusivamente para séries com sazonalidade pronunciada, não sendo aplicável a séries sem padrão sazonal.
- d) É um modelo estritamente determinístico, ou seja, dado o histórico da série, a previsão futura é calculada sem qualquer componente aleatório.

**Resposta certa:** b) Requer que a série seja estacionária, sendo a diferenciação o recurso utilizado pelo modelo para lidar com séries que não apresentam essa propriedade.

**Explicação:** A resposta é a que diz que o ARIMA exige série estacionária e usa a diferenciação para tratar as que não são. A diferenciação subtrai a observação anterior da atual e remove tendências. O modelo não é exclusivo de séries sazonais e tem componente aleatório.

**Fonte:** Aula de Séries Temporais (ARIMA Box-Jenkins), pág. 54

**Situação:** explicação conferida com o material das aulas

---

### Questão 182475-1-9
Área 5 · Séries Temporais II

Uma empresa precisa realizar a previsão de vendas para o próximo mês de seu produto mais conhecido. Os valores dos últimos dez meses estão na tabela abaixo.

Se a empresa pretende realizar uma previsão pelo NAIVE, o valor previsto para o próximo mês será de:
Uma empresa precisa realizar a previsão de vendas para o próximo mês de seu produto mais conhecido. Os valores dos últimos dez meses estão na tabela abaixo.
Se a empresa pretende realizar uma previsão pelo NAIVE, o valor previsto para o próximo mês será de:

[imagem: imagens/182475_1_9_0.jpg]

- a) 36
- b) 30
- c) 28
- d) 40

**Resposta certa:** d) 40

**Explicação:** No NAIVE a previsão é o último valor observado. Na tabela, o Mês 10 tem vendas de 40 (os valores vão 30, 35, 27, 42, 34, 36, 56, 33, 28 e 40), então a previsão para o próximo mês é 40.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

## Séries Temporais III

### Questão 183434-1-1
Área 5 · Séries Temporais III

A série temporal da imagem abaixo corresponde ao Consumo de Energia (GWh) de uma determinada cidade nos últimos 24 meses. Pergunta-se: Qual é o valor da previsão da série temporal pelo modelo NAIVE para o 25º mês?

[imagem: imagens/183434_1_1_0.jpg]

- a) 175,2
- b) 173,7
- c) 174,1
- d) 174,5

**Resposta certa:** b) 173,7

**Explicação:** O NAIVE repete o último valor observado. Na tabela, o 24º mês (t = 24) tem consumo de 173,7 GWh, então a previsão para o 25º mês é 173,7.

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-10
Área 5 · Séries Temporais III

Um modelo na forma
 é um modelo:

[imagem: imagens/183434_1_10_0.png]

- a) ARIMA (1,1,1)
- b) ARIMA (1,0,1)
- c) ARIMA (0,1,1)
- d) ARIMA (1,0,0)

**Resposta certa:** b) ARIMA (1,0,1)

**Explicação:** A equação da figura é yt = 0,5·yt-1 - 0,2·εt-1 + εt, com uma defasagem da série (p = 1), uma defasagem do erro (q = 1) e nenhuma diferenciação (d = 0). Esse é o ARMA(1,1), ou seja, ARIMA(1,0,1).

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-2
Área 5 · Séries Temporais III

Qual dos conjuntos de critérios abaixo é utilizado para a escolha de modelos em séries temporais?

- a) Teste de Ljung-Box e Teste de Dickey-Fuller Aumentado (ADF).
- b) Média e Desvio Padrão da série.
- c) AIC (Critério de Informação de Akaike) e BIC (Critério de Informação Bayesiano).
- d) FAC (Função de Autocorrelação) e FACP (Função de Autocorrelação Parcial).

**Resposta certa:** c) AIC (Critério de Informação de Akaike) e BIC (Critério de Informação Bayesiano).

**Explicação:** A resposta é AIC e BIC. Os dois são critérios de informação usados para comparar modelos: quanto menor o valor, melhor o equilíbrio entre ajuste e complexidade. FAC e FACP servem para identificar p e q, e Ljung-Box e ADF testam resíduos e estacionariedade.

**Fonte:** Aula de Séries Temporais (escolha dos modelos), pág. 60

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-3
Área 5 · Séries Temporais III

Qual dos testes abaixo corresponde a um Teste de Normalidade dos Resíduos?

- a) Critério de Informação de Akaike (AIC).
- b) Teste de Dickey-Fuller Aumentado (ADF).
- c) Teste de Ljung-Box.
- d) Teste de Kolmogorov-Smirnov.

**Resposta certa:** d) Teste de Kolmogorov-Smirnov.

**Explicação:** A resposta é Kolmogorov-Smirnov, um teste de aderência à distribuição normal. AIC é critério de seleção, ADF testa raiz unitária e Ljung-Box testa autocorrelação dos resíduos. Nas aulas aparece também o Jarque-Bera como teste de normalidade.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 234

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-4
Área 5 · Séries Temporais III

Assinale a alternativa CORRETA sobre um Modelo Autorregressivo AR(1):

- a) Possui apenas uma única defasagem.
- b) Possui zero defasagens.
- c) Possui duas defasagens autorregressivas.
- d) Possui três ou mais defasagens.

**Resposta certa:** a) Possui apenas uma única defasagem.

**Explicação:** A resposta é que o AR(1) tem apenas uma defasagem. O p do modelo é a defasagem máxima de Y presente na equação, então no AR(1) só Y de t-1 explica Y de t. Com duas defasagens seria AR(2).

**Fonte:** Aula de Séries Temporais (modelos ARIMA), pág. 76

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-5
Área 5 · Séries Temporais III

Um modelo na forma
 é um modelo:

[imagem: imagens/183434_1_5_0.png]

- a) AR (2)
- b) MA (2)
- c) ARMA (2,2)
- d) AR (1)

**Resposta certa:** a) AR (2)

**Explicação:** A equação da figura é yt = 0,5·yt-1 - 0,3·yt-2 + εt. A variável depende de dois valores passados dela própria e só do erro corrente, sem erros defasados. Isso caracteriza um AR(2).

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-6
Área 5 · Séries Temporais III

Assinale a alternativa que apresenta o padrão típico da Função de Autocorrelação (FAC) de um processo MA (q):

- a) Cresce progressivamente à medida que o número de defasagens aumenta.
- b) Decai exponencialmente com padrão de onda senoidal amortecida.
- c) Cresce progressivamente para 1.
- d) Apresenta valores significativos até a defasagem q.

**Resposta certa:** d) Apresenta valores significativos até a defasagem q.

**Explicação:** A resposta é que a FAC de um MA(q) tem valores significativos até a defasagem q e depois corta. O AR(p) é o que decai exponencialmente, com padrão de onda senoidal amortecida. É a FACP que corta no AR.

**Fonte:** Aula de Séries Temporais (características da FAC), pág. 74

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-7
Área 5 · Séries Temporais III

Qual dos testes abaixo é utilizado para verificar se uma série temporal possui raiz unitária?

- a) Teste de Dickey-Fuller aumentado (ADF).
- b) Teste Qui-Quadrado.
- c) Teste de Ljung-Box.
- d) Kolmogorov-Smirnov.

**Resposta certa:** a) Teste de Dickey-Fuller aumentado (ADF).

**Explicação:** A resposta é o teste de Dickey-Fuller aumentado (ADF). A hipótese nula é que a série tem raiz unitária, ou seja, não é estacionária. Ljung-Box avalia autocorrelação, e Kolmogorov-Smirnov e qui-quadrado não servem para esse fim.

**Fonte:** Aula de Séries Temporais (teste de estacionariedade), pág. 68

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-8
Área 5 · Séries Temporais III

Assinale a alternativa que melhor descreve a Função de Autocorrelação (FAC):

- a) A FAC elimina automaticamente todos os outliers que prejudicam a visualização do gráfico.
- b) A FAC transforma uma série de modelo multiplicativo em uma série de modelo aditivo.
- c) A FAC calcula a acurácia final do modelo após a realização de uma simulação de Monte Carlo.
- d) A FAC apresenta as autocorrelações de uma série temporal em diferentes defasagens, acompanhadas de um intervalo de confiança que indica sua significância estatística.

**Resposta certa:** d) A FAC apresenta as autocorrelações de uma série temporal em diferentes defasagens, acompanhadas de um intervalo de confiança que indica sua significância estatística.

**Explicação:** A resposta é que a FAC mostra as autocorrelações da série em várias defasagens, com um intervalo de confiança que indica a significância de cada uma. Ela não remove outliers, não converte modelo multiplicativo em aditivo e não calcula a acurácia do modelo.

**Fonte:** Aula de Séries Temporais (correlogramas), pág. 72

**Situação:** explicação conferida com o material das aulas

---

### Questão 183434-1-9
Área 5 · Séries Temporais III

Um modelo na forma
 é um modelo:

[imagem: imagens/183434_1_9_0.png]

- a) MA (2)
- b) AR (2)
- c) AR (1)
- d) MA (1)

**Resposta certa:** c) AR (1)

**Explicação:** A equação da figura é yt = 0,8·yt-1 + εt. Há apenas uma defasagem da própria série e o erro corrente, sem erros passados, então é um AR(1).

**Fonte:** Figura da questão

**Situação:** explicação conferida com o material das aulas

---

## Text Mining, Sentiment Analysis e NLP I

### Questão 192418-1-1
Área 5 · Text Mining, Sentiment Analysis e NLP I

Sobre a importância da linguística, podemos afirmar que:

- a) O estudo da linguística não influencia na compreensão de diferentes sociedades.
- b) A linguística estuda apenas a gramática de um idioma.
- c) A língua não interfere na identidade cultural de um grupo.
- d) A linguagem representa a cultura, as tradições e a união de um povo.

**Resposta certa:** d) A linguagem representa a cultura, as tradições e a união de um povo.

**Explicação:** A resposta é que a linguagem representa a cultura, as tradições e a união de um povo. A aula diz que uma língua não é só um conjunto de palavras. Por isso a alternativa que reduz a linguística à gramática, ou que nega o papel da língua na identidade cultural, está errada.

**Fonte:** Aula de Text Mining, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-10
Área 5 · Text Mining, Sentiment Analysis e NLP I

Por que a remoção de pontuação é importante no processo de pré-processamento de texto?

- a) Porque torna o texto mais fácil de ser lido por humanos.
- b) Porque melhora a fluidez do texto final.
- c) Porque aumenta a complexidade dos modelos de machine learning.
- d) Porque evita que caracteres especiais influenciem na análise de dados.

**Resposta certa:** d) Porque evita que caracteres especiais influenciem na análise de dados.

**Explicação:** A remoção de pontuação elimina sinais como "!" que viram tokens soltos e poluem a análise; sem eles, o modelo trabalha só com as palavras. O motivo é analítico, não deixar o texto mais legível para humanos.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 29

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-2
Área 5 · Text Mining, Sentiment Analysis e NLP I

Onde o Text Mining se destaca?

- a) Unicamente da tomada de decisão sobre valor moral ou ético.
- b) Na extração de informação de grandes volumes textuais, análise de sentimentos, classificação de texto, detecção de fraudes e spam.
- c) Apenas na organização de textos em bancos de dados.
- d) Exclusivamente na criação de textos completamente novos.

**Resposta certa:** b) Na extração de informação de grandes volumes textuais, análise de sentimentos, classificação de texto, detecção de fraudes e spam.

**Explicação:** O text mining se destaca em extração de informação, análise de sentimentos, classificação de textos, detecção de fraudes e spam, sumarização e modelagem de tópicos. Ele extrai padrões de grandes volumes de texto; não é só organização em banco de dados nem geração de texto novo.

**Fonte:** Aula de Text Mining, pág. 25

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-3
Área 5 · Text Mining, Sentiment Analysis e NLP I

Considere os conceitos discutidos em aula e responda: o que são stopwords?

- a) São palavras que não agregam muito significado ao conteúdo em análises textuais, como "de", "e", "o".
- b) São técnicas usadas para criar resumos automáticos.
- c) São palavras usadas para indicar sentimentos em um texto.
- d) São conjuntos de palavras que precisam ser enfatizadas na análise textual.

**Resposta certa:** a) São palavras que não agregam muito significado ao conteúdo em análises textuais, como "de", "e", "o".

**Explicação:** Stopwords são palavras muito comuns, como "a", "o", "e", "de", "que", "em", que pouco acrescentam ao conteúdo e costumam ser removidas no pré-processamento. Não têm relação com resumo automático nem com expressar sentimento.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-4
Área 5 · Text Mining, Sentiment Analysis e NLP I

Quando falamos em reduzir palavras à sua raiz, e em reduzir a palavra à sua forma canônica, estamos nos referindo, respectivamente, a quais técnicas de pré-processamento de texto?

- a) Lemmatization e Stemming.
- b) Stemming e Lemmatization.
- c) Tokenization e Lemmatization.
- d) Stemming e Tokenization.

**Resposta certa:** b) Stemming e Lemmatization.

**Explicação:** Stemming reduz a palavra à sua raiz ("amasse" vira "am"), enquanto a lematização leva à forma canônica do dicionário ("amar"). A ordem da pergunta é raiz primeiro e forma canônica depois, então é Stemming e Lemmatization. Tokenization apenas divide o texto em unidades.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-5
Área 5 · Text Mining, Sentiment Analysis e NLP I

Dado o seguinte texto: "Eu estou aprendendo processamento de linguagem natural!". Aplique o processo de lowercasing e assinale a alternativa que representa corretamente o resultado final.

- a) os algoritmos de machine learning sao incríveis
- b) [eu, estou, aprendendo, processamento, de, linguagem, natural]
- c) eu estou aprendendo processamento de linguagem natural!
- d) aprendendo processamento linguagem natural

**Resposta certa:** c) eu estou aprendendo processamento de linguagem natural!

**Explicação:** Lowercasing só converte tudo para minúsculas e mantém o resto, inclusive a pontuação: "eu estou aprendendo processamento de linguagem natural!". A lista de palavras é o resultado da tokenização, e a versão sem "de" já passou por remoção de stopwords.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 37

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-6
Área 5 · Text Mining, Sentiment Analysis e NLP I

O que é lowercasing no processamento de linguagem natural?

- a) Técnica para converter todas as letras de um texto para maiúsculas.
- b) Processo de remover palavras irrelevantes de um texto.
- c) É uma forma de classificar vídeos e textos automaticamente.
- d) Técnica comum de pré-processamento de texto usada para padronizar o texto e reduzir a complexidade do vocabulário.

**Resposta certa:** d) Técnica comum de pré-processamento de texto usada para padronizar o texto e reduzir a complexidade do vocabulário.

**Explicação:** Lowercasing é uma etapa de pré-processamento que padroniza o texto, passando tudo para minúsculas, de modo que "Eu" e "eu" virem a mesma palavra e o vocabulário fique menor. A alternativa de converter para maiúsculas descreve o contrário do que a técnica faz.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 28

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-7
Área 5 · Text Mining, Sentiment Analysis e NLP I

Considere os conceitos discutidos em aula e assinale a assertiva CORRETA sobre tokenização:

- a) Tokenização é uma técnica para criptografar textos.
- b) Tokenização é um método para transformar palavras em números.
- c) Tokenização é um processo de divisão de um texto em unidades menores, como palavras ou frases.
- d) Tokenização é uma estratégia para remover pontuação de um texto.

**Resposta certa:** c) Tokenização é um processo de divisão de um texto em unidades menores, como palavras ou frases.

**Explicação:** Tokenização é dividir o texto em unidades menores, os tokens, como palavras e sinais de pontuação: "Eu amo MBA!" vira ["Eu", "amo", "MBA", "!"]. Remover pontuação é outra etapa, e transformar palavras em números é vetorização.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-8
Área 5 · Text Mining, Sentiment Analysis e NLP I

Considere os conceitos discutidos em aula e responda: o que é o stemming?

- a) Técnica para remover palavras irrelevantes de um texto.
- b) Método de análise sintática de frases.
- c) Processo de encontrar o radical de uma palavra para reduzir sua variação morfológica.
- d) Estratégia para contar a frequência de palavras.

**Resposta certa:** c) Processo de encontrar o radical de uma palavra para reduzir sua variação morfológica.

**Explicação:** Stemming reduz a palavra ao seu radical, tirando a variação morfológica; no exemplo da aula, "amasse" vira "am". Remover palavras irrelevantes é a retirada de stopwords, e contar frequência é outra coisa.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 192418-1-9
Área 5 · Text Mining, Sentiment Analysis e NLP I

Qual alternativa melhor descreve o Text Mining?

- a) É um processo para criar automaticamente textos longos e complexos.
- b) É um método que extrai padrões, insights e informações úteis a partir de grandes quantidades de texto.
- c) Trata-se de estratégia para corrigir gramática e ortografia de textos.
- d) Consiste em uma técnica usada exclusivamente na tradução automática.

**Resposta certa:** b) É um método que extrai padrões, insights e informações úteis a partir de grandes quantidades de texto.

**Explicação:** Text mining é o processo de extrair padrões, informações úteis e conhecimento de grandes volumes de dados textuais. Gerar texto é mais próximo do que fazem os LLMs, e corrigir gramática ou traduzir são aplicações pontuais, não a definição.

**Fonte:** Aula de Text Mining, pág. 16 e 23

**Situação:** explicação conferida com o material das aulas

---

## Text Mining, Sentiment Analysis e NLP II

### Questão 193589-1-1
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre tokenização. Para que serve o ToktokTokenizer?

- a) Para dividir um texto em frases, identificando pontos finais e outras pontuações.
- b) Para dividir um texto em palavras (tokens), separando pontuação e símbolos de forma rápida.
- c) Para calcular o sentimento predominante em cada palavra do texto.
- d) Para traduzir automaticamente o texto tokenizado para outro idioma.

**Resposta certa:** b) Para dividir um texto em palavras (tokens), separando pontuação e símbolos de forma rápida.

**Explicação:** O ToktokTokenizer, do NLTK, é um tokenizador de palavras: quebra o texto em tokens e separa pontuação e símbolos, com regras simples que o tornam rápido. Quem divide texto em frases é o sent_tokenize. Os trechos recebidos só tratam de tokenização em geral, não do Toktok.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 193589-1-10
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre expressões regulares (regex). Qual das alternativas abaixo descreve corretamente o que é o regex?

- a) Uma função para ordenar listas de palavras em ordem alfabética.
- b) Uma mini-linguagem para descrever padrões de texto.
- c) Uma ferramenta para calcular o sentimento de uma frase.
- d) Uma biblioteca para treinar modelos de machine learning.

**Resposta certa:** b) Uma mini-linguagem para descrever padrões de texto.

**Explicação:** Regex (expressão regular) é uma mini-linguagem para descrever padrões de texto, usada para buscar, extrair ou substituir trechos. Em Python fica no módulo re. Não ordena listas, não calcula sentimento e não treina modelos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 193589-1-2
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula e responda: O que é o NLTK (Natural Language Toolkit)?

- a) Um algoritmo de machine learning para classificação de imagens.
- b) Uma biblioteca tradicional de Python para processamento de linguagem natural (NLP).
- c) Uma linguagem de programação criada especificamente para análise de sentimento.
- d) Um banco de dados de textos jornalísticos usado apenas para testes acadêmicos.

**Resposta certa:** b) Uma biblioteca tradicional de Python para processamento de linguagem natural (NLP).

**Explicação:** O NLTK (Natural Language Toolkit) é uma biblioteca popular de ferramentas de NLP para Python, com livro próprio disponível online. Não é algoritmo de imagens, linguagem de programação nem banco de dados.

**Fonte:** Data Science do Zero, pág. 359

**Situação:** explicação conferida com o material das aulas

---

### Questão 193589-1-3
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre Stemming. Por que palavras como "comprei", "comprou" e "compraria" são um problema para o computador, caso não haja um tratamento como o Stemming?

- a) Porque o computador não consegue identificar nenhuma dessas palavras como texto válido.
- b) Porque essas palavras são automaticamente removidas durante a limpeza do texto.
- c) Porque essas palavras sempre indicam um erro de digitação no texto.
- d) Porque cada forma é tratada como um token diferente, inflando o vocabulário.

**Resposta certa:** d) Porque cada forma é tratada como um token diferente, inflando o vocabulário.

**Explicação:** Sem stemming, "comprei", "comprou" e "compraria" viram três tokens distintos, mesmo tendo o mesmo radical, o que infla o vocabulário e dispersa a contagem. Com o stemming todas caem em "compr", como no exemplo da aula.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 45

**Situação:** explicação conferida com o material das aulas

---

### Questão 193589-1-4
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula e selecione a alternativa que apresenta duas etapas de Limpeza (Pré-processamento do texto):

- a) Tokenizar o texto e Calcular a frequência das palavras.
- b) Remover URLs e Remover acentos.
- c) Remover acentos e Calcular o sentimento da frase.
- d) Vetorizar o texto e Treinar o modelo de classificação.

**Resposta certa:** b) Remover URLs e Remover acentos.

**Explicação:** Limpeza é a etapa de preparar o texto bruto, e remover URLs e acentos são duas dessas operações. Tokenizar e contar frequência, vetorizar, calcular sentimento e treinar modelo vêm depois. Os trechos recebidos não citam URLs nem acentos, então a resposta se apoia no raciocínio geral.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 193589-1-5
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre Tokenização (Tokenization). O que essa técnica faz com o texto?

- a) Quebra o texto em unidades menores, chamadas tokens.
- b) Traduz o texto para outro idioma.
- c) Corrige automaticamente os erros gramaticais do texto.
- d) Junta várias frases em um único parágrafo.

**Resposta certa:** a) Quebra o texto em unidades menores, chamadas tokens.

**Explicação:** A tokenização divide o texto em unidades menores, os tokens, que podem ser palavras ou pontuação: "Eu amo MBA!" vira ["Eu", "amo", "MBA", "!"]. Não traduz, não corrige erros e não junta frases.

**Fonte:** Aula de Text Mining (pré-processamento), pág. 30

**Situação:** explicação conferida com o material das aulas

---

### Questão 193589-1-6
Área 5 · Text Mining, Sentiment Analysis e NLP II

Em Python, suponha que uma frase tenha sido tokenizada (dividida em palavras e sinais de pontuação) e armazenada na lista tokens. Qual das alternativas abaixo descreve corretamente o que a expressão len(tokens) retorna?

- a) A quantidade de vogais da lista, desconsiderando os sinais de pontuação.
- b) O comprimento médio, em caracteres, dos tokens presente na lista.
- c) A quantidade total de itens na lista, incluindo palavras e sinais de pontuação.
- d) O número de consoantes distintas presentes em todos os tokens da lista.

**Resposta certa:** c) A quantidade total de itens na lista, incluindo palavras e sinais de pontuação.

**Explicação:** len() de uma lista devolve o número de elementos. Se a lista guarda palavras e sinais de pontuação como tokens, cada um conta como um item; por exemplo, ["eu", "amo", "ds", "!"] tem len 4. Não conta vogais, consoantes nem calcula tamanho médio.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 193589-1-7
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre tokenização. Qual é o objetivo da função sent_tokenize()?

- a) Remover a pontuação de um texto antes da análise.
- b) Dividir um texto em palavras individuais, separando pontuação de cada token.
- c) Dividir um texto em frases, identificando onde cada uma termina com base em pontuação e regras linguísticas.
- d) Contar quantas frases diferentes existem em um texto.

**Resposta certa:** c) Dividir um texto em frases, identificando onde cada uma termina com base em pontuação e regras linguísticas.

**Explicação:** sent_tokenize, do NLTK, faz a tokenização em frases: usa pontuação e regras da língua para achar onde cada sentença termina. Quem separa em palavras e pontuação é o word_tokenize (ou o Toktok), e remover pontuação é outra etapa.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 193589-1-8
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre expressões regulares (regex) em Python. Qual é a função do módulo re que encontra todas as ocorrências de um padrão em um texto?

- a) re.count(padrao, texto)
- b) re.findall(padrao, texto)
- c) re.sub(padrao, substituto, texto)
- d) re.remove(padrao, texto)

**Resposta certa:** b) re.findall(padrao, texto)

**Explicação:** No módulo re, re.findall(padrao, texto) devolve todas as ocorrências do padrão. O re.sub substitui, e re.count e re.remove não existem. O livro usa re.findall para extrair as palavras de um texto.

**Fonte:** Data Science do Zero, pág. 344

**Situação:** explicação conferida com o material das aulas

---

### Questão 193589-1-9
Área 5 · Text Mining, Sentiment Analysis e NLP II

Considere os conceitos discutidos em aula sobre a remoção de acentos no pré-processamento de texto e responda: O que caracteriza a decisão de remover acentos de um texto?

- a) É uma regra fixa que deve ser sempre aplicada, sem exceções, em qualquer projeto de NLP.
- b) É uma etapa obrigatória apenas para textos em produção, nunca usada em aula ou estudos.
- c) É uma decisão que envolve vantagens e desvantagens, podendo agrupar erros de digitação, mas também juntar palavras diferentes.
- d) É uma técnica que sempre elimina completamente a ambiguidade entre palavras parecidas.

**Resposta certa:** c) É uma decisão que envolve vantagens e desvantagens, podendo agrupar erros de digitação, mas também juntar palavras diferentes.

**Explicação:** Remover acentos tem prós e contras: agrupa variações como erros de digitação ("não" e "nao"), mas também junta palavras diferentes ("sábia" e "sabia"). Por isso não é regra fixa e não elimina a ambiguidade. Nenhum trecho recebido fala de acentos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Text Mining, Sentiment Analysis e NLP III

### Questão 194788-1-1
Área 5 · Text Mining, Sentiment Analysis e NLP III

De acordo com o que foi discutido em aula, o nível de aspecto é considerado o mais refinado porque foca em quê?

- a) Na classificação de cada sentença individualmente
- b) Em características específicas e essenciais para um feedback detalhado
- c) Na definição da arquitetura do modelo antes da análise
- d) No texto inteiro como uma única opinião

**Resposta certa:** b) Em características específicas e essenciais para um feedback detalhado

**Explicação:** O nível de aspecto é o mais refinado porque foca em características específicas e essenciais para um feedback detalhado, por exemplo o atendimento e a comida de um restaurante. Frase classifica cada sentença, e documento dá uma opinião única ao texto inteiro.

**Fonte:** Aula de Text Mining (granularidade), pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 194788-1-10
Área 5 · Text Mining, Sentiment Analysis e NLP III

De acordo com o que foi discutido em aula, o nível de documento classifica o texto de qual forma?

- a) Classificando cada sentença individualmente
- b) Como uma única opinião, considerando o texto inteiro
- c) Focando em características específicas do produto
- d) Identificando primeiro se é subjetivo ou objetivo

**Resposta certa:** b) Como uma única opinião, considerando o texto inteiro

**Explicação:** O nível de documento classifica o texto inteiro como uma única opinião. É útil para reviews globais, mas pouco detalhado. Classificar sentença por sentença é o nível de frase, e as características do produto são o nível de aspecto.

**Fonte:** Aula de Text Mining (granularidade), pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 194788-1-2
Área 5 · Text Mining, Sentiment Analysis e NLP III

Observe o trecho de código abaixo:

X_test_vec = vectorizer.transform(X_test)

Considerando os conceitos discutidos em aula sobre Text Mining, o que esse comando realiza?

- a) Aprende um novo vocabulário a partir dos textos de teste
- b) Transforma os textos de teste em números usando o mesmo vocabulário aprendido no treino
- c) Treina o modelo de Naive Bayes com os textos de teste
- d) Combina o vocabulário de treino e teste em uma única matriz

**Resposta certa:** b) Transforma os textos de teste em números usando o mesmo vocabulário aprendido no treino

**Explicação:** O transform aplica ao teste o vocabulário já aprendido no treino pelo fit, convertendo os textos em números sem aprender nada novo. Se o teste ensinasse o vocabulário, haveria vazamento de informação. O treino do Naive Bayes é feito por outro método, o fit do classificador.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 194788-1-3
Área 5 · Text Mining, Sentiment Analysis e NLP III

Qual das bibliotecas abaixo foi utilizada em aula para implementar o modelo de Machine Learning?

- a) MinePyLib
- b) DataFlowPy
- c) Scikit-learn
- d) TextCortex

**Resposta certa:** c) Scikit-learn

**Explicação:** O Scikit-learn é a biblioteca de machine learning em Python que fornece o CountVectorizer e o Naive Bayes. As outras opções (MinePyLib, DataFlowPy, TextCortex) não são bibliotecas de ML reconhecidas. Os trechos recebidos não trazem o código da aula.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 194788-1-4
Área 5 · Text Mining, Sentiment Analysis e NLP III

Considerando os conceitos discutidos em aula sobre Text Mining, assinale a alternativa que descreve corretamente o papel do algoritmo Naive Bayes em um processo de classificação de sentimentos.

- a) Criar manualmente os arquivos de exemplos positivos e negativos
- b) Aprender, a partir de exemplos, a associação entre palavras e sentimento
- c) Transformar o texto em vetores numéricos
- d) Testar a performance computacional durante o treinamento

**Resposta certa:** b) Aprender, a partir de exemplos, a associação entre palavras e sentimento

**Explicação:** O Naive Bayes aprende, a partir de exemplos rotulados, as probabilidades de cada palavra em cada classe (como spam ou não spam, ou positivo e negativo) e depois classifica textos novos. Ele não monta os exemplos nem vetoriza o texto, que é papel do vetorizador.

**Fonte:** Data Science do Zero, pág. 236

**Situação:** explicação conferida com o material das aulas

---

### Questão 194788-1-5
Área 5 · Text Mining, Sentiment Analysis e NLP III

Qual foi a proporção de frases reservada para o conjunto de teste durante a aula?

- a) 30%
- b) 70%
- c) 50%
- d) 20%

**Resposta certa:** c) 50%

**Explicação:** O gabarito aponta 50%, mas a proporção usada na aula não aparece em nenhum trecho recebido. O mais comum em prática é reservar 20% a 30% para teste.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** a proporção de teste da aula não consta nos trechos; não dá para confirmar os 50% do gabarito.

---

### Questão 194788-1-6
Área 5 · Text Mining, Sentiment Analysis e NLP III

Considerando os conceitos discutidos em aula sobre Text Mining, assinale a alternativa que indica a técnica utilizada para transformar texto em números antes do treinamento de um modelo de classificação.

- a) Regressão Linear
- b) Naive Bayes
- c) Bag of Words
- d) Árvore de Decisão

**Resposta certa:** c) Bag of Words

**Explicação:** Bag of Words transforma o texto em números contando as palavras de cada documento, gerando um vetor por frase. Regressão linear, Naive Bayes e árvore de decisão são algoritmos de classificação ou regressão, que usam esses números depois.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 194788-1-7
Área 5 · Text Mining, Sentiment Analysis e NLP III

Observe o trecho de código abaixo:

X_train_vec = vectorizer.fit_transform(X_train)

Considerando os conceitos discutidos em aula sobre Text Mining, o que esse comando realiza?

- a) Aprende o vocabulário dos textos de treino e os transforma em uma matriz numérica
- b) Aplica o vocabulário aprendido no treino para transformar os textos de teste
- c) Divide os dados de treino em positivos e negativos
- d) Treina o modelo de Naive Bayes com a matriz numérica

**Resposta certa:** a) Aprende o vocabulário dos textos de treino e os transforma em uma matriz numérica

**Explicação:** fit_transform no treino faz duas coisas: aprende o vocabulário (fit) e converte os textos em matriz numérica (transform). Aplicar o vocabulário ao teste é o transform sozinho, e treinar o Naive Bayes é outra chamada.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 194788-1-8
Área 5 · Text Mining, Sentiment Analysis e NLP III

Em Análise de Sentimentos, a granularidade da análise pode ocorrer em diferentes níveis, como documento, frase ou aspecto. Qual desses níveis é o mais refinado (mais detalhado)?

- a) Nível de frase
- b) Nível de documento
- c) Nível de aspecto
- d) Nível de parágrafo

**Resposta certa:** c) Nível de aspecto

**Explicação:** O nível de aspecto é o mais refinado: o de documento dá uma única opinião ao texto todo, o de frase classifica cada sentença, e o de aspecto separa características específicas. "Parágrafo" não é um dos níveis da aula.

**Fonte:** Aula de Text Mining (granularidade), pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 194788-1-9
Área 5 · Text Mining, Sentiment Analysis e NLP III

Observe o trecho de código abaixo:

vectorizer = CountVectorizer()

Considerando os conceitos discutidos em aula sobre Text Mining, o que esse objeto faz ao ser utilizado?

- a) Separa os dados em conjuntos de treino e teste
- b) Remove pontuação e caracteres especiais dos textos
- c) Transforma textos em números com base na contagem de palavras
- d) Treina um modelo de Naive Bayes para classificar sentimentos

**Resposta certa:** c) Transforma textos em números com base na contagem de palavras

**Explicação:** CountVectorizer transforma textos em números a partir da contagem de palavras (bag of words), montando uma matriz documento por termo. Não divide treino e teste, não é uma etapa de limpeza e não treina o Naive Bayes.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 194788-2-1
Área 5 · Text Mining, Sentiment Analysis e NLP III

De acordo com o que foi discutido em aula, no nível de frase, o que é identificado primeiro antes de definir a polaridade?

- a) Se o texto é um review global
- b) Se o documento inteiro é positivo ou negativo
- c) Se o texto possui características específicas
- d) Se a sentença é subjetiva ou objetiva

**Resposta certa:** d) Se a sentença é subjetiva ou objetiva

**Explicação:** No nível de frase, primeiro se identifica se a sentença é subjetiva ou objetiva e só então se define a polaridade. Faz sentido porque frases objetivas, sem opinião, não têm sentimento a classificar.

**Fonte:** Aula de Text Mining (granularidade), pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 194788-2-4
Área 5 · Text Mining, Sentiment Analysis e NLP III

Considerando os conceitos discutidos em aula sobre Text Mining, no conjunto de teste, o método transform (sem fit) é utilizado para simular:

- a) Frases traduzidas para outro idioma
- b) Frases sem pontuação
- c) Frases novas no mundo real
- d) Frases já vistas no treino

**Resposta certa:** c) Frases novas no mundo real

**Explicação:** No teste usa-se só o transform, com o vocabulário aprendido no treino: o modelo recebe frases que nunca viu, como ocorre em produção. Se o teste participasse do fit, o resultado ficaria otimista demais. Nenhum trecho recebido trata disso.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 194788-2-9
Área 5 · Text Mining, Sentiment Analysis e NLP III

Considerando os conceitos discutidos em aula sobre Text Mining, assinale a alternativa CORRETA sobre como o vocabulário é aprendido ao utilizar o CountVectorizer.

- a) O vocabulário é aprendido com treino e teste juntos, utilizando fit_transform nos dois conjuntos
- b) O vocabulário é aprendido apenas com os dados de teste, utilizando fit_transform
- c) O vocabulário não precisa ser aprendido, pois é gerado automaticamente pelo Naive Bayes
- d) O vocabulário é aprendido apenas com os dados de treino, utilizando fit_transform

**Resposta certa:** d) O vocabulário é aprendido apenas com os dados de treino, utilizando fit_transform

**Explicação:** O vocabulário do CountVectorizer é aprendido só com o treino, via fit_transform. O teste usa apenas transform, para o modelo ser avaliado como se visse frases novas. Aprender o vocabulário com o teste vazaria informação, e o Naive Bayes não gera vocabulário.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---


# Área 6: Gestão (metodologias ágeis, legislação, BI, cloud, engenharia de dados, big data, conjuntura, liderança)

## Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

### Questão 154900-1-1
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Uma análise de conjuntura macroeconômica frequentemente envolve:

- a) A análise de novos entrantes e a probabilidade de produtos substitutos.
- b) A análise da estrutura de mercado e de seu ambiente competitivo.
- c) A análise do comportamento do consumidor em um determinado setor.
- d) A análise dos agregados econômicos de um país ou região como o produto e a renda.

**Resposta certa:** d) A análise dos agregados econômicos de um país ou região como o produto e a renda.

**Explicação:** A conjuntura macroeconômica olha para agregados e políticas do país ou região, como produto e renda, no curto e médio prazo. As outras opções são análise de mercado e de concorrência, ou seja, microeconomia e estratégia de firma.

**Fonte:** Aula de Análise Econômica (conjuntura), pág. 12

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-10
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

A equação PIB = C + I + G + (Ex. – Im.) corresponde à:

- a) A operacionalização do conceito de PIB pela ótica do dispêndio.
- b) A operacionalização do conceito de PIB pela ótica da produção.
- c) A operacionalização do conceito de PIB pela ótica dos setores.
- d) A operacionalização do conceito de PIB pela ótica da oferta.

**Resposta certa:** a) A operacionalização do conceito de PIB pela ótica do dispêndio.

**Explicação:** A resposta é a ótica do dispêndio, também chamada de despesa ou demanda. A soma de consumo, investimento, gastos do governo e exportações líquidas mede quanto se gasta com a produção do país. As outras duas óticas do PIB são a da oferta (produção) e a da renda, com equações diferentes.

**Fonte:** Aula de Nível de Atividade, pág. 8

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-2
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Em determinadas circunstâncias econômicas, o aumento dos gastos de governo e do investimento público podem ser ações de uma estratégia deliberada para:

- a) Diminuição da renda disponível das famílias.
- b) Estatizar a economia e abdicar dos investimentos privados.
- c) Aumentar a demanda agregada de uma economia nos períodos anticíclicos.
- d) Provocar uma inflação na economia para impacto positivo na balança comercial.

**Resposta certa:** c) Aumentar a demanda agregada de uma economia nos períodos anticíclicos.

**Explicação:** Governo gastando mais e investindo mais eleva a demanda agregada, e em períodos anticíclicos (recessão) isso exerce a função estabilizadora, de combater o desemprego e buscar crescimento. Não visa reduzir a renda das famílias nem estatizar a economia.

**Fonte:** Aula de Análise Econômica (papel do governo), pág. 25

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-3
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Qual é o impacto esperado de uma redução da alíquota dos impostos que incidem sobre renda e propriedade para o Produto Interno Bruto de um país?

- a) Redução da renda disponível para o consumo.
- b) Aumento dos gastos do governo.
- c) Aumento do poder de compra da população.
- d) Redução na demanda por investimentos.

**Resposta certa:** c) Aumento do poder de compra da população.

**Explicação:** Reduzir impostos sobre renda e propriedade deixa mais renda disponível, o que aumenta o poder de compra da população e, em geral, o consumo e o PIB. A aula lista a tributação entre os fatores do consumo; reduzir o imposto não eleva os gastos do governo.

**Fonte:** Aula de Análise Econômica (componentes do PIB), pág. 25

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-4
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Qual dos fatores abaixo pode afetar negativamente a balança comercial de um país?

- a) Uma queda das barreiras alfandegárias dos principais parceiros comerciais.
- b) O aumento dos custos de transação para as exportações de bens de consumo.
- c) Uma desvalorização (ou depreciação) da moeda nacional.
- d) A diminuição das importações de bens de consumo por falhas logísticas.

**Resposta certa:** b) O aumento dos custos de transação para as exportações de bens de consumo.

**Explicação:** Custos de transação maiores para exportar encarecem e reduzem as vendas externas, diminuindo as exportações e piorando a balança comercial. Barreiras menores nos parceiros e desvalorização cambial tendem a ajudar as exportações, e importar menos eleva o saldo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 154900-1-5
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Marque a opção que apresenta a correspondência adequada entre o índice de preço ao consumidor e sua principal função na economia brasileira.

- a) IPCA-IBGE, utilizado como indexador de contratos entre agentes econômicos.
- b) ICV-DIEESE, utilizado pelo Governo e Bacen para monitorar a meta de inflação.
- c) IGPM-FGV, utilizado como indexador de contratos entre agentes econômicos.
- d) IPC-FIPE, utilizado pelo Governo e Bacen para monitorar a meta de inflação.

**Resposta certa:** c) IGPM-FGV, utilizado como indexador de contratos entre agentes econômicos.

**Explicação:** Pela aula, o IGP-M da FGV é usado em contratos, ou seja, como indexador entre agentes. O IPCA do IBGE serve à meta de inflação, o IPC-FIPE aos impostos de SP e o ICV-DIEESE a acordos salariais. A tentadora seria o IPCA, mas ele é o índice da meta.

**Fonte:** Aula de Análise Econômica (índices de inflação), pág. 44

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-6
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Se diminuir as importações de um país e suas exportações permanecerem constantes, observaremos:

- a) Um aumento do volume de comércio internacional do país.
- b) Uma diminuição do saldo das Transferências Unilaterais
- c) Um incremento do saldo da Conta Capital.
- d) Um aumento do saldo da Balança Comercial.

**Resposta certa:** d) Um aumento do saldo da Balança Comercial.

**Explicação:** Balança comercial = exportações menos importações. Com as exportações constantes e as importações menores, a diferença cresce e o saldo aumenta. O volume total de comércio, a soma das duas, na verdade diminui.

**Fonte:** Aula de Análise Econômica (balanço de pagamentos), pág. 47

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-7
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

O Nível de Atividade de quaisquer economias pode ser analisado, inicialmente:

- a) Pelo PIB, Taxa de Inflação e a Taxa de Desemprego.
- b) Pelo PIB, PIB per capita e o IDH.
- c) Pelo PIB, Nível de Preços e o Desenvolvimento Sustentável (ODS).
- d) Pelo PIB, Nível de Emprego e a Expectativa de Vida.

**Resposta certa:** a) Pelo PIB, Taxa de Inflação e a Taxa de Desemprego.

**Explicação:** A resposta é PIB, taxa de inflação e taxa de desemprego porque o nível de atividade resume três objetivos da economia: crescimento do produto, estabilidade de preços e geração de emprego, e cada um tem um indicador próprio (PIB, inflação, desemprego). IDH, expectativa de vida e ODS tratam de desenvolvimento e bem-estar, não de nível de atividade.

**Fonte:** Aula de Nível de Atividade, pág. 20

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-8
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

A Taxa de Desemprego de um país é definida como sendo a relação entre:

- a) O número de pessoas que estão procurando emprego e a população total do país.
- b) O número de desempregados e a população em idade ativa do país.
- c) O número de desempregados e a população total do país.
- d) O número de desempregados e a população economicamente ativa do país.

**Resposta certa:** d) O número de desempregados e a população economicamente ativa do país.

**Explicação:** A resposta é desempregados sobre a população economicamente ativa (PEA). A taxa de desemprego mede quantos dos que estão na força de trabalho, ocupados ou procurando vaga, estão sem ocupação. Usar a população total ou a em idade ativa no denominador incluiria inativos, que não pressionam o mercado de trabalho.

**Fonte:** Aula de Mercado de Trabalho e Taxa de Desemprego, pág. 16

**Situação:** explicação conferida com o material das aulas

---

### Questão 154900-1-9
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas I

Mecanização agrícola, incompatibilidade geográfica entre oferta e demanda no mercado de trabalho e recessão econômica explicam, respectivamente, os desempregos:

- a) Estrutural, conjuntural e friccional.
- b) Friccional, cíclico e conjuntural.
- c) Cíclico, estrutural e friccional.
- d) Estrutural, friccional e conjuntural.

**Resposta certa:** d) Estrutural, friccional e conjuntural.

**Explicação:** A resposta é estrutural, friccional e conjuntural, nessa ordem. Mecanização agrícola muda a estrutura produtiva e elimina postos de forma duradoura (estrutural). Desencontro geográfico entre vaga e trabalhador é um problema de ajuste do mercado (friccional). Recessão derruba a demanda por um tempo (conjuntural, também chamado de cíclico).

**Fonte:** Aula de Tipos de Desemprego, pág. 17

**Situação:** explicação conferida com o material das aulas

---

## Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

### Questão 155564-1-1
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

O que são operações de open market?

- a) São operações de compra e venda de títulos no mercado secundário (papéis emitidos anteriormente pelo governo já em circulação).
- b) São operações de empréstimos diretos do Banco Central aos bancos comerciais a uma taxa de juros pré-determinada.
- c) São operações de emissão primária de novos títulos públicos pelo Tesouro Nacional para financiar o déficit fiscal.
- d) São operações de compra e venda de moeda estrangeira realizadas pelo Banco Central para controlar a taxa de câmbio.

**Resposta certa:** a) São operações de compra e venda de títulos no mercado secundário (papéis emitidos anteriormente pelo governo já em circulação).

**Explicação:** A resposta é a compra e venda de títulos no mercado secundário, isto é, papéis do governo que já estavam em circulação. O Banco Central compra ou vende esses títulos para enxugar ou injetar liquidez e controlar a oferta monetária. Emissão nova pelo Tesouro e compra de moeda estrangeira são outras operações.

**Fonte:** Aula de Política Monetária, pág. 40

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-10
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

Entre as políticas econômicas conjunturais, pode-se citar:

- a) A política de regularização fundiária e de reforma agrária.
- b) A política de distribuição de renda e de estratificação social.
- c) A política monetária que define a taxa de juros e a oferta monetária.
- d) A política de infraestrutura que favorece os investimentos produtivos.

**Resposta certa:** c) A política monetária que define a taxa de juros e a oferta monetária.

**Explicação:** A resposta é a política monetária, que define juros e oferta de moeda. As políticas conjunturais são a fiscal, a monetária e a cambial, voltadas a ajustes de curto prazo. Reforma agrária, distribuição de renda e infraestrutura são políticas estruturais, de mudança mais lenta e profunda.

**Fonte:** Aula de Políticas Econômicas Conjunturais, pág. 24

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-2
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

O tripé macroeconômico, nome dado a um rol de orientações que regem a política econômica em muitos países que perfazem as principais economias do mundo, é composto por diretrizes como:

- a) Meta de taxa de inflação e câmbio flutuante.
- b) Meta de déficit primário e câmbio fixo.
- c) Câmbio flutuante e meta de taxa de desemprego natural.
- d) Câmbio fixo e meta de inflação.

**Resposta certa:** a) Meta de taxa de inflação e câmbio flutuante.

**Explicação:** A resposta é meta de inflação e câmbio flutuante. O tripé macroeconômico combina meta de inflação (política monetária), regime de câmbio flutuante (política cambial) e meta de superávit primário (política fiscal). As opções com câmbio fixo ou meta de desemprego natural não fazem parte do tripé.

**Fonte:** Aula de Políticas Econômicas Conjunturais, pág. 53

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-3
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

Qual dos fatores abaixo é plausível para explicar a taxa de crescimento negativa do PIB brasileiro – de -3,9% – no ano de 2020, primeiro ano da pandemia de Covid-19?

- a) Valorização do real frente ao dólar.
- b) Crescimento dos investimentos produtivos.
- c) Diminuição da taxa de desemprego.
- d) Diminuição da renda disponível das famílias.

**Resposta certa:** d) Diminuição da renda disponível das famílias.

**Explicação:** A resposta é a diminuição da renda disponível das famílias. O consumo é o maior componente do PIB, e menos renda para gastar reduz a demanda e a atividade, o que combina com a queda de 2020. Crescimento dos investimentos e queda do desemprego puxariam o PIB para cima, e o real se desvalorizou naquele ano. A aula traz questão parecida com outro valor (-3,3%).

**Fonte:** Aula de Componentes do PIB, pág. 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-4
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

O orçamento do governo de um pequeno país apresenta os seguintes valores: as receitas totalizam R$ 220 bilhões/ano, as despesas (exceto pagamento de juros) totalizam R$ 195 bilhões/ano e as despesas com juros da dívida pública totalizam R$ 45 bilhões/ano. Pode-se afirmar que este país tem um resultado primário e um resultado nominal que são, respectivamente:

- a) Um superávit primário e um déficit nominal.
- b) Um superávit primário e um superávit nominal.
- c) Um déficit primário e um superávit nominal.
- d) Um déficit primário e um déficit nominal.

**Resposta certa:** a) Um superávit primário e um déficit nominal.

**Explicação:** A resposta é superávit primário e déficit nominal. O primário exclui juros: 220 - 195 = +25 bilhões. O nominal inclui os juros: 220 - (195 + 45) = -20 bilhões. Os juros da dívida são o que faz o resultado virar déficit.

**Fonte:** Aula de Resultado Primário e Nominal, pág. 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-5
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

Considere os tipos de impostos e a política tributária no Brasil e assinale a alternativa CORRETA:

- a) Os impostos indiretos são progressivos e incidem principalmente sobre a renda, enquanto os impostos diretos são regressivos e incidem sobre o consumo.
- b) Os impostos diretos incidem sobre renda e propriedade, já os impostos indiretos sobre a venda de bens e serviços.
- c) O ICMS e o IR são exemplos de impostos diretos, pois são cobrados diretamente do contribuinte no momento da compra.
- d) Os impostos proporcionais variam conforme a capacidade contributiva, sendo o IPTU um exemplo típico de imposto regressivo.

**Resposta certa:** b) Os impostos diretos incidem sobre renda e propriedade, já os impostos indiretos sobre a venda de bens e serviços.

**Explicação:** A resposta é a que diz que impostos diretos incidem sobre renda e propriedade (IRPF, IPTU, IPVA) e os indiretos sobre a venda de bens e serviços (ICMS, IPI, ISS). Nas demais, os conceitos aparecem trocados: ICMS é indireto, e o imposto direto recai sobre quem paga e não embutido no preço do produto.

**Fonte:** Aula de Tipos de Impostos e Política Tributária, pág. 28

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-6
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

Entre os instrumentos clássicos (ou tradicionais) de política monetária, encontra-se:

- a) A operação de open market.
- b) O regime cambial flutuante.
- c) O controle de preços dos bens não-administrados pelo governo.
- d) A meta de superávit primário.

**Resposta certa:** a) A operação de open market.

**Explicação:** A resposta é a operação de open market. Os instrumentos clássicos de política monetária são open market, taxa de compulsório e taxa de redesconto. Regime cambial é política cambial, e meta de superávit primário é política fiscal.

**Fonte:** Aula de Política Monetária, pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-7
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

Qual das alternativas abaixo representa uma função do Banco Central na economia brasileira contemporânea?

- a) Indicar os setores e negócios para o investimento público.
- b) Definir a taxa de juros básica (SELIC) da economia.
- c) Determinar a meta de inflação.
- d) Financiar o déficit público.

**Resposta certa:** b) Definir a taxa de juros básica (SELIC) da economia.

**Explicação:** A resposta é definir a taxa básica de juros, a Selic, que o Banco Central fixa nas reuniões do Copom. A meta de inflação é a tentação aqui, mas ela é definida pelo Conselho Monetário Nacional e o Banco Central persegue essa meta. Indicar setores de investimento e financiar o déficit não são funções dele.

**Fonte:** Aula de Política Monetária, pág. 38

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-8
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

Qual das alternativas abaixo representa três instrumentos clássicos de política monetária?

- a) Política fiscal, gasto público e arrecadação tributária.
- b) Meta de inflação, superávit primário e taxa de juros real.
- c) Taxa Selic, taxa de câmbio e controle de preços.
- d) Open market, taxa compulsório e taxa de redesconto.

**Resposta certa:** d) Open market, taxa compulsório e taxa de redesconto.

**Explicação:** A resposta é open market, taxa de compulsório e taxa de redesconto, que são os três instrumentos clássicos de política monetária. As outras opções misturam política fiscal (gasto, arrecadação, superávit primário), metas e variáveis como câmbio e controle de preços, que não são instrumentos clássicos de política monetária.

**Fonte:** Aula de Política Monetária, pág. 39

**Situação:** explicação conferida com o material das aulas

---

### Questão 155564-1-9
Área 6 · Análise da Conjuntura Econômica em Cenários de Tecnologias Disruptivas II

O Boletim Focus do Banco Central é utilizado para:

- a) A divulgação dos instrumentos de política monetária mobilizados pelo Bacen.
- b) A divulgação da ata do Copom após cada reunião de decisão sobre a taxa Selic.
- c) A divulgação da oferta de títulos públicos, semanalmente, do Tesouro Nacional.
- d) A divulgação das expectativas do mercado, semanalmente, para variáveis macroeconômicas.

**Resposta certa:** d) A divulgação das expectativas do mercado, semanalmente, para variáveis macroeconômicas.

**Explicação:** A resposta é a divulgação semanal das expectativas do mercado para variáveis macroeconômicas. O Boletim Focus reúne projeções de instituições financeiras para inflação, juros, câmbio e PIB. A ata do Copom é outro documento, publicada após cada reunião sobre a Selic.

**Fonte:** Aula de Política Monetária, pág. 43

**Situação:** explicação conferida com o material das aulas

---

## Big Data e Deployment de Modelos I

### Questão 179551-1-1
Área 6 · Big Data e Deployment de Modelos I

Sobre MLOps, assinale a alternativa CORRETA:

- a) Facilita a colaboração entre cientistas de dados e engenheiros de software, acelerando a entrega de modelos escaláveis em produção.
- b) Substitui completamente as práticas de DevOps nas organizações, tornando desnecessária a integração entre equipes de desenvolvimento e operações.
- c) Consiste em uma metodologia voltada exclusivamente ao treinamento de modelos, sem envolver etapas de monitoramento ou atualização em produção.
- d) Tem como principal objetivo reduzir o volume de dados utilizados no treinamento, garantindo maior eficiência computacional nos pipelines.

**Resposta certa:** a) Facilita a colaboração entre cientistas de dados e engenheiros de software, acelerando a entrega de modelos escaláveis em produção.

**Explicação:** A resposta é a que diz que o MLOps facilita a colaboração entre cientistas de dados e engenheiros de software e acelera a entrega de modelos escaláveis em produção. Ele estende as ideias do DevOps para o ciclo de vida de modelos, sem substituí-lo, e cobre também monitoramento e atualização, não só o treino.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-10
Área 6 · Big Data e Deployment de Modelos I

Qual das alternativas abaixo apresenta um benefício do MLflow?

- a) Geração automática de dados sintéticos para compensar conjuntos de dados insuficientes durante o treinamento de modelos.
- b) Eliminação da necessidade de infraestrutura de servidores.
- c) Simplificação do deploy e monitoramento de modelos em produção.
- d) Substituição completa das etapas de pré-processamento e feature engineering no pipeline de machine learning.

**Resposta certa:** c) Simplificação do deploy e monitoramento de modelos em produção.

**Explicação:** A resposta é a simplificação do deploy e do monitoramento de modelos em produção, que é o que o MLflow entrega ao padronizar empacotamento, registro e implantação. Ele não gera dados sintéticos, não dispensa servidores e não substitui pré-processamento nem feature engineering.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-2
Área 6 · Big Data e Deployment de Modelos I

Sobre um modelo em produção no MLFlow, assinale a alternativa CORRETA:

- a) Um modelo arquivado não consegue ser utilizado para consumo.
- b) Um modelo só deve ter uma versão.
- c) O MLflow não trabalha com o conceito de deployment de modelos.
- d) Um modelo pode ter diversas versões diferentes em estágios diferentes (adaptação, produção e arquivado).

**Resposta certa:** d) Um modelo pode ter diversas versões diferentes em estágios diferentes (adaptação, produção e arquivado).

**Explicação:** A resposta é que um modelo pode ter várias versões em estágios diferentes. No registro de modelos do MLflow cada versão registrada passa por estágios, como staging (a de adaptação), produção e arquivado. Versão arquivada continua acessível, só não é a ativa, e o MLflow trata sim de deployment.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-3
Área 6 · Big Data e Deployment de Modelos I

Qual dos softwares abaixo é considerado um framework para trabalhar com o ciclo de vida e gerenciamento de modelos?

- a) MLFlow.
- b) RStudio.
- c) Excel.
- d) Power BI.

**Resposta certa:** a) MLFlow.

**Explicação:** A resposta é o MLflow, plataforma de código aberto para gerenciar o ciclo de vida de modelos: experimentos, empacotamento, registro e implantação. RStudio é um ambiente de desenvolvimento, Excel é planilha e Power BI é ferramenta de visualização.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-4
Área 6 · Big Data e Deployment de Modelos I

Sobre o MLflow Models, assinale a alternativa CORRETA:

- a) Padroniza a estrutura e o empacotamento do código, garantindo que experimentos possam ser reproduzidos em diferentes ambientes.
- b) Oferece um formato unificado para salvar e implantar modelos em diferentes plataformas.
- c) Registra e versiona modelos treinados, permitindo controlar seu ciclo de vida desde o desenvolvimento até a produção.
- d) Rastreia métricas, parâmetros e artefatos gerados durante a execução de experimentos de machine learning.

**Resposta certa:** b) Oferece um formato unificado para salvar e implantar modelos em diferentes plataformas.

**Explicação:** A resposta é a que fala em formato unificado para salvar e implantar modelos em diferentes plataformas. O MLflow Models define um padrão de empacotamento (os flavors). As outras alternativas descrevem outros componentes: padronizar o código é o MLflow Projects, versionar é o Model Registry e rastrear métricas é o Tracking.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-5
Área 6 · Big Data e Deployment de Modelos I

O que significa a sigla API?

- a) Advanced Platform Integration.
- b) Advanced Programming Interface.
- c) Application Platform Interface.
- d) Application Programming Interface.

**Resposta certa:** d) Application Programming Interface.

**Explicação:** A resposta é Application Programming Interface, ou interface de programação de aplicações. É o contrato pelo qual um programa pede serviços ou dados a outro, como um modelo em produção que recebe requisições e devolve previsões.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-6
Área 6 · Big Data e Deployment de Modelos I

Em relação às API e modelos em produção, assinale a afirmativa CORRETA:

- a) Uma API não pode se comunicar com um modelo em produção, sendo necessário armazenar o resultado previamente em um banco de dados.
- b) Uma rota de uma API pode consumir um modelo em produção do MLFlow e retornar o resultado para quem fez a solicitação.
- c) Uma rota de uma API não pode fornecer o predict de um modelo.
- d) Modelos em produção e API não tem nenhuma relação entre si.

**Resposta certa:** b) Uma rota de uma API pode consumir um modelo em produção do MLFlow e retornar o resultado para quem fez a solicitação.

**Explicação:** A resposta é que uma rota de API pode consumir um modelo em produção do MLflow e devolver o resultado a quem pediu. É o uso mais comum: a rota recebe os dados, chama o predict do modelo carregado e retorna a previsão, sem precisar gravar nada antes em banco.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-7
Área 6 · Big Data e Deployment de Modelos I

Considere os conceitos discutidos em aula e responda: Qual é um desafio comum no deployment de modelos?

- a) O fato de modelos treinados com grandes volumes de dados apresentarem desempenho inferior em produção.
- b) A impossibilidade de reutilizar hiperparâmetros otimizados durante o treinamento na etapa de inferência.
- c) A ausência de frameworks de treinamento compatíveis com Python.
- d) A diferença entre ambientes de desenvolvimento e produção.

**Resposta certa:** d) A diferença entre ambientes de desenvolvimento e produção.

**Explicação:** A resposta é a diferença entre ambientes de desenvolvimento e produção. Versões de bibliotecas, dependências, volume de dados e infraestrutura mudam entre os dois, e um modelo que roda no notebook pode falhar ou se comportar diferente no servidor. Python tem frameworks de sobra, e hiperparâmetros treinados podem ser reaproveitados.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-8
Área 6 · Big Data e Deployment de Modelos I

Quais são as informações que o MLFlow consegue gerenciar no ciclo de vida de um modelo?

- a) Parâmetros e métricas dos modelos.
- b) Apenas as métricas dos modelos.
- c) Apenas os parâmetros dos modelos.
- d) Parâmetros, métricas, artefatos e os dados do modelo.

**Resposta certa:** d) Parâmetros, métricas, artefatos e os dados do modelo.

**Explicação:** A resposta é parâmetros, métricas, artefatos e os dados do modelo. O MLflow guarda não só parâmetros e métricas de cada execução, mas também artefatos (arquivos como o modelo serializado e gráficos) e as informações do modelo. As opções com apenas métricas ou apenas parâmetros são incompletas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179551-1-9
Área 6 · Big Data e Deployment de Modelos I

Qual é o objetivo central do componente MLflow Tracking?

- a) Gerenciar experimentos, rastreando métricas, parâmetros e resultados de cada execução.
- b) Disponibilizar o modelo treinado como um serviço de inferência acessível via API REST.
- c) Empacotar o código e as dependências do modelo em um formato reproduzível e portável.
- d) Registrar e versionar modelos treinados, controlando seu ciclo de vida até a produção.

**Resposta certa:** a) Gerenciar experimentos, rastreando métricas, parâmetros e resultados de cada execução.

**Explicação:** A resposta é gerenciar experimentos, registrando métricas, parâmetros e resultados de cada execução. Esse é o MLflow Tracking. Servir o modelo por API REST, empacotar o código e versionar modelos pertencem a outros componentes (Models, Projects e Model Registry).

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Big Data e Deployment de Modelos II

### Questão 179780-1-1
Área 6 · Big Data e Deployment de Modelos II

Estima-se que em 2025 o volume global de dados atingiu aproximadamente 180 zettabytes. Qual dos fatores abaixo está mais ligado à recente explosão no volume de dados gerados no mundo?

- a) O boom da Inteligência Artificial Generativa, que impulsionou a criação massiva de dados sintéticos, textos, imagens e modelos em escala global.
- b) A redução no número de usuários de internet, que forçou as empresas a coletarem dados com maior frequência para compensar a queda no tráfego digital.
- c) A substituição dos dispositivos móveis por computadores desktop, que por terem maior capacidade de armazenamento, passaram a registrar volumes maiores de dados por usuário.
- d) O declínio das redes sociais, que levou os usuários a migrarem para plataformas offline e a gerarem dados de forma mais controlada e centralizada.

**Resposta certa:** a) O boom da Inteligência Artificial Generativa, que impulsionou a criação massiva de dados sintéticos, textos, imagens e modelos em escala global.

**Explicação:** A resposta é o boom da IA generativa. Texto, imagem, vídeo e dados sintéticos gerados por esses modelos aceleraram o crescimento do volume global de dados. As outras opções contradizem a realidade: o número de usuários de internet cresce, o celular segue dominante e as redes sociais não declinaram.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-10
Área 6 · Big Data e Deployment de Modelos II

Qual é a biblioteca de Machine Learning integrada ao Apache Spark?

- a) MLlib.
- b) Scikit-learn.
- c) XGBoost.
- d) TensorFlow.

**Resposta certa:** a) MLlib.

**Explicação:** A resposta é MLlib, a biblioteca de machine learning que vem com o Apache Spark. Scikit-learn, XGBoost e TensorFlow são bibliotecas independentes, que podem ser usadas junto com o Spark mas não são integradas a ele.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-2
Área 6 · Big Data e Deployment de Modelos II

Assinale a alternativa que apresenta dois componentes do Apache Spark.

- a) ETL (Extract, Transform, Load) e OLAP (Online Analytical Processing).
- b) API Gateway e Load Balancer.
- c) DAG (Directed Acyclic Graph) e RDD (Resilient Distributed Dataset).
- d) HDFS (Hadoop Distributed File System) e YARN (Yet Another Resource Negotiator).

**Resposta certa:** c) DAG (Directed Acyclic Graph) e RDD (Resilient Distributed Dataset).

**Explicação:** A resposta é DAG e RDD. O Spark organiza o trabalho em grafos acíclicos dirigidos (DAG) de operações sobre RDDs, os conjuntos de dados distribuídos e resilientes. HDFS e YARN são componentes do ecossistema Hadoop, e ETL, OLAP, API Gateway e Load Balancer não são componentes do Spark.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-3
Área 6 · Big Data e Deployment de Modelos II

Qual das afirmativas abaixo está mais alinhada ao conceito de Big Data?

- a) Big Data é uma técnica de compressão de dados que permite armazenar grandes volumes de informação em servidores locais com menor custo de infraestrutura, sem exigir mudanças nas ferramentas de processamento existentes.
- b) Big Data é um termo que descreve exclusivamente o armazenamento distribuído de dados em nuvem, sendo aplicável apenas a empresas de tecnologia que lidam com transações financeiras em tempo real.
- c) Big Data consiste em um conjunto de algoritmos de aprendizado de máquina desenvolvidos especificamente para operar em bancos de dados relacionais de grande porte, como os utilizados em sistemas ERP corporativos.
- d) Big Data refere-se a conjuntos de dados extremamente grandes e complexos que não podem ser facilmente processados ou gerenciados com ferramentas de processamento de dados tradicionais.

**Resposta certa:** d) Big Data refere-se a conjuntos de dados extremamente grandes e complexos que não podem ser facilmente processados ou gerenciados com ferramentas de processamento de dados tradicionais.

**Explicação:** A resposta é a que define Big Data como conjuntos de dados muito grandes e complexos, difíceis de processar com ferramentas tradicionais. Não é técnica de compressão, nem se restringe à nuvem ou a empresas de tecnologia, nem é um conjunto de algoritmos de machine learning.

**Fonte:** Manual de Análise de Dados (Fávero), pág. 13

**Situação:** explicação conferida com o material das aulas

---

### Questão 179780-1-4
Área 6 · Big Data e Deployment de Modelos II

Uma das características do Hadoop MapReduce é a escalabilidade. O que isso significa na prática?

- a) Significa que o Hadoop MapReduce comprime os dados automaticamente à medida que o volume cresce, reduzindo o espaço ocupado nos servidores existentes.
- b) Significa que o sistema limita o volume de dados processados simultaneamente para garantir a estabilidade e o desempenho do cluster.
- c) Significa que o sistema ajusta automaticamente a qualidade dos dados processados conforme o volume aumenta, priorizando os registros mais recentes.
- d) Significa que é possível adicionar mais servidores conforme a necessidade para lidar com o aumento no volume de dados.

**Resposta certa:** d) Significa que é possível adicionar mais servidores conforme a necessidade para lidar com o aumento no volume de dados.

**Explicação:** A resposta é que dá para adicionar mais servidores conforme o volume de dados cresce. Escalabilidade no MapReduce é horizontal: o cluster ganha nós e o processamento se distribui entre eles. Não tem a ver com compressão, limite de volume nem com priorizar registros mais recentes.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-5
Área 6 · Big Data e Deployment de Modelos II

Quais são os 5 V's do Big Data apresentados em aula?

- a) Veracidade, Valor, Variedade, Velocidade e Volume.
- b) Veracidade, Valor, Velocidade, Volume e Virtualização.
- c) Veracidade, Valor, Variedade, Volume e Validade.
- d) Veracidade, Valor, Variedade, Velocidade e Visibilidade.

**Resposta certa:** a) Veracidade, Valor, Variedade, Velocidade e Volume.

**Explicação:** A resposta é veracidade, valor, variedade, velocidade e volume, a versão mais usada dos 5 Vs. Virtualização, validade e visibilidade não fazem parte dessa lista. O Fávero usa outras cinco dimensões (volume, velocidade, variedade, variabilidade e complexidade), mas só uma alternativa traz a lista mais comum.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-6
Área 6 · Big Data e Deployment de Modelos II

Assinale a alternativa que apresenta duas características centrais do Apache Spark.

- a) Processamento In-Memory e suporte a diversos tipos de dados.
- b) Processamento em disco e suporte exclusivo a dados estruturados em formato tabular.
- c) Armazenamento distribuído de arquivos e gerenciamento de recursos em clusters via YARN.
- d) Conteinerização de aplicações e orquestração automática de pipelines em microsserviços.

**Resposta certa:** a) Processamento In-Memory e suporte a diversos tipos de dados.

**Explicação:** A resposta é processamento in-memory e suporte a diversos tipos de dados. O Spark mantém dados em memória entre as etapas, o que o torna rápido, e lida com dados estruturados, semiestruturados e em fluxo. Armazenamento distribuído e YARN são do Hadoop, e conteinerização não é característica do Spark.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-7
Área 6 · Big Data e Deployment de Modelos II

Considere os conceitos discutidos em aula sobre o Apache Spark e assinale a alternativa INCORRETA:

- a) O Apache Spark utiliza DataFrames como principal estrutura de dados, organizados em formato tabular (linhas e colunas).
- b) O Apache Spark é eficaz no processamento de dados em diferentes formatos, como Parquet, CSV e JSON, entre outros.
- c) O Spark Streaming permite processamento em tempo real, sendo útil para lidar com a velocidade dos dados.
- d) A implementação de algoritmos de aprendizado de máquina no Apache Spark é complexa, uma vez que a ferramenta não possui uma biblioteca de machine learning integrada.

**Resposta certa:** d) A implementação de algoritmos de aprendizado de máquina no Apache Spark é complexa, uma vez que a ferramenta não possui uma biblioteca de machine learning integrada.

**Explicação:** A resposta é a quarta alternativa, que é a falsa: o Spark tem biblioteca de machine learning integrada, o MLlib, o que facilita implementar algoritmos. As outras três afirmações são verdadeiras: DataFrames tabulares, leitura de Parquet, CSV e JSON, e processamento em tempo real com Spark Streaming.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-8
Área 6 · Big Data e Deployment de Modelos II

Assinale a alternativa que apresenta uma diferença entre o Hadoop MapReduce e o Apache Spark.

- a) Ao contrário do Hadoop, que oferece suporte nativo a Machine Learning, o Spark não possui bibliotecas para modelagem preditiva ou análise estatística.
- b) Ao contrário do Hadoop, que opera exclusivamente em ambientes de nuvem pública, o Spark foi projetado para funcionar apenas em servidores locais (on-premise).
- c) Ao contrário do Hadoop, que grava dados no disco entre as etapas do processamento, o Spark realiza processamento em memória.
- d) Ao contrário do Hadoop, que utiliza a linguagem Python como padrão, o Spark foi desenvolvido para operar exclusivamente com a linguagem Scala.

**Resposta certa:** c) Ao contrário do Hadoop, que grava dados no disco entre as etapas do processamento, o Spark realiza processamento em memória.

**Explicação:** A resposta é que o Hadoop MapReduce grava dados em disco entre as etapas, enquanto o Spark processa em memória, o que o deixa bem mais rápido em tarefas iterativas. O Spark tem bibliotecas de ML, roda em nuvem e local e aceita Python, Scala, Java e R.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 179780-1-9
Área 6 · Big Data e Deployment de Modelos II

Assinale a alternativa que apresenta três características centrais do Hadoop MapReduce.

- a) Armazenamento centralizado, alta disponibilidade e processamento em grafos acíclicos dirigidos (DAG).
- b) Escalabilidade, containerização automática e orquestração de microsserviços em clusters.
- c) Processamento em memória, baixa latência e suporte nativo a streaming de dados em tempo real.
- d) Armazenamento distribuído, processamento distribuído e escalabilidade.

**Resposta certa:** d) Armazenamento distribuído, processamento distribuído e escalabilidade.

**Explicação:** A resposta é armazenamento distribuído, processamento distribuído e escalabilidade. O Hadoop guarda os dados espalhados pelo cluster (HDFS), processa em paralelo com o MapReduce e cresce acrescentando nós. Processamento em memória e streaming são do Spark, e containerização não é do Hadoop.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Business Intelligence e Data Visualization I

### Questão 147517-1-1
Área 6 · Business Intelligence e Data Visualization I

Em um processo eficiente de análise de dados, é essencial:

- a) Compreender a situação atual, identificar oportunidades e dar suporte a decisões estratégicas.
- b) Começar criando o dashboard antes mesmo da análise dos dados.
- c) Utilizar apenas planilhas que já estejam prontas e bem organizadas.
- d) Priorizar trabalhar com arquivos desconectados entre si.

**Resposta certa:** a) Compreender a situação atual, identificar oportunidades e dar suporte a decisões estratégicas.

**Explicação:** A resposta é compreender a situação atual, identificar oportunidades e apoiar decisões estratégicas, que é o propósito da análise de dados. Começar pelo dashboard antes de analisar, depender só de planilhas prontas ou trabalhar com arquivos desconectados atrapalham o processo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-10
Área 6 · Business Intelligence e Data Visualization I

São considerados fatores determinantes para o sucesso de projetos de Business Intelligence, exceto:

- a) Iniciar a construção do dashboard sem uma estratégia de análise bem estruturada.
- b) A implantação da cultura orientada a dados (Data Driven).
- c) A capacitação da equipe com habilidades analíticas.
- d) O gerenciamento de dados eficaz.

**Resposta certa:** a) Iniciar a construção do dashboard sem uma estratégia de análise bem estruturada.

**Explicação:** A exceção é iniciar o dashboard sem estratégia de análise. Um painel feito antes de definir quais perguntas ele precisa responder tende a virar um conjunto de gráficos sem utilidade. Cultura data driven, equipe capacitada e boa gestão de dados são justamente os fatores que sustentam um projeto de BI.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-2
Área 6 · Business Intelligence e Data Visualization I

Ao desenvolver um dashboard, qual das opções representa uma boa prática na escolha de gráficos?

- a) Sempre optar por gráficos de rosca com muitas divisões.
- b) Utilizar prioritariamente gráficos de linhas, independentemente do contexto.
- c) Os gráficos mais indicados são sempre o de pizza e linhas, pois são os mais comuns.
- d) A escolha do gráfico deve ser feita conforme o tipo de dado e a mensagem que se quer transmitir.

**Resposta certa:** d) A escolha do gráfico deve ser feita conforme o tipo de dado e a mensagem que se quer transmitir.

**Explicação:** A resposta é escolher o gráfico conforme o tipo de dado e a mensagem a transmitir. Cada gráfico serve a um propósito: barras para comparar categorias, linhas para evolução no tempo. Rosca com muitas divisões fica ilegível e nenhum tipo é o melhor em todos os contextos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-3
Área 6 · Business Intelligence e Data Visualization I

Assinale a alternativa que contém duas ferramentas de análise de dados e Business Intelligence.

- a) Power BI e Tableau.
- b) Photoshop e Illustrator.
- c) Trello e Slack.
- d) PowerPoint e Word.

**Resposta certa:** a) Power BI e Tableau.

**Explicação:** A resposta é Power BI e Tableau, duas ferramentas de BI e visualização de dados. Photoshop e Illustrator são de design gráfico, Trello e Slack são de gestão e comunicação, e PowerPoint e Word são de apresentação e texto.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-4
Área 6 · Business Intelligence e Data Visualization I

No contexto do Power BI, o principal objetivo do Power Query é:

- a) Transformar, limpar e preparar os dados antes da análise.
- b) Analisar diretamente os gráficos.
- c) Criar objetos gráficos no dashboard.
- d) Apenas importar dados simples, como planilhas.

**Resposta certa:** a) Transformar, limpar e preparar os dados antes da análise.

**Explicação:** A resposta é transformar, limpar e preparar os dados antes da análise. O Power Query é o editor de ETL do Power BI: conecta a várias fontes, trata colunas, remove erros e junta tabelas. Criar visuais e analisar gráficos acontece depois, na parte de relatório.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-5
Área 6 · Business Intelligence e Data Visualization I

Considerando as fontes de dados que podem ser integradas ao Power BI, assinale a alternativa INCORRETA:

- a) Arquivos TXT e arquivos CSV podem ser integrados ao Power BI.
- b) Dados disponíveis na internet e arquivos CSV podem ser integrados ao Power BI.
- c) Bancos de dados como SQL Server e Oracle podem ser integrados, mas o MySQL não é compatível.
- d) Arquivos Excel e planilhas podem ser integrados.

**Resposta certa:** c) Bancos de dados como SQL Server e Oracle podem ser integrados, mas o MySQL não é compatível.

**Explicação:** A questão pede a incorreta, e é a que diz que o MySQL não é compatível. O Power BI se conecta ao MySQL, além de SQL Server e Oracle, e também a TXT, CSV, Excel e dados da web. As outras três afirmações são verdadeiras.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-6
Área 6 · Business Intelligence e Data Visualization I

Em relação ao conceito de Business Intelligence (BI), assinale a alternativa INCORRETA:

- a) Business Intelligence resume-se a uma ferramenta específica chamada Power BI.
- b) Representa um conceito de gestão e análise de dados, e não uma tecnologia isolada.
- c) Pode ser aplicado em diversos setores como indústria, saúde, tecnologia e varejo online.
- d) Envolve análise de dados para gerar informações úteis e apoiar as decisões estratégicas.

**Resposta certa:** a) Business Intelligence resume-se a uma ferramenta específica chamada Power BI.

**Explicação:** A questão pede a incorreta, e é a que reduz o BI ao Power BI. BI é um conceito de gestão e análise de dados para gerar informação e apoiar decisões, aplicável a vários setores, e o Power BI é só uma das ferramentas que o apoiam.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-7
Área 6 · Business Intelligence e Data Visualization I

Assinale a alternativa que contém exemplos de funções que podem ser utilizadas na criação de medidas no Power BI:

- a) Soma() e Tableau.
- b) Sum() e Average().
- c) Power Query e Linguagem M.
- d) KPI e DAX.

**Resposta certa:** b) Sum() e Average().

**Explicação:** A resposta é Sum() e Average() porque são funções DAX, a linguagem usada para escrever medidas no Power BI (por exemplo, Total = SUM(Vendas[Valor])). Tableau é outra ferramenta, e Power Query com Linguagem M serve para transformar dados antes de carregá-los, não para criar medidas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-8
Área 6 · Business Intelligence e Data Visualization I

No Power BI, para que serve uma medida?

- a) Inserir elementos como títulos no relatório.
- b) Realizar cálculos e operações matemáticas.
- c) Realizar ajustes em campos de dados.
- d) Alterar formatação visual de gráficos.

**Resposta certa:** b) Realizar cálculos e operações matemáticas.

**Explicação:** Uma medida no Power BI serve para calcular, escrevendo uma expressão DAX que faz somas, médias, contagens e razões. Esse cálculo é refeito conforme os filtros e segmentações do relatório. Títulos e formatação de gráficos são recursos visuais, e ajustar campos é papel de colunas e do Power Query.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147517-1-9
Área 6 · Business Intelligence e Data Visualization I

Sobre a prática de Data Visualization (Dataviz), é INCORRETO afirmar que:

- a) Muitas vezes, é apresentada em formato de dashboards.
- b) Tem como objetivo facilitar a interpretação dos dados por meio de representações visuais organizadas.
- c) Consiste em criar visualizações sem se preocupar com a origem ou qualidade dos dados, pois tudo é feito automaticamente.
- d) Ela é a arte de contar histórias usando dados e elementos visuais como gráficos e textos.

**Resposta certa:** c) Consiste em criar visualizações sem se preocupar com a origem ou qualidade dos dados, pois tudo é feito automaticamente.

**Explicação:** A afirmação incorreta é a que diz que dataviz dispensa a preocupação com origem e qualidade dos dados. Uma visualização só é confiável se os dados que a alimentam forem bem coletados e tratados, e nada disso é automático. As outras três descrevem corretamente o objetivo, o formato de dashboard e o lado de contar histórias.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Business Intelligence e Data Visualization II

### Questão 147942-1-1
Área 6 · Business Intelligence e Data Visualization II

No contexto do Business Intelligence e Data Visualization, qual ferramenta de visualização é especificamente utilizada para representar a frequência de palavras em textos de forma gráfica?

- a) Tabela dinâmica.
- b) Gráfico de barras.
- c) Mapa coroplético.
- d) Nuvem de palavras.

**Resposta certa:** d) Nuvem de palavras.

**Explicação:** A resposta é nuvem de palavras, que desenha cada palavra com tamanho proporcional à sua frequência no texto. Gráfico de barras e tabela dinâmica até mostram contagens, mas não são a ferramenta feita para frequência de termos, e o mapa coroplético trata de dados geográficos.

**Fonte:** Data Science do Zero, pág. 340

**Situação:** explicação conferida com o material das aulas

---

### Questão 147942-1-10
Área 6 · Business Intelligence e Data Visualization II

Considere os conceitos apresentados em aula e responda: Qual das alternativas abaixo NÃO representa uma boa prática no storytelling com dados?

- a) Escolher objetos visuais adequados.
- b) Definir uma narrativa clara.
- c) Iniciar a construção dos gráficos antes mesmo de conhecer o público-alvo.
- d) Compreender o contexto e o público-alvo.

**Resposta certa:** c) Iniciar a construção dos gráficos antes mesmo de conhecer o público-alvo.

**Explicação:** A prática que não vale é começar os gráficos antes de conhecer o público-alvo. No storytelling com dados, entender o contexto e quem vai ler vem primeiro, depois se define a narrativa e se escolhem os visuais. Montar gráficos antes disso costuma gerar um material que não responde ao que a audiência precisa.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-2
Área 6 · Business Intelligence e Data Visualization II

Sobre a utilização de KPI (Key Performance Indicator) em painéis de controle, assinale a alternativa CORRETA:

- a) KPI é um indicador que mede o desempenho de um item, processo ou objetivo específico.
- b) É um tipo de relacionamento criado automaticamente entre tabelas.
- c) Reflete exclusivamente dados financeiros.
- d) Serve apenas como rótulo descritivo nos gráficos.

**Resposta certa:** a) KPI é um indicador que mede o desempenho de um item, processo ou objetivo específico.

**Explicação:** A resposta é que KPI é um indicador que mede o desempenho de um item, processo ou objetivo específico, comparando o resultado com uma meta. Ele não se limita a dados financeiros, pode medir qualquer área, e não é um relacionamento entre tabelas nem um simples rótulo de gráfico.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-3
Área 6 · Business Intelligence e Data Visualization II

A respeito dos tipos de mapas disponíveis no Power BI para visualização de dados geográficos, é CORRETO afirmar que:

- a) Mapas são utilizados apenas no Power Query.
- b) Só é possível criar mapas com dados de latitude e longitude.
- c) Existem dois tipos principais: mapa simples e mapa coroplético.
- d) Não é possível trabalhar com dados geográficos no Power BI.

**Resposta certa:** c) Existem dois tipos principais: mapa simples e mapa coroplético.

**Explicação:** A resposta é que existem dois tipos principais, o mapa simples (com pontos ou bolhas em coordenadas ou locais) e o mapa coroplético (áreas coloridas conforme o valor). A alternativa da latitude e longitude é restritiva demais, porque o Power BI também localiza por nome de país, estado ou cidade.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-4
Área 6 · Business Intelligence e Data Visualization II

Avalie as afirmativas abaixo sobre o relacionamento entre tabelas no contexto do Business Intelligence e Data Visualization e, em seguida, assinale a alternativa CORRETA.

I. A chave primária assegura que os registros sejam únicos em uma tabela.

II. A chave estrangeira permite conectar dados, buscando informações na chave primária de outra tabela.

III. As chaves primárias podem ter valores duplicados em uma tabela.
Avalie as afirmativas abaixo sobre o relacionamento entre tabelas no contexto do Business Intelligence e Data Visualization e, em seguida, assinale a alternativa CORRETA.
I. A chave primária assegura que os registros sejam únicos em uma tabela.
II. A chave estrangeira permite conectar dados, buscando informações na chave primária de outra tabela.
III. As chaves primárias podem ter valores duplicados em uma tabela.

- a) Apenas as afirmativas I e II estão corretas.
- b) Todas estão as afirmativas estão incorretas.
- c) Apenas a afirmativa I está correta.
- d) Apenas a afirmativa II está correta.

**Resposta certa:** a) Apenas as afirmativas I e II estão corretas.

**Explicação:** A resposta é que apenas I e II estão corretas. A chave primária identifica cada registro de forma única, então não admite duplicatas, o que torna a III falsa. A chave estrangeira aponta para a chave primária de outra tabela, e é assim que o relacionamento entre elas é feito.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-5
Área 6 · Business Intelligence e Data Visualization II

No processo de construção de dashboards, qual é a função de uma coluna condicional?

- a) Retornar valores baseados em condições específicas, como “Se... então...”.
- b) Produzir mapas temáticos.
- c) Gerar relações automáticas entre tabelas.
- d) Realizar análises estatísticas.

**Resposta certa:** a) Retornar valores baseados em condições específicas, como “Se... então...”.

**Explicação:** Uma coluna condicional retorna um valor conforme uma condição, no formato se... então... senão. Por exemplo, classificar uma venda como alta ou baixa conforme o valor. Ela não cria mapas, não gera relacionamentos e não faz análise estatística.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-6
Área 6 · Business Intelligence e Data Visualization II

Ao pensar em indicadores de desempenho, qual é a definição correta de KPI no contexto de Business Intelligence e Data Visualization?

- a) Indicador chave de performance, que mede o progresso de um objetivo específico.
- b) É um tipo de relacionamento criado entre tabelas.
- c) Processo de remoção de filtros ativos no painel.
- d) Ferramenta gráfica utilizada para construção de mapas no Power BI.

**Resposta certa:** a) Indicador chave de performance, que mede o progresso de um objetivo específico.

**Explicação:** A resposta é indicador chave de performance, que acompanha o progresso de um objetivo específico, em geral contra uma meta. As demais alternativas descrevem outras coisas: relacionamento entre tabelas, limpeza de filtros e criação de mapas, que nada têm a ver com KPI.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-7
Área 6 · Business Intelligence e Data Visualization II

Considere os conceitos discutidos em aula e responda: Qual é o principal objetivo da criação de um infográfico?

- a) Servir apenas como decoração no dashboard.
- b) Substituir completamente a análise de gráficos no Power BI.
- c) Eliminar o uso de elementos visuais nos painéis.
- d) Permitir a combinação de textos, números e elementos visuais para contar uma história baseada em dados.

**Resposta certa:** d) Permitir a combinação de textos, números e elementos visuais para contar uma história baseada em dados.

**Explicação:** O infográfico combina texto, números e elementos visuais para contar uma história com base em dados, e esse é o objetivo principal. Ele complementa os gráficos do painel em vez de substituí-los, e por isso decoração pura ou eliminar elementos visuais não fazem sentido.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-8
Área 6 · Business Intelligence e Data Visualization II

No contexto de projetos de análise de dados, o que significa o conceito de privacidade de dados?

- a) Significa somente atribuir senhas aos arquivos do Power BI.
- b) Significa garantir a segurança, sigilo, integridade e confidencialidade dos dados utilizados.
- c) Significa ocultar os nomes das tabelas.
- d) Significa Impedir que os gráficos sejam visualizados publicamente.

**Resposta certa:** b) Significa garantir a segurança, sigilo, integridade e confidencialidade dos dados utilizados.

**Explicação:** Privacidade de dados é garantir segurança, sigilo, integridade e confidencialidade das informações usadas no projeto. Pôr senha em arquivo ou esconder nomes de tabelas são medidas pontuais, e restringir a exibição pública de gráficos é só uma parte do problema.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 147942-1-9
Área 6 · Business Intelligence e Data Visualization II

No Power BI, qual recurso permite realizar cálculos, como somas, médias e contagens, dinamicamente?

- a) Relacionamento.
- b) DAX (Data Analysis Expressions).
- c) Power Query.
- d) Chave Primária.

**Resposta certa:** b) DAX (Data Analysis Expressions).

**Explicação:** A resposta é DAX (Data Analysis Expressions), a linguagem de fórmulas do Power BI que calcula somas, médias e contagens de forma dinâmica, respondendo aos filtros do relatório. O Power Query prepara e transforma os dados antes de carregá-los, e relacionamento e chave primária ligam tabelas sem calcular nada.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Business Intelligence e Data Visualization III

### Questão 148239-1-1
Área 6 · Business Intelligence e Data Visualization III

Dentre as alternativas abaixo, assinale a que representa um dos papéis principais da ANPD (Agência Nacional de Proteção de Dados).

- a) Zelar pela proteção de dados, fiscalizar e conscientizar sobre a LGPD.
- b) Aprovar o desenvolvimento de relatórios analíticos.
- c) Gerar dashboards para empresas públicas.
- d) Controlar exclusivamente os dados financeiros das empresas.

**Resposta certa:** a) Zelar pela proteção de dados, fiscalizar e conscientizar sobre a LGPD.

**Explicação:** A resposta é zelar pela proteção de dados, fiscalizar e conscientizar sobre a LGPD, que são as funções centrais da ANPD. Ela não aprova relatórios analíticos nem gera dashboards, e sua atuação não se limita aos dados financeiros das empresas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-10
Área 6 · Business Intelligence e Data Visualization III

Diante de ameaças como cyber attacks, shadow IT e fraudes, qual é a principal missão da governança e da gestão de dados?

- a) Maximizar o compartilhamento de dados não estruturados.
- b) Limitar o acesso aos dashboards de marketing.
- c) Disponibilizar os dados livremente.
- d) Proteger, garantindo confidencialidade, integridade e segurança das informações.

**Resposta certa:** d) Proteger, garantindo confidencialidade, integridade e segurança das informações.

**Explicação:** Diante de ameaças como ataques, shadow IT e fraudes, a missão da governança e da gestão de dados é proteger as informações, garantindo confidencialidade, integridade e segurança. Liberar ou compartilhar dados sem controle iria no sentido contrário.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-2
Área 6 · Business Intelligence e Data Visualization III

Em relação às boas práticas para garantir a privacidade de dados, qual das opções a seguir não é recomendada?

- a) Utilizar senhas fortes.
- b) Conectar-se a redes Wi-Fi públicas sem restrição.
- c) Proteger informações com contratos de sigilo (NDA).
- d) Ter cautela no armazenamento de documentos do cliente.

**Resposta certa:** b) Conectar-se a redes Wi-Fi públicas sem restrição.

**Explicação:** A prática não recomendada é conectar-se a redes Wi-Fi públicas sem restrição, porque nelas o tráfego pode ser interceptado por terceiros. Senhas fortes, NDA e cuidado no armazenamento de documentos de clientes são medidas que ajudam a proteger a privacidade.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-3
Área 6 · Business Intelligence e Data Visualization III

No contexto de Cultura Data Driven, assinale a alternativa CORRETA:

- a) É a cultura organizacional onde as decisões são tomadas com base em intuição.
- b) É quando a organização prioriza o uso de dados e análises na tomada de decisões.
- c) Refere-se ao uso de dados apenas na área de tecnologia.
- d) É um conceito aplicado apenas em startups.

**Resposta certa:** b) É quando a organização prioriza o uso de dados e análises na tomada de decisões.

**Explicação:** Cultura data driven é aquela em que a organização prioriza dados e análises nas decisões, em vez de depender de intuição. Ela não se restringe à área de tecnologia nem a startups, pois vale para qualquer setor e porte de empresa.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-4
Área 6 · Business Intelligence e Data Visualization III

Dentro dos pilares da Governança de Dados, o item que responde à pergunta “como?” é:

- a) Dados.
- b) Tecnologia.
- c) Processos.
- d) Pessoas.

**Resposta certa:** c) Processos.

**Explicação:** Nos pilares da governança de dados, processos respondem ao como, ou seja, as regras e fluxos que definem a forma de tratar o dado. Pessoas respondem ao quem, tecnologia entra com as ferramentas e os dados são o objeto da governança.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-5
Área 6 · Business Intelligence e Data Visualization III

Na Governança de Dados, qual elemento está relacionado aos responsáveis pela execução das atividades, ou seja, 'quem faz'?

- a) Tecnologia.
- b) Processos.
- c) Pessoas.
- d) Documentos.

**Resposta certa:** c) Pessoas.

**Explicação:** Pessoas respondem ao quem faz na governança de dados: são os responsáveis, como gestores de dados, stewards e donos, que executam as atividades. Processos dizem como fazer e tecnologia fornece as ferramentas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-6
Área 6 · Business Intelligence e Data Visualization III

O papel da tecnologia na Governança de Dados é:

- a) Definir os responsáveis pela proteção dos dados.
- b) Determinar as políticas de RH.
- c) Controlar exclusivamente o acesso físico ao escritório.
- d) Oferecer ferramentas que suportam a gestão da informação e sua segurança.

**Resposta certa:** d) Oferecer ferramentas que suportam a gestão da informação e sua segurança.

**Explicação:** A tecnologia na governança de dados oferece as ferramentas que apoiam a gestão da informação e a sua segurança, como catálogos, controle de acesso e criptografia. Definir responsáveis é papel de pessoas e processos, e as políticas de RH e o acesso físico estão fora do escopo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-7
Área 6 · Business Intelligence e Data Visualization III

A sigla NDA (Non-Disclosure Agreement) significa:

- a) Contrato de confidencialidade, que protege informações sensíveis entre as partes envolvidas.
- b) Documento que permite o livre compartilhamento de dados.
- c) Termo técnico utilizado na criação de dashboards.
- d) Contrato exclusivo para uso em redes sociais.

**Resposta certa:** a) Contrato de confidencialidade, que protege informações sensíveis entre as partes envolvidas.

**Explicação:** NDA, ou Non-Disclosure Agreement, é um contrato de confidencialidade que protege informações sensíveis trocadas entre as partes. Ele restringe a divulgação, ao contrário de liberar o compartilhamento, e não é termo de dashboards nem de redes sociais.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-8
Área 6 · Business Intelligence e Data Visualization III

Entre as opções a seguir, qual representa um risco à segurança da informação dentro das empresas?

- a) Uso de softwares licenciados.
- b) Shadow IT — uso de sistemas e ferramentas sem o conhecimento do setor de TI.
- c) Criptografia de dados.
- d) Autenticação em dois fatores.

**Resposta certa:** b) Shadow IT — uso de sistemas e ferramentas sem o conhecimento do setor de TI.

**Explicação:** Shadow IT é o uso de sistemas e ferramentas sem o conhecimento do setor de TI, e por isso é um risco: esses recursos escapam de políticas de segurança, de backup e de controle de acesso. Software licenciado, criptografia e autenticação em dois fatores são medidas de proteção.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148239-1-9
Área 6 · Business Intelligence e Data Visualization III

Assinale a alternativa que representa um dos objetivos centrais da LGPD (Lei Geral de Proteção de Dados).

- a) Proteger os dados pessoais de cidadãos, assegurando direitos de privacidade e segurança.
- b) Liberar o compartilhamento irrestrito de dados.
- c) Regular o uso de dashboards em empresas públicas.
- d) Controlar os acessos à internet dentro da empresa.

**Resposta certa:** a) Proteger os dados pessoais de cidadãos, assegurando direitos de privacidade e segurança.

**Explicação:** Um dos objetivos centrais da LGPD é proteger os dados pessoais dos cidadãos, assegurando direitos de privacidade e segurança. A lei regula o tratamento desses dados e não libera o compartilhamento irrestrito, nem trata de dashboards ou de acesso à internet na empresa.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Cloud Computing I

### Questão 152972-1-1
Área 6 · Cloud Computing I

Qual é o objetivo principal da prática de FinOps (Cloud Cost Management) no contexto da computação em nuvem?

- a) Transferir toda a responsabilidade dos custos da engenharia para a equipe de finanças.
- b) Proibir que os engenheiros criem novos recursos para evitar custos.
- c) Gastar o mínimo possível na nuvem, mesmo que isso prejudique o desempenho.
- d) Trazer responsabilidade financeira para os gastos em nuvem, unindo equipes para tomar decisões inteligentes sobre custos.

**Resposta certa:** d) Trazer responsabilidade financeira para os gastos em nuvem, unindo equipes para tomar decisões inteligentes sobre custos.

**Explicação:** O FinOps traz responsabilidade financeira para o gasto variável da nuvem e une engenharia, finanças e negócios para decidir bem sobre custos. O objetivo não é gastar o mínimo, e sim gastar melhor, por isso cortar desempenho ou proibir recursos novos está errado.

**Fonte:** Aula de Cloud Computing I, pág. 67

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-10
Área 6 · Cloud Computing I

O que é Entrega Contínua no contexto de CI/CD da computação em nuvem?

- a) Prática de engenharia de software na qual as equipes, de desenvolvimento de software, produzem um entregável em ciclos curtos
- b) Processo no desenvolvimento de software onde o código de um desenvolvedor é analisado por outros membros da equipe
- c) Espaço para desenvolvedores armazenarem, gerenciarem e compartilharem seu código, bem como rastrear alterações e colaborarem em projetos
- d) Prática de mesclar todas as cópias de trabalho dos desenvolvedores em uma linha principal compartilhada, várias vezes ao dia

**Resposta certa:** a) Prática de engenharia de software na qual as equipes, de desenvolvimento de software, produzem um entregável em ciclos curtos

**Explicação:** Entrega contínua (CD) é a prática em que equipes de desenvolvimento produzem um entregável em ciclos curtos, de modo que o software possa ser lançado com segurança a qualquer momento. A alternativa sobre mesclar cópias de trabalho várias vezes ao dia descreve a integração contínua (CI), e a de revisão de código descreve o code review.

**Fonte:** Aula de Cloud Computing I, pág. 54

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-2
Área 6 · Cloud Computing I

Considere os conceitos discutidos em aula e responda: Qual das alternativas abaixo representa uma das desvantagens da arquitetura Serverless?

- a) Um custo sempre menor, pois os recursos estão sempre ativos esperando uma requisição.
- b) A latência (o tempo que os dados levam para ir e voltar) é uma desvantagem em aplicações de alta frequência.
- c) Uma complexidade maior que impossibilita o gerenciamento de atualizações do sistema operacional.
- d) A impossibilidade de escalar para lidar com picos de tráfego.

**Resposta certa:** b) A latência (o tempo que os dados levam para ir e voltar) é uma desvantagem em aplicações de alta frequência.

**Explicação:** A latência é uma desvantagem, principalmente em aplicações de alta frequência, que precisam de respostas em microssegundos. No serverless isso aparece também nos cold starts, o atraso da primeira execução de uma função parada. As outras alternativas contradizem as vantagens do modelo: cobra só pelo uso, escala sozinho e a plataforma cuida do sistema operacional.

**Fonte:** Aula de Cloud Computing I, pág. 18 e 40

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-3
Área 6 · Cloud Computing I

Considere os conceitos discutidos em aula e assinale a alternativa que apresenta uma das vantagens da implementação de Nuvem Híbrida:

- a) Eliminação completa da infraestrutura local.
- b) Segurança absoluta dos dados.
- c) Flexibilidade.
- d) Redução total dos custos operacionais.

**Resposta certa:** c) Flexibilidade.

**Explicação:** Flexibilidade é a vantagem da nuvem híbrida: dados sensíveis ficam na infraestrutura local e a nuvem pública entra para escalar o processamento ou para recuperação de desastres. As demais são exageradas, já que a híbrida não elimina a infraestrutura local nem garante segurança absoluta ou custo zero.

**Fonte:** Aula de Cloud Computing I, pág. 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-4
Área 6 · Cloud Computing I

No contexto da computação em nuvem, qual das seguintes estratégias de otimização de custos envolve a identificação e exclusão de recursos ociosos, como discos não atachados?

- a) Agendamento (Ligar/Desligar).
- b) Caça aos 'Recursos Zumbis'.
- c) Rightsizing (Dimensionamento Correto).
- d) Uso de Tags (Etiquetas).

**Resposta certa:** b) Caça aos 'Recursos Zumbis'.

**Explicação:** A resposta é a caça aos recursos zumbis, que consiste em achar e apagar discos não atachados a nenhuma VM, IPs elásticos sem uso e snapshots antigos. Rightsizing reduz o tamanho de máquinas superdimensionadas, agendamento liga e desliga recursos, e tags servem para atribuir custos.

**Fonte:** Aula de Cloud Computing I, pág. 69

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-5
Área 6 · Cloud Computing I

Assinale a alternativa que apresenta uma das principais vantagens de um Gerenciamento de Identidade e Acesso (IAM) robusto no contexto da computação em nuvem.

- a) Reduz drasticamente a superfície de ataque. Se uma conta for comprometida, o dano é limitado pelo princípio do menor privilégio.
- b) Dar as mesmas permissões a todos os usuários para simplificar o gerenciamento.
- c) Conceder acesso de administrador a todos os usuários para garantir que eles possam fazer seu trabalho.
- d) Remover todas as permissões e exigi-las caso a caso por meio de tickets de suporte.

**Resposta certa:** a) Reduz drasticamente a superfície de ataque. Se uma conta for comprometida, o dano é limitado pelo princípio do menor privilégio.

**Explicação:** Um IAM robusto reduz drasticamente a superfície de ataque, porque pelo princípio do menor privilégio uma conta comprometida só causa dano limitado. Dar as mesmas permissões ou acesso de administrador a todos faz o oposto, e exigir tudo por ticket não é prática de IAM.

**Fonte:** Aula de Cloud Computing I, pág. 62 e 64

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-6
Área 6 · Cloud Computing I

Qual dos seguintes é um exemplo de um serviço de SaaS (Software como Serviço)?

- a) Google App Engine (Plataforma de Aplicações).
- b) Amazon EC2 (Máquinas Virtuais).
- c) Kubernetes.
- d) Microsoft Office 365.

**Resposta certa:** d) Microsoft Office 365.

**Explicação:** Microsoft Office 365 é SaaS, um software pronto que se usa pela internet sem gerenciar infraestrutura. Google App Engine é PaaS, Amazon EC2 é IaaS (máquinas virtuais) e Kubernetes é uma plataforma de orquestração de contêineres, não um software final.

**Fonte:** Aula de Cloud Computing I, pág. 25

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-7
Área 6 · Cloud Computing I

Qual dos modelos de implantação de nuvem oferece o máximo de controle, segurança e privacidade, sendo ideal para bancos e governos?

- a) Nuvem Privada.
- b) Multi-Cloud.
- c) Nuvem Pública.
- d) Nuvem Híbrida.

**Resposta certa:** a) Nuvem Privada.

**Explicação:** A nuvem privada tem infraestrutura de uso exclusivo de uma organização, o que dá o máximo de controle, segurança e privacidade, e por isso é ideal para bancos e governos. A híbrida combina a privada com a pública e tem a flexibilidade como vantagem principal.

**Fonte:** Aula de Cloud Computing I, pág. 30 e 31

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-8
Área 6 · Cloud Computing I

Em bancos de dados, qual característica define um sistema SQL (Relacional)?

- a) Uso de documentos JSON para armazenar dados.
- b) Otimização para escalabilidade horizontal massiva em clusters de máquinas baratas.
- c) Schema flexível, onde cada registro pode ter uma estrutura diferente.
- d) Estrutura rígida e predefinida (schema fixo), com dados organizados em tabelas, linhas e colunas.

**Resposta certa:** d) Estrutura rígida e predefinida (schema fixo), com dados organizados em tabelas, linhas e colunas.

**Explicação:** Um sistema SQL relacional tem estrutura rígida e predefinida, o schema fixo, com dados em tabelas, linhas e colunas. As outras alternativas descrevem o NoSQL: documentos JSON, schema flexível e escalabilidade horizontal em clusters de máquinas baratas.

**Fonte:** Aula de Cloud Computing I, pág. 42 e 44

**Situação:** explicação conferida com o material das aulas

---

### Questão 152972-1-9
Área 6 · Cloud Computing I

Qual é a principal ideia por trás da computação 'Serverless' (sem servidor)?

- a) Reduzir a segurança ao remover as camadas de gerenciamento do servidor.
- b) Eliminar completamente o uso de servidores na computação.
- c) Permitir que os desenvolvedores executem código sem gerenciar a infraestrutura subjacente.
- d) Forçar o uso de um único servidor físico massivo para todas as tarefas.

**Resposta certa:** c) Permitir que os desenvolvedores executem código sem gerenciar a infraestrutura subjacente.

**Explicação:** A ideia do serverless é permitir que o desenvolvedor execute código sem gerenciar a infraestrutura. Os servidores continuam existindo, mas o provedor cuida deles por completo, e a plataforma só aloca recursos quando a função é acionada. Por isso dizer que elimina servidores está errado.

**Fonte:** Aula de Cloud Computing I, pág. 37

**Situação:** explicação conferida com o material das aulas

---

## Cloud Computing II

### Questão 153477-1-1
Área 6 · Cloud Computing II

Com relação a Análise Preditiva de dados, assinale a alternativa INCORRETA:

- a) Seu objetivo é identificar os fatores e as razões por trás de um determinado evento ou tendência. Para isso, a análise preditiva utiliza métodos de correlação e análise de causa raiz.
- b) Possui objetivo de antecipar tendências, oportunidades ou riscos futuros.
- c) Dentre os métodos utilizados na análise preditiva estão: modelagem estatística, e aprendizado de máquina.
- d) Um exemplo de uso da análise preditiva é: usar dados de vendas anteriores e tendências de mercado para prever a demanda de um produto na próxima temporada de festas de fim de ano.

**Resposta certa:** a) Seu objetivo é identificar os fatores e as razões por trás de um determinado evento ou tendência. Para isso, a análise preditiva utiliza métodos de correlação e análise de causa raiz.

**Explicação:** A alternativa incorreta é a primeira, pois descreve a análise de diagnóstico (por que aconteceu, com correlações e causa raiz). A preditiva busca antecipar tendências, oportunidades ou riscos futuros com modelagem estatística e machine learning, como prever a demanda de fim de ano.

**Fonte:** Aula de Cloud Computing II, pág. 8 e 9

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-10
Área 6 · Cloud Computing II

Durante a aula, foi introduzido o Apache Kafka. Avalie as alternativas abaixo e assinale a CORRETA sobre o Kafka.

- a) Kafka é uma ferramenta de orquestração de containers que automatiza o deployment e scaling de aplicações em ambientes Kubernetes.
- b) Kafka é uma plataforma de streaming distribuída que permite publicar, assinar, armazenar e processar fluxos de registros em tempo real.
- c) Kafka é um framework de machine learning que facilita o treinamento de modelos de deep learning em clusters distribuídos com GPU.
- d) Kafka é um banco de dados NoSQL orientado a documentos que oferece consultas SQL complexas e transações ACID em ambientes distribuídos.

**Resposta certa:** b) Kafka é uma plataforma de streaming distribuída que permite publicar, assinar, armazenar e processar fluxos de registros em tempo real.

**Explicação:** A resposta é a que define o Kafka como plataforma de streaming distribuída para publicar, assinar, armazenar e processar fluxos de registros em tempo real. Ele nasceu no LinkedIn e hoje é projeto da Apache. As demais descrevem outras coisas: Kubernetes (orquestração de containers), frameworks de deep learning e bancos NoSQL de documentos.

**Fonte:** Aula de Cloud Computing (Introdução ao Apache Kafka), pág. 28

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-2
Área 6 · Cloud Computing II

Assinale a alternativa que apresenta os quatro tipos de análises de dados discutidas em aula.

- a) Análise exploratória, análise confirmatória, análise estatística e análise temporal.
- b) Análise estruturada, análise não-estruturada, análise semiestruturada e análise híbrida.
- c) Análise batch, análise streaming, análise distribuída e análise paralela.
- d) Análise descritiva, análise de diagnóstico, análise preditiva e análise prescritiva.

**Resposta certa:** d) Análise descritiva, análise de diagnóstico, análise preditiva e análise prescritiva.

**Explicação:** Os quatro tipos de análise vistos em aula são descritiva (o que aconteceu), diagnóstica (por que aconteceu), preditiva (o que vai acontecer) e prescritiva (o que devemos fazer). As outras opções misturam classificações de dados ou de processamento que não são esses tipos.

**Fonte:** Aula de Cloud Computing II, pág. 6

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-3
Área 6 · Cloud Computing II

Durante a aula foi discutido o ciclo de vida de um projeto de análise de dados baseado na metodologia CRISP-DM. Assinale a alternativa INCORRETA sobre a etapa de visualização e apresentação dos dados.

- a) A etapa de visualização e apresentação dos dados deve ser capaz de comunicar os resultados.
- b) A etapa de visualização e apresentação dos dados é a última do ciclo de vida de um projeto de análise de dados baseado na metodologia CRISP-DM apresentada em aula.
- c) Na etapa de visualização e apresentação dos dados, é importante que os resultados sejam capazes de gerar recomendações para a audiência.
- d) O método de apresentação dos insights obtidos deve ser sempre via dashboad no Power BI, independente da audiência.

**Resposta certa:** d) O método de apresentação dos insights obtidos deve ser sempre via dashboad no Power BI, independente da audiência.

**Explicação:** A alternativa incorreta é a que impõe o dashboard no Power BI como método único, independente da audiência. A apresentação deve ser adaptada ao público e aos objetivos, e o importante é comunicar os resultados e gerar recomendações. As demais afirmações descrevem corretamente essa etapa final do ciclo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 153477-1-4
Área 6 · Cloud Computing II

Qual é a ideia central do conceito de Dados como um produto (Data as a product – DaaP)?

- a) Tratar os dados como um produto acabado, não como um subproduto bruto.
- b) Transformar todos os dados da empresa em produtos comercializáveis para venda externa e geração de receita adicional.
- c) Aplicar metodologias ágeis exclusivamente no desenvolvimento de pipelines de dados para acelerar a entrega de relatórios.
- d) Centralizar todos os dados em uma única plataforma de nuvem para garantir consistência e reduzir custos de armazenamento.

**Resposta certa:** a) Tratar os dados como um produto acabado, não como um subproduto bruto.

**Explicação:** Na ideia de dados como produto (DaaP), os dados são tratados como produto acabado, um ativo essencial voltado ao valor para o consumidor, e não como subproduto bruto. A qualidade passa a ser característica principal e a propriedade é clara e de longo prazo. Não implica vender todos os dados.

**Fonte:** Aula de Cloud Computing II, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-5
Área 6 · Cloud Computing II

Durante a aula, foi introduzido o Apache Kafka. Assinale a alternativa que apresenta um caso de uso comum do Apache Kafka.

- a) Criação de aplicativos que consomem, processam e analisam fluxos de dados em tempo real.
- b) Renderização de imagens e vídeos de alta resolução para uso em aplicações gráficas.
- c) Edição colaborativa de documentos de texto em tempo real por múltiplos usuários.
- d) Armazenamento permanente de grandes volumes de dados em um banco de dados relacional.

**Resposta certa:** a) Criação de aplicativos que consomem, processam e analisam fluxos de dados em tempo real.

**Explicação:** Um caso de uso comum do Kafka é o processamento de fluxo: criar aplicativos que consomem, processam e analisam fluxos de dados em tempo real. Ele é uma plataforma de streaming de eventos, e não serve para renderizar vídeo, editar documentos nem como banco relacional.

**Fonte:** Aula de Cloud Computing II, pág. 29

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-6
Área 6 · Cloud Computing II

Durante a aula, foram discutidos dois métodos para coleta de informações: o streaming de eventos e a fila de mensagens. Assinale a alternativa que apresenta as principais características da Plataforma de streaming de eventos.

- a) Garante que uma tarefa seja sempre executada uma única vez.
- b) Não suporta um modelo de publicação-assinatura, no qual vários aplicativos podem consumir o mesmo fluxo de dados.
- c) Remove mensagens quando elas são consumidas por um único destinatário.
- d) Alto rendimento, baixa latência, dados frequentemente imutáveis e reproduzíveis.

**Resposta certa:** d) Alto rendimento, baixa latência, dados frequentemente imutáveis e reproduzíveis.

**Explicação:** A plataforma de streaming de eventos tem alto rendimento, baixa latência e dados frequentemente imutáveis e reproduzíveis, além de suportar publicação-assinatura com vários consumidores. As outras três alternativas descrevem a fila de mensagens, que remove a mensagem ao ser consumida e garante execução única da tarefa.

**Fonte:** Aula de Cloud Computing II, pág. 20

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-7
Área 6 · Cloud Computing II

Durante a aula foi discutido o ciclo de vida de um projeto de análise de dados baseado na metodologia CRISP-DM. Quais são os três primeiros passos desse ciclo de vida?

- a) Business Issue Understanding, Data Understanding e Data Preparation.
- b) Requirements Gathering, Data Analysis e Results Validation.
- c) Data Collection, Data Cleaning e Data Modeling.
- d) Problem Definition, Algorithm Selection e Model Training.

**Resposta certa:** a) Business Issue Understanding, Data Understanding e Data Preparation.

**Explicação:** A resposta é Business Issue Understanding, Data Understanding e Data Preparation, porque o CRISP-DM começa entendendo o problema de negócio, depois conhece os dados disponíveis e só então os prepara. Só depois dessas três fases vêm modelagem, avaliação e implantação. As outras alternativas misturam nomes de etapas genéricas que não são as fases do CRISP-DM.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 153477-1-8
Área 6 · Cloud Computing II

Quando aplicado pelas empresas, o conceito de Dados como um produto (Data as a Product – DaaP) pode trazer uma série de benefícios. Assinale a alternativa que apresenta um desses benefícios:

- a) Eliminar completamente a necessidade de profissionais especializados em dados e analytics.
- b) Garantir que todos os dados da empresa sejam automaticamente públicos e acessíveis externamente.
- c) Reduzir a zero os custos de infraestrutura de armazenamento e processamento de dados.
- d) Desbloquear novos fluxos de receita.

**Resposta certa:** d) Desbloquear novos fluxos de receita.

**Explicação:** A resposta é desbloquear novos fluxos de receita, porque ao tratar dados como produto a empresa pode criar produtos e serviços em cima deles ou vender os dados a terceiros. Os outros itens são exageros: o DaaP não elimina especialistas, não torna tudo público e não zera custo de infraestrutura, no máximo reduz retrabalho e pipelines redundantes.

**Fonte:** Aula de Cloud Computing (Dados como produto), pág. 14

**Situação:** explicação conferida com o material das aulas

---

### Questão 153477-1-9
Área 6 · Cloud Computing II

Durante a aula, foram discutidos dois métodos para coleta de informações: o streaming de eventos e a fila de mensagens. Assinale a alternativa que apresenta o foco principal da Plataforma de streaming de eventos.

- a) Processamento em tempo real de fluxos de dados contínuos.
- b) Garantir que uma tarefa seja sempre executada uma única vez.
- c) Remover mensagens quando elas são consumidas por um único destinatário.
- d) Entregar mensagens entre aplicativos.

**Resposta certa:** a) Processamento em tempo real de fluxos de dados contínuos.

**Explicação:** A resposta é processamento em tempo real de fluxos de dados contínuos, que é o foco da plataforma de streaming de eventos. As outras três alternativas descrevem a fila de mensagens: entrega entre aplicativos, remoção da mensagem quando um único destinatário a consome e execução de cada tarefa uma só vez.

**Fonte:** Aula de Cloud Computing (streaming vs. fila de mensagens), pág. 20

**Situação:** explicação conferida com o material das aulas

---

## Engenharia de dados I

### Questão 148632-1-1
Área 6 · Engenharia de dados I

Qual das alternativas a seguir representa a principal linguagem usada para manipular bancos de dados relacionais?

- a) HTML
- b) Java
- c) C++
- d) SQL

**Resposta certa:** d) SQL

**Explicação:** A resposta é SQL (Structured Query Language), linguagem declarativa usada para consultar e manipular dados em bancos relacionais como Oracle, MySQL e SQL Server. HTML serve para páginas web, e Java e C++ são linguagens de programação gerais.

**Fonte:** Data Science do Zero, pág. 389

**Situação:** explicação conferida com o material das aulas

---

### Questão 148632-1-10
Área 6 · Engenharia de dados I

Analise as afirmações sobre engenharia de dados e assinale a alternativa que apresenta a classificação CORRETA em Verdadeiro (V) ou Falso (F):

( ) A função do engenheiro de dados termina após a coleta dos dados.

( ) A preparação dos dados envolve limpeza, transformação e integração de dados.

( ) O trabalho do engenheiro de dados ajuda a reduzir o tempo gasto pelos cientistas de dados na preparação dos dados.
Analise as afirmações sobre engenharia de dados e assinale a alternativa que apresenta a classificação CORRETA em Verdadeiro (V) ou Falso (F):
( ) A função do engenheiro de dados termina após a coleta dos dados.
( ) A preparação dos dados envolve limpeza, transformação e integração de dados.
( ) O trabalho do engenheiro de dados ajuda a reduzir o tempo gasto pelos cientistas de dados na preparação dos dados.

- a) V, V, F
- b) F, V, V
- c) F, F, V
- d) V, F, V

**Resposta certa:** b) F, V, V

**Explicação:** A resposta é F, V, V. A primeira é falsa porque o trabalho do engenheiro de dados vai além da coleta e inclui transformar, armazenar e manter os pipelines. A segunda é verdadeira, pois preparar dados envolve limpeza, transformação e integração. A terceira também, porque dados já preparados poupam tempo do cientista.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148632-1-2
Área 6 · Engenharia de dados I

No processo de ETL (Extração, Transformação e Carregamento), a etapa de 'Transformação' refere-se a:

- a) Carregar os dados no destino final.
- b) Consultar dados diretamente no banco relacional.
- c) Corrigir, limpar e preparar os dados para uso.
- d) Criar dashboards e visualizar resultados.

**Resposta certa:** c) Corrigir, limpar e preparar os dados para uso.

**Explicação:** A resposta é corrigir, limpar e preparar os dados para uso. No ETL a extração busca os dados nas fontes, a transformação os limpa, padroniza e integra, e o carregamento os grava no destino. Carregar é a terceira etapa, e consultar ou criar dashboards vem depois do ETL.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148632-1-3
Área 6 · Engenharia de dados I

O que são bancos de dados relacionais?

- a) São sistemas de armazenamento de dados que utilizam exclusivamente estruturas hierárquicas para organizar as informações.
- b) São modelos de dados que funcionam apenas com objetos gráficos, sem suporte a operações lógicas ou relacionais.
- c) São sistemas de armazenamento de dados onde as informações ficam organizadas em tabelas (linhas e colunas) que se relacionam entre si.
- d) São bancos de dados que armazenam os dados em arquivos de texto simples, sem estrutura definida e sem possibilidade de relacionamentos.

**Resposta certa:** c) São sistemas de armazenamento de dados onde as informações ficam organizadas em tabelas (linhas e colunas) que se relacionam entre si.

**Explicação:** A resposta é que bancos relacionais guardam as informações em tabelas, com linhas e colunas, que se relacionam entre si por chaves. Isso permite juntar tabelas com JOIN. Os bancos NoSQL é que fogem desse modelo e não representam dados em tabelas.

**Fonte:** Data Science do Zero, pág. 406

**Situação:** explicação conferida com o material das aulas

---

### Questão 148632-1-4
Área 6 · Engenharia de dados I

Qual das opções abaixo NÃO é uma responsabilidade típica do engenheiro de dados?

- a) Criar e gerenciar pipelines de dados.
- b) Automatizar processos de coleta e transformação de dados.
- c) Desenvolver aplicativos de software.
- d) Garantir a qualidade e consistência dos dados.

**Resposta certa:** c) Desenvolver aplicativos de software.

**Explicação:** A resposta é desenvolver aplicativos de software. O engenheiro de dados cuida dos pipelines, da automação da coleta e transformação e da qualidade e consistência dos dados. Construir aplicações é trabalho típico de desenvolvimento de software.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148632-1-5
Área 6 · Engenharia de dados I

Qual das alternativas abaixo é uma característica de um banco de dados relacional?

- a) Armazenamento em formato não estruturado.
- b) Armazenamento apenas de imagens e vídeos.
- c) Suporte exclusivo para dados em nuvem.
- d) Armazenamento de dados em tabelas com linhas e colunas.

**Resposta certa:** d) Armazenamento de dados em tabelas com linhas e colunas.

**Explicação:** A resposta é armazenar dados em tabelas com linhas e colunas. Essa é a característica central do modelo relacional. Os bancos NoSQL guardam documentos, pares chave-valor e outras estruturas fora de tabelas, e o modelo relacional não se limita a imagens ou à nuvem.

**Fonte:** Data Science do Zero, pág. 406

**Situação:** explicação conferida com o material das aulas

---

### Questão 148632-1-6
Área 6 · Engenharia de dados I

Você precisa extrair todos os registros da tabela 'clientes' para análise. Considerando boas práticas de SQL, qual comando você utilizaria?

- a) SELECT * FROM clientes;
- b) SELECT ALL FROM clientes;
- c) SHOW * FROM clientes;
- d) GET * FROM clientes;

**Resposta certa:** a) SELECT * FROM clientes;

**Explicação:** A resposta é SELECT * FROM clientes;, em que o asterisco traz todas as colunas e, sem WHERE, todas as linhas da tabela. SELECT ALL, SHOW e GET não são a sintaxe padrão para consultar registros em SQL.

**Fonte:** Data Science do Zero, pág. 394

**Situação:** explicação conferida com o material das aulas

---

### Questão 148632-1-7
Área 6 · Engenharia de dados I

O ciclo de vida dos dados no processo de Engenharia de Dados inclui as etapas:

- a) Extração, Transformação e Carregamento (ETL).
- b) Armazenamento, Modelagem e Predição.
- c) Coleta, Análise e Relatório.
- d) Visualização, Análise e Carga.

**Resposta certa:** a) Extração, Transformação e Carregamento (ETL).

**Explicação:** A resposta é extração, transformação e carregamento (ETL), o fluxo clássico em que os dados saem das fontes, são tratados e vão para o destino. As outras opções misturam etapas de análise e de ciência de dados, como predição, relatório e visualização, que vêm depois do trabalho da engenharia de dados.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 148632-1-8
Área 6 · Engenharia de dados I

Qual das alternativas abaixo representa um comando SQL que remove um registro específico de uma tabela?

- a) DELETE
- b) UPDATE
- c) CREATE
- d) INSERT

**Resposta certa:** a) DELETE

**Explicação:** A resposta é DELETE, que apaga linhas de uma tabela. Com uma cláusula WHERE remove só o registro desejado, por exemplo DELETE FROM users WHERE user_id = 1, e sem WHERE apaga todas as linhas. UPDATE altera valores, INSERT inclui linhas e CREATE cria objetos.

**Fonte:** Data Science do Zero, pág. 393

**Situação:** explicação conferida com o material das aulas

---

### Questão 148632-1-9
Área 6 · Engenharia de dados I

Qual das alternativas abaixo representa o principal objetivo do engenheiro de dados?

- a) Preparar, organizar e estruturar dados para uso posterior.
- b) Analisar dados estatísticos e gerar insights.
- c) Desenvolver APIs para front-end.
- d) Criar modelos de machine learning.

**Resposta certa:** a) Preparar, organizar e estruturar dados para uso posterior.

**Explicação:** A resposta é preparar, organizar e estruturar dados para uso posterior. O engenheiro de dados deixa os dados disponíveis e confiáveis para analistas e cientistas. Gerar insights é do analista, e criar modelos de machine learning é do cientista de dados.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Engenharia de dados II

### Questão 149365-1-1
Área 6 · Engenharia de dados II

Considerando as tabelas livros e autores criadas em aula, qual comando SQL retorna todos os livros juntamente com os nomes de seus respectivos autores?

- a) SELECT livro.nome, autor.nome FROM autores, livros;
- b) SELECT livros.nome, autores.nome WHERE autor_id = id;
- c) SELECT l.nome AS livro, a.nome AS autor FROM livros l JOIN autores a ON l.autor_id = a.id;
- d) SELECT nome FROM livros JOIN autores;

**Resposta certa:** c) SELECT l.nome AS livro, a.nome AS autor FROM livros l JOIN autores a ON l.autor_id = a.id;

**Explicação:** A resposta é a que usa JOIN com a condição ON l.autor_id = a.id, ligando cada livro ao seu autor pela chave estrangeira. A primeira alternativa faz produto cartesiano, sem condição de ligação, e ainda usa nomes de tabela errados. A segunda não tem FROM e a quarta não indica a coluna de ligação nem qual nome mostrar.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-10
Área 6 · Engenharia de dados II

Considere os conceitos relacionados à Engenharia de Dados e assinale a alternativa que apresenta um exemplo de entidade associativa.

- a) Uma tabela de estoque que registra a quantidade disponível de cada produto, sem vínculo com clientes ou vendas.
- b) Uma tabela vendas que liga clientes e produtos e armazena informações como data e quantidade.
- c) Uma tabela que armazena apenas os nomes dos clientes sem qualquer relação com outras tabelas.
- d) Uma tabela de categorias de produtos que apenas classifica os itens por tipo, sem se relacionar com outras entidades.

**Resposta certa:** b) Uma tabela vendas que liga clientes e produtos e armazena informações como data e quantidade.

**Explicação:** A resposta é a tabela vendas, porque ela liga clientes e produtos e ainda carrega atributos próprios do relacionamento (data e quantidade). É isso que define uma entidade associativa: um relacionamento muitos-para-muitos promovido a tabela. As outras opções são entidades isoladas, sem ligação com outras.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-2
Área 6 · Engenharia de dados II

Sobre o Modelo Entidade-Relacionamento (MER), é CORRETO afirmar que:

- a) É utilizado exclusivamente em bancos de dados NoSQL.
- b) Identifica entidades, seus relacionamentos e os atributos que os descrevem.
- c) Não representa atributos, apenas entidades e relacionamentos.
- d) Substitui completamente o modelo relacional em projetos de banco de dados.

**Resposta certa:** b) Identifica entidades, seus relacionamentos e os atributos que os descrevem.

**Explicação:** A resposta é que o MER identifica entidades, os relacionamentos entre elas e os atributos que as descrevem. É um modelo conceitual usado para projetar bancos, principalmente relacionais, e costuma ser convertido em tabelas. Não é exclusivo de NoSQL e não substitui o modelo relacional.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-3
Área 6 · Engenharia de dados II

Considerando a tabela livros, criada em aula, qual comando SQL retorna todos os livros publicados após o ano de 2010?

- a) SELECT nome FROM livros WHERE ano_publicacao > 2010;
- b) SELECT nome FROM livros WHERE ano_publicacao < 2010;
- c) SELECT nome FROM livros ORDER BY ano_publicacao;
- d) SELECT * FROM livros WHERE vendas > 2010;

**Resposta certa:** a) SELECT nome FROM livros WHERE ano_publicacao > 2010;

**Explicação:** A resposta é SELECT nome FROM livros WHERE ano_publicacao > 2010;. O WHERE filtra as linhas pela condição, e o sinal de maior que traz só os anos posteriores a 2010. O sinal de menor traz os anteriores, ORDER BY só ordena sem filtrar e a última compara a coluna errada.

**Fonte:** Data Science do Zero, pág. 394

**Situação:** explicação conferida com o material das aulas

---

### Questão 149365-1-4
Área 6 · Engenharia de dados II

Sobre a integração entre sistemas operacionais e sistemas analíticos, é CORRETO afirmar que:

- a) Só pode ser realizada em tempo real, por meio de tecnologias de streaming de dados.
- b) É restrita a ambientes baseados em bancos de dados NoSQL, devido à sua flexibilidade.
- c) Tem como principal finalidade a geração de dashboards para apresentação visual dos dados.
- d) Tem o objetivo de conectar a infraestrutura operacional de dados às necessidades de análise e tomada de decisão.

**Resposta certa:** d) Tem o objetivo de conectar a infraestrutura operacional de dados às necessidades de análise e tomada de decisão.

**Explicação:** A resposta é a que fala em conectar a infraestrutura operacional às necessidades de análise e decisão, porque essa é a razão de ser da integração: levar o que os sistemas transacionais produzem para onde dá para analisar. Não precisa ser só em tempo real (existe carga em lote), nem ficar restrita a NoSQL, e o dashboard é só um dos usos possíveis no fim da cadeia.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-5
Área 6 · Engenharia de dados II

Considere os conceitos relacionados à Engenharia de Dados e assinale a alternativa que apresenta uma característica central de uma entidade forte:

- a) Possui uma chave primária própria, que a identifica de forma única no banco de dados.
- b) Não possui chave primária completa sem a chave de outra entidade.
- c) Representa um relacionamento entre entidades e pode conter atributos adicionais.
- d) Depende de outra entidade para garantir sua existência no modelo.

**Resposta certa:** a) Possui uma chave primária própria, que a identifica de forma única no banco de dados.

**Explicação:** A resposta é a que diz que a entidade forte tem chave primária própria. Ela se identifica sozinha, sem precisar da chave de outra entidade. Quem depende de outra para existir ou para completar a chave é a entidade fraca, e quem representa um relacionamento com atributos próprios é a entidade associativa.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-6
Área 6 · Engenharia de dados II

Qual é o comando SQL correto para remover a tabela “comentários” do banco de dados?

- a) REMOVE TABLE comentarios;
- b) DELETE TABLE comentarios;
- c) DROP TABLE comentarios;
- d) ERASE comentarios;

**Resposta certa:** c) DROP TABLE comentarios;

**Explicação:** A resposta é DROP TABLE comentarios;, que apaga a tabela inteira (estrutura e dados) do banco. DELETE remove linhas dentro da tabela e não aceita a forma DELETE TABLE. REMOVE TABLE e ERASE não existem no SQL padrão.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-7
Área 6 · Engenharia de dados II

No contexto de Engenharia da Dados, uma chave estrangeira é utilizada para:

- a) Estabelecer um vínculo entre registros de tabelas diferentes, mantendo a integridade referencial.
- b) Armazenar informações textuais fornecidas pelos usuários, como observações ou comentários.
- c) Assegurar que os valores em uma coluna sejam únicos dentro de uma tabela.
- d) Criar índices que otimizam o desempenho das consultas em grandes volumes de dados.

**Resposta certa:** a) Estabelecer um vínculo entre registros de tabelas diferentes, mantendo a integridade referencial.

**Explicação:** A resposta é a que fala em vincular registros de tabelas diferentes mantendo a integridade referencial. A chave estrangeira guarda o valor da chave primária de outra tabela e impede referências a registros que não existem. Garantir unicidade é papel da chave primária ou da restrição UNIQUE, e acelerar consultas é papel do índice.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-8
Área 6 · Engenharia de dados II

Considere os conceitos relacionados à Engenharia de Dados e assinale a alternativa que apresenta um exemplo de entidade fraca.

- a) Uma tabela de "clientes", com CPF como chave primária e independente de outras tabelas.
- b) Uma tabela de "itens de pedido", que depende de um "pedido" para existir.
- c) Uma tabela de "produtos", que possui código único e pode existir sem vínculos com outras entidades.
- d) Uma tabela de "fornecedores", que armazena CNPJ, razão social e telefone, de forma autônoma.

**Resposta certa:** b) Uma tabela de "itens de pedido", que depende de um "pedido" para existir.

**Explicação:** A resposta é itens de pedido, porque um item só faz sentido dentro de um pedido: sua identificação depende da chave do pedido, e sem ele o item não existe. Clientes, produtos e fornecedores têm chave própria e existem de forma independente, então são entidades fortes.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 149365-1-9
Área 6 · Engenharia de dados II

Para criar uma tabela em SQL, utiliza-se o comando:

- a) NEW TABLE nome (...);
- b) CREATE TABLE nome (...);
- c) SELECT * INTO nome (...);
- d) INSERT TABLE nome (...);

**Resposta certa:** b) CREATE TABLE nome (...);

**Explicação:** A resposta é CREATE TABLE nome (...);, que define a tabela com os nomes e tipos das colunas. O livro mostra o exemplo com a tabela users, declarando user_id como INT NOT NULL e name como VARCHAR. INSERT serve para colocar linhas numa tabela já criada, e NEW TABLE não existe.

**Fonte:** Data Science do Zero, pág. 390

**Situação:** explicação conferida com o material das aulas

---

## Engenharia de dados III

### Questão 150431-1-1
Área 6 · Engenharia de dados III

O que caracteriza uma arquitetura de dados do tipo Data Mesh?

- a) Cada equipe cuida dos dados do seu domínio, preparando-os para uso por outros.
- b) Toda a coleta de dados é feita por ferramentas de automação.
- c) Uma única equipe controla todos os dados da organização.
- d) Os dados são gerenciados apenas por analistas de negócios.

**Resposta certa:** a) Cada equipe cuida dos dados do seu domínio, preparando-os para uso por outros.

**Explicação:** A resposta é a que diz que cada equipe cuida dos dados do seu domínio e os prepara para uso por outros. Isso é a ideia central do Data Mesh: propriedade descentralizada por domínio, com os dados tratados como produto. Uma única equipe controlando tudo descreve a arquitetura centralizada, o oposto do mesh.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-10
Área 6 · Engenharia de dados III

Assinale a opção que representa uma vantagem do uso de procedures em um banco de dados:

- a) Criação automática de views.
- b) Execução de tarefas automatizadas com segurança e controle.
- c) Geração automática de relatórios visuais.
- d) Substituição de tabelas físicas por tabelas virtuais.

**Resposta certa:** b) Execução de tarefas automatizadas com segurança e controle.

**Explicação:** A resposta é executar tarefas automatizadas com segurança e controle, já que a procedure encapsula a rotina no banco e permite dar permissão de execução sem liberar acesso direto às tabelas. Criar views, gerar relatórios visuais e trocar tabelas físicas por virtuais não são funções de procedure.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-2
Área 6 · Engenharia de dados III

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre uma arquitetura centralizada de dados.

- a) Cada equipe define sua própria infraestrutura de dados.
- b) Uma equipe dedicada é responsável por toda a coleta e organização dos dados.
- c) Os times são independentes na organização e análise dos dados.
- d) O modelo é adequado apenas para ambientes distribuídos.

**Resposta certa:** b) Uma equipe dedicada é responsável por toda a coleta e organização dos dados.

**Explicação:** A resposta é a que coloca uma equipe dedicada responsável por toda a coleta e organização dos dados. Na arquitetura centralizada existe um time central de dados que atende a empresa toda. As demais alternativas (cada equipe com sua infraestrutura, times independentes) descrevem modelos descentralizados.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-3
Área 6 · Engenharia de dados III

Classifique em V (verdadeiro) ou F (falso) cada uma das três assertivas abaixo e em seguida assinale a alternativa com a sequência correta de V ou F:

( ) Views não podem alterar os dados.

( ) Procedures não podem receber parâmetros de entrada.

( ) Views são úteis para abstrair dados.
Classifique em V (verdadeiro) ou F (falso) cada uma das três assertivas abaixo e em seguida assinale a alternativa com a sequência correta de V ou F:
( ) Views não podem alterar os dados.
( ) Procedures não podem receber parâmetros de entrada.
( ) Views são úteis para abstrair dados.

- a) F, F, V
- b) V, F, F
- c) V, V, V
- d) V, F, V

**Resposta certa:** d) V, F, V

**Explicação:** O gabarito V, F, V parte de que view serve para consulta e abstração e de que procedure aceita parâmetros de entrada (a segunda frase é falsa de qualquer jeito). A primeira frase é o ponto delicado: em muitos bancos, views simples são atualizáveis e permitem INSERT, UPDATE e DELETE, então dizer que views não alteram dados só vale como regra geral da aula.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** A primeira assertiva (views não podem alterar os dados) é discutível, pois views simples costumam ser atualizáveis; a resposta depende da definição adotada na aula.

---

### Questão 150431-1-4
Área 6 · Engenharia de dados III

No contexto da Engenharia de Dados, um benefício comum entre views e procedures é:

- a) Eliminar a necessidade de tabelas no banco.
- b) Armazenar dados historicamente.
- c) Controlar o acesso físico ao banco de dados.
- d) Promover a reutilização de lógica e consultas.

**Resposta certa:** d) Promover a reutilização de lógica e consultas.

**Explicação:** A resposta é promover a reutilização de lógica e consultas. A view guarda uma consulta pronta e a procedure guarda um bloco de lógica, e os dois podem ser chamados de vários lugares sem reescrever o código. Nenhum dos dois elimina tabelas, guarda histórico nem controla acesso físico ao banco.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-5
Área 6 · Engenharia de dados III

Qual das alternativas representa uma motivação válida para o uso de views em bancos de dados?

- a) Evitar o uso de consultas SQL.
- b) Substituir procedures.
- c) Eliminar o uso de índices.
- d) Simplificar consultas complexas e abstrair dados.

**Resposta certa:** d) Simplificar consultas complexas e abstrair dados.

**Explicação:** A resposta é simplificar consultas complexas e abstrair dados. A view esconde joins e filtros atrás de um nome simples, e o usuário consulta como se fosse uma tabela. Ela não evita SQL (é feita de SQL), não substitui procedures e não tem relação com a eliminação de índices.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-6
Área 6 · Engenharia de dados III

Considere os conceitos relacionados à Engenharia de Dados e responda: Uma view é particularmente útil em qual situação?

- a) Quando é preciso reutilizar uma mesma consulta em diferentes relatórios.
- b) Quando o engenheiro quer-se substituir procedures existentes.
- c) Quando há necessidade de criar múltiplos índices para performance.
- d) Quando deseja-se executar ações automáticas em tempo real.

**Resposta certa:** a) Quando é preciso reutilizar uma mesma consulta em diferentes relatórios.

**Explicação:** A resposta é reutilizar a mesma consulta em diferentes relatórios, porque a view guarda a consulta uma vez e todos os relatórios passam a ler dela. Executar ações automáticas é papel de trigger, e criar índices ou substituir procedures não é objetivo de view.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-7
Área 6 · Engenharia de dados III

Sobre a definição de uma view em SQL, é CORRETO afirmar que:

- a) É utilizada apenas para criar índices.
- b) É uma tabela física que armazena dados permanentemente.
- c) É usada para alterar diretamente os dados de uma tabela.
- d) É uma tabela virtual baseada em uma consulta SQL.

**Resposta certa:** d) É uma tabela virtual baseada em uma consulta SQL.

**Explicação:** A resposta é que a view é uma tabela virtual baseada em uma consulta SQL. Ela não guarda os dados fisicamente: a consulta é executada sobre as tabelas de origem a cada acesso. Por isso não é uma tabela física permanente e também não serve para criar índices.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-8
Área 6 · Engenharia de dados III

No contexto da Engenharia de Dados, quando se recomenda a criação de uma view?

- a) Quando se precisa reutilizar consultas complexas em diferentes contextos.
- b) Quando se quer excluir dados duplicados.
- c) Quando se deseja armazenar grandes volumes de dados brutos.
- d) Quando se quer automatizar cálculos complexos com lógica condicional.

**Resposta certa:** a) Quando se precisa reutilizar consultas complexas em diferentes contextos.

**Explicação:** A resposta é reutilizar consultas complexas em diferentes contextos, que é o uso típico de uma view. Automatizar cálculo com lógica condicional pede procedure ou função, e guardar grande volume de dados brutos pede tabela. Excluir duplicados é operação de limpeza, não de view.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 150431-1-9
Área 6 · Engenharia de dados III

No contexto da Engenharia de Dados, um dos benefícios do uso de procedures é:

- a) Otimizar relatórios gráficos diretamente.
- b) Eliminar a necessidade de views.
- c) Criar arquivos em formato PDF.
- d) Reutilização de código e organização do banco.

**Resposta certa:** d) Reutilização de código e organização do banco.

**Explicação:** A resposta é reutilização de código e organização do banco. A procedure guarda a lógica no servidor e pode ser chamada por várias aplicações, o que evita repetir código e concentra as regras num lugar só. Ela não gera PDF, não otimiza gráficos e não elimina a necessidade de views.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Legislação no Ambiente Digital (LGPD)

### Questão 158034-1-1
Área 6 · Legislação no Ambiente Digital (LGPD)

Com relação aos dados pessoais sensíveis, o que estabelece a Lei Geral de Proteção de Dados (LGPD)?

- a) A LGPD trouxe um rol de dados de cunho íntimo, como origem racial ou étnica, convicção religiosa, opinião política, dados referentes à saúde ou à vida sexual, dados genéticos ou biométricos, entre outros.
- b) Dados sensíveis podem ser utilizados livremente, desde que o titular autorize verbalmente o tratamento.
- c) A LGPD não trata especificamente sobre dados pessoais sensíveis.
- d) As informações financeiras e movimentações bancárias do indivíduo são consideradas dados sensíveis pela LGPD.

**Resposta certa:** a) A LGPD trouxe um rol de dados de cunho íntimo, como origem racial ou étnica, convicção religiosa, opinião política, dados referentes à saúde ou à vida sexual, dados genéticos ou biométricos, entre outros.

**Explicação:** A resposta é a que lista o rol de dados íntimos: origem racial ou étnica, convicção religiosa, opinião política, saúde, vida sexual, dados genéticos ou biométricos. Esses dados têm tratamento diferenciado porque podem gerar discriminação. Dados financeiros não entram no rol, e o consentimento verbal não basta.

**Fonte:** Aula de Legislação no ambiente digital, pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-10
Área 6 · Legislação no Ambiente Digital (LGPD)

Qual a finalidade da Lei Geral de Proteção de Dados?

- a) Proteção dos direitos fundamentais, por meio da proteção dos dados das pessoas físicas.
- b) Regulamentar o tratamento de dados apenas no meio digital.
- c) Proteger os dados das pessoas físicas e jurídicas.
- d) Regulamentar as atividades de proteção de dados realizadas por empresas públicas.

**Resposta certa:** a) Proteção dos direitos fundamentais, por meio da proteção dos dados das pessoas físicas.

**Explicação:** A resposta é proteger os direitos fundamentais por meio da proteção dos dados das pessoas físicas, como privacidade e liberdade. A lei vale para tratamento digital e físico, e não protege pessoa jurídica. Também não se limita a empresas públicas.

**Fonte:** Aula de Legislação no ambiente digital, pág. 14

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-2
Área 6 · Legislação no Ambiente Digital (LGPD)

Qual das alternativas abaixo apresenta princípios da Lei Geral de Proteção de Dados (LGPD)?

- a) Liberdade das partes, impessoalidade e moralidade.
- b) Moralidade administrativa, função social e autonomia de vontades.
- c) Consensualismo, equilíbrio econômico e publicidade.
- d) Finalidade, necessidade, transparência e segurança.

**Resposta certa:** d) Finalidade, necessidade, transparência e segurança.

**Explicação:** A resposta é finalidade, necessidade, transparência e segurança, que aparecem entre os princípios da LGPD ao lado de adequação, livre acesso, qualidade, não discriminação, responsabilização e prevenção. As outras alternativas misturam princípios de direito civil e administrativo, como autonomia da vontade, moralidade e impessoalidade.

**Fonte:** Aula de Legislação no ambiente digital, pág. 15 e 33

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-3
Área 6 · Legislação no Ambiente Digital (LGPD)

O vazamento de dados, nos termos da Lei Geral de Proteção de Dados (LGPD), abrange qual das situações abaixo?

- a) Ataque hacker, com ações de phishing, por exemplo, que resultem na divulgação indevida de dados pessoais.
- b) Armazenamento de dados pessoais em servidor seguro e criptografado.
- c) Atualização cadastral feita com autorização do titular dos dados.
- d) Compartilhamento de dados pessoais entre departamentos da mesma empresa, desde que para fins internos.

**Resposta certa:** a) Ataque hacker, com ações de phishing, por exemplo, que resultem na divulgação indevida de dados pessoais.

**Explicação:** A resposta é o ataque hacker, como o phishing, que resulta em divulgação indevida de dados. Esse é um incidente de segurança, e a aula usa o caso da Enel, responsabilizada pelo STJ mesmo com o ataque vindo de terceiros, por não ter adotado medidas de segurança adequadas. Armazenar com criptografia ou atualizar cadastro com autorização são tratamentos regulares.

**Fonte:** Aula de Legislação no ambiente digital, pág. 50

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-4
Área 6 · Legislação no Ambiente Digital (LGPD)

De acordo com a Lei Geral de Proteção de Dados (LGPD), quem é o responsável pelas tarefas descritas abaixo, respectivamente?

i) Tomar as decisões referentes à forma e à duração do tratamento dos dados pessoais;

ii) Realizar o tratamento de dados conforme as instruções do outro agente.
De acordo com a Lei Geral de Proteção de Dados (LGPD), quem é o responsável pelas tarefas descritas abaixo, respectivamente?

i) Tomar as decisões referentes à forma e à duração do tratamento dos dados pessoais;
ii) Realizar o tratamento de dados conforme as instruções do outro agente.

- a) ANPD e Encarregado.
- b) Operador e Controlador.
- c) Controlador e Operador.
- d) Encarregado e Controlador.

**Resposta certa:** c) Controlador e Operador.

**Explicação:** A resposta é controlador e operador, nessa ordem. O controlador toma as decisões sobre forma e duração do tratamento, e o operador trata os dados em nome dele, seguindo as suas instruções. O encarregado é o canal de comunicação e a ANPD fiscaliza.

**Fonte:** Aula de Legislação no ambiente digital, pág. 49 e 25

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-5
Área 6 · Legislação no Ambiente Digital (LGPD)

A transparência é um dos princípios da LGPD e também constitui um princípio fundamental da Administração Pública. Nesse contexto, qual é o principal desafio de conciliação entre esses dois princípios?

- a) O desafio é conciliar a necessidade de transparência, especialmente em relação às atividades governamentais, com o direito à privacidade dos indivíduos. Enquanto a LAI (Lei de Acesso à Informação) promove um ambiente de abertura e acesso à informação, a LGPD impõe limites para proteger dados pessoais.
- b) O desafio consiste em substituir a LAI pela LGPD, de forma que apenas esta regule a transparência pública.
- c) O desafio é garantir que todos os dados pessoais tratados pela Administração Pública sejam divulgados para aumentar a confiança da população.
- d) O desafio está em eliminar completamente a publicidade dos atos administrativos, evitando qualquer exposição de informações.

**Resposta certa:** a) O desafio é conciliar a necessidade de transparência, especialmente em relação às atividades governamentais, com o direito à privacidade dos indivíduos. Enquanto a LAI (Lei de Acesso à Informação) promove um ambiente de abertura e acesso à informação, a LGPD impõe limites para proteger dados pessoais.

**Explicação:** A resposta é conciliar a transparência das atividades governamentais com a privacidade das pessoas. A LAI abre o acesso à informação pública, enquanto a LGPD põe limites para proteger dados pessoais, e o desafio está em equilibrar as duas. As outras opções propõem substituir uma lei ou eliminar um dos lados, o que não é a ideia.

**Fonte:** Aula de Legislação no ambiente digital, pág. 35

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-6
Área 6 · Legislação no Ambiente Digital (LGPD)

O que são dados pessoais no contexto da Lei Geral de Proteção de Dados (LGPD)?

- a) Dados cadastrais como nome, endereço, conta bancária e números de documentos.
- b) Somente aqueles que se referem à intimidade, como filiação sindical, opinião política, dados de saúde dentre outros.
- c) Qualquer informação referente à pessoa física, identificada ou identificável.
- d) Razão social e número de CNPJ.

**Resposta certa:** c) Qualquer informação referente à pessoa física, identificada ou identificável.

**Explicação:** A resposta é qualquer informação referente à pessoa física identificada ou identificável. A definição é ampla: nome, endereço e documentos são só exemplos, e o que é íntimo (sindicato, saúde, política) é a subcategoria dos dados sensíveis. Dados de pessoa jurídica, como CNPJ, ficam fora.

**Fonte:** Aula de Legislação no ambiente digital, pág. 17 e 19

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-7
Área 6 · Legislação no Ambiente Digital (LGPD)

Qual das alternativas representa um dos direitos dos titulares de dados pessoais previstos na Lei Geral de Proteção de Dados (LGPD)?

- a) Anonimização, bloqueio ou eliminação de dados desnecessários, excessivos ou tratados em desconformidade com a lei.
- b) A venda de dados pessoais a terceiros, desde que garantido o anonimato do titular.
- c) A transferência compulsória de dados pessoais para órgãos públicos, independentemente de consentimento.
- d) A coleta e o tratamento de dados pessoais sem necessidade de informar a finalidade.

**Resposta certa:** a) Anonimização, bloqueio ou eliminação de dados desnecessários, excessivos ou tratados em desconformidade com a lei.

**Explicação:** A resposta é anonimização, bloqueio ou eliminação de dados desnecessários, excessivos ou em desconformidade, que está na lista de direitos do titular junto com acesso, correção, portabilidade e revogação do consentimento. Vender dados, transferir compulsoriamente ou tratar sem informar a finalidade vão contra a lei.

**Fonte:** Aula de Legislação no ambiente digital, pág. 20

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-8
Área 6 · Legislação no Ambiente Digital (LGPD)

De acordo com o Marco Legal das Criptomoedas (Lei Nº 14.478, de 21 de dezembro de 2022), é CORRETO afirmar que:

- a) As atividades relacionadas a criptoativos no Brasil não requerem supervisão de órgãos governamentais, operando de forma totalmente independente.
- b) Empresas que operam com criptoativos devem se registrar e obter autorização do governo brasileiro para funcionar.
- c) A lei não estabelece procedimentos específicos para prevenir a lavagem de dinheiro e o financiamento ao terrorismo no mercado de criptoativos.
- d) O Marco Legal dos Criptoativos desencoraja a transparência e não exige que sejam fornecidas informações claras sobre os riscos associados aos criptoativos.

**Resposta certa:** b) Empresas que operam com criptoativos devem se registrar e obter autorização do governo brasileiro para funcionar.

**Explicação:** A resposta é que empresas que operam com criptoativos precisam de autorização do governo para funcionar. A Lei 14.478/2022 trata das prestadoras de serviços de ativos digitais e prevê regras de autorização de funcionamento, supervisão e cancelamento da autorização. Por isso não são atividades sem supervisão.

**Fonte:** Aula de Legislação no ambiente digital, pág. 11

**Situação:** explicação conferida com o material das aulas

---

### Questão 158034-1-9
Área 6 · Legislação no Ambiente Digital (LGPD)

No contexto do equilíbrio entre transparência e privacidade no Brasil, qual das seguintes afirmações é correta?

- a) A divulgação de informações de funcionários públicos exemplifica um conflito entre a necessidade de transparência e a proteção de dados pessoais.
- b) A Lei Geral de Proteção de Dados (LGPD) e a Lei de Acesso à Informação (LAI) têm objetivos completamente opostos, sendo impossível conciliá-los.
- c) A LGPD permite a divulgação irrestrita de dados pessoais de funcionários públicos em nome da transparência.
- d) Não existe distinção entre dados públicos e dados sensíveis no que diz respeito à transparência e privacidade.

**Resposta certa:** a) A divulgação de informações de funcionários públicos exemplifica um conflito entre a necessidade de transparência e a proteção de dados pessoais.

**Explicação:** A resposta é que a divulgação de dados de funcionários públicos exemplifica o conflito entre transparência e proteção de dados. A transparência pede alguma divulgação, e a LGPD protege contra a exposição indevida. As leis não são opostas a ponto de não conciliar, e a LGPD não libera divulgação irrestrita.

**Fonte:** Aula de Legislação no ambiente digital, pág. 35

**Situação:** explicação conferida com o material das aulas

---

## Liderança em Data Science

### Questão 157423-1-1
Área 6 · Liderança em Data Science

O "Manual de Liderança para a Era Digital" (MIT Sloan Management Review, 2020) apresenta diretrizes fundamentais para líderes contemporâneos. Qual das alternativas reflete corretamente um desses apontamentos?

- a) A urgência da transformação exige que líderes abandonem práticas tradicionais, pois o tempo para adaptação está se esgotando.
- b) A transformação digital deve ser conduzida prioritariamente pelo departamento de TI, com envolvimento limitado da liderança executiva.
- c) Os líderes devem focar exclusivamente em competências técnicas, delegando aspectos humanos para a área de recursos humanos.
- d) A liderança eficaz na era digital requer manter hierarquias rígidas para garantir controle sobre processos automatizados.

**Resposta certa:** a) A urgência da transformação exige que líderes abandonem práticas tradicionais, pois o tempo para adaptação está se esgotando.

**Explicação:** A resposta é a que fala na urgência da mudança: o material diz que a necessidade de mudar é urgente e que o tempo está se esgotando para líderes que se apegam às formas antigas de trabalhar e liderar. As outras opções (TI sozinha, só técnica, hierarquia rígida) vão contra a ideia de transformar a si mesmo e à equipe.

**Fonte:** Aula de Liderança em Data Science, pág. 20

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-10
Área 6 · Liderança em Data Science

Durante a aula foram discutidas as três dores da incerteza que afetam equipes e líderes em contextos de mudança. Quais são elas?

- a) Paciência, frustração e coragem.
- b) Ansiedade, desconfiança e desânimo.
- c) Insegurança, paralisia e resiliência.
- d) Medo, confusão e resistência.

**Resposta certa:** b) Ansiedade, desconfiança e desânimo.

**Explicação:** A resposta é ansiedade, desconfiança e desânimo, as três dores da incerteza, segundo a especialista Beatriz Garcia citada na aula. Cabe ao líder ajudar a equipe a lidar com elas. Medo, paralisia e resistência não fazem parte dessa lista.

**Fonte:** Aula de Liderança em Data Science, pág. 15

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-2
Área 6 · Liderança em Data Science

Daniel Goleman, especialista em inteligência emocional, identifica competências intrapessoais e interpessoais. Quais são as duas aptidões da inteligência emocional interpessoal?

- a) Autoconsciência e autorregulação.
- b) Pensamento estratégico e visão sistêmica.
- c) Consciência social e administração de relacionamentos.
- d) Comunicação assertiva e delegação eficaz.

**Resposta certa:** c) Consciência social e administração de relacionamentos.

**Explicação:** A resposta é consciência social e administração de relacionamentos, os dois domínios interpessoais da inteligência emocional de Goleman, que determinam o nosso relacionamento com os outros. Autoconsciência e autogestão são os domínios intrapessoais.

**Fonte:** Aula de Liderança em Data Science, pág. 35 e 36

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-3
Área 6 · Liderança em Data Science

Segundo o "Manual de Liderança para a Era Digital" (MIT Sloan Management Review, 2020), quais são os principais desafios enfrentados por líderes na atualidade?

- a) Redução de investimentos em tecnologia, priorização de processos manuais, evitar treinamentos e minimizar comunicação.
- b) Preservação de métodos tradicionais, rejeição de dados na tomada de decisão, isolamento de equipes e controle autoritário.
- c) Manutenção de estruturas hierárquicas rígidas, resistência à inovação, centralização de decisões e eliminação de feedback.
- d) Adaptação às mudanças, lacunas de habilidades, gestão da mudança e gestão da informação.

**Resposta certa:** d) Adaptação às mudanças, lacunas de habilidades, gestão da mudança e gestão da informação.

**Explicação:** A resposta é adaptação às mudanças, lacunas de habilidades, gestão da mudança e gestão da informação, que são os desafios listados no Manual de Liderança para a Era Digital. As demais alternativas descrevem comportamentos ruins, não desafios do líder.

**Fonte:** Aula de Liderança em Data Science, pág. 21

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-4
Área 6 · Liderança em Data Science

Para liderar em cenários de incerteza, o líder deve considerar alguns pontos de atenção importantes na relação com suas equipes. Dentre as alternativas abaixo, qual apresenta um ponto de atenção pertinente para o líder nesse contexto?

- a) Levar em conta os fatores emocionais resultantes do desconforto, da dissonância e da vulnerabilidade que a incerteza provoca.
- b) Priorizar a manutenção de rotinas rígidas e controles hierárquicos, pois a previsibilidade é o melhor antídoto contra a incerteza.
- c) Evitar expor a equipe a informações incertas ou contraditórias, a fim de preservar um ambiente de estabilidade e previsibilidade.
- d) Manter o foco exclusivamente nos resultados quantitativos, evitando discussões sobre aspectos emocionais que possam reduzir a objetividade da equipe.

**Resposta certa:** a) Levar em conta os fatores emocionais resultantes do desconforto, da dissonância e da vulnerabilidade que a incerteza provoca.

**Explicação:** A resposta é levar em conta os fatores emocionais do desconforto, da dissonância e da vulnerabilidade que a incerteza provoca. Esse é um dos pontos de atenção citados para o líder. As outras opções propõem rigidez, esconder informação ou ignorar emoções, o contrário do que se recomenda.

**Fonte:** Aula de Liderança em Data Science, pág. 67

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-5
Área 6 · Liderança em Data Science

Durante a aula foi discutido sobre o paradigma da empatia. Assinale a alternativa CORRETA sobre esse paradigma.

- a) É a capacidade de oferecer soluções racionais e objetivas para os problemas dos outros, evitando envolvimento emocional para manter a neutralidade.
- b) É a tendência de assumir as responsabilidades e emoções das outras pessoas, buscando resolver suas dificuldades de forma direta.
- c) É a habilidade de concordar com todas as opiniões do grupo, a fim de preservar o clima de harmonia e evitar conflitos interpessoais.
- d) É o comportamento de esforçar-se para compreender as razões e emoções de outras pessoas, assim como suas motivações, desejos e intenções.

**Resposta certa:** d) É o comportamento de esforçar-se para compreender as razões e emoções de outras pessoas, assim como suas motivações, desejos e intenções.

**Explicação:** A resposta é que empatia é o comportamento de se esforçar para compreender razões, emoções, motivações, desejos e intenções do outro. Na aula ela é tratada como comportamento e não como sentimento, e não exige sentir o mesmo que a pessoa, nem concordar com tudo ou assumir os problemas dela.

**Fonte:** Aula de Liderança em Data Science, pág. 82

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-6
Área 6 · Liderança em Data Science

A inteligência emocional é fundamental para líderes. Daniel Goleman, um dos maiores especialistas no tema, propõe que a inteligência emocional intrapessoal é composta por quais aptidões?

- a) Autoconsciência e autogestão.
- b) Empatia e habilidades sociais.
- c) Assertividade e negociação.
- d) Motivação e comunicação.

**Resposta certa:** a) Autoconsciência e autogestão.

**Explicação:** A resposta é autoconsciência e autogestão, os domínios intrapessoais, ou seja, as capacidades que determinam como lidamos conosco. Empatia e habilidades sociais pertencem ao lado interpessoal.

**Fonte:** Aula de Liderança em Data Science, pág. 35

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-7
Área 6 · Liderança em Data Science

Para lidar com cenários de incerteza, são necessárias algumas atitudes e capacidades específicas de um líder. Assinale a alternativa que apresenta uma atitude esperada de um líder em um momento de incerteza.

- a) Promover conversas abertas em ambientes de confiança, entendendo que, muitas vezes, opostos antagônicos podem ser complementares.
- b) Aguardar por maior clareza e estabilidade antes de tomar decisões, reduzindo o risco de cometer erros em situações indefinidas.
- c) Centralizar as decisões no líder, garantindo respostas rápidas e controle sobre todas as variáveis do processo.
- d) Evitar discussões divergentes para manter o grupo coeso e evitar conflitos que possam comprometer a produtividade.

**Resposta certa:** a) Promover conversas abertas em ambientes de confiança, entendendo que, muitas vezes, opostos antagônicos podem ser complementares.

**Explicação:** A resposta é promover conversas abertas em ambientes de confiança, entendendo que opostos antagônicos podem ser complementares. Está na lista de atitudes necessárias diante da incerteza. Esperar clareza, centralizar decisões ou evitar divergência são posturas que a aula aponta como falhas do líder.

**Fonte:** Aula de Liderança em Data Science, pág. 66

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-8
Área 6 · Liderança em Data Science

De acordo com a Teoria da Liderança na Complexidade (Complexity Leadership Theory), um líder deve integrar as características presentes em dois lados de uma organização. Quais são esses dois lados?

- a) O lado hierárquico, baseado em autoridade formal, e o lado colaborativo, baseado em trabalho em equipe.
- b) O lado administrativo, com foco em produzir eficiência, e o lado adaptativo, com foco em produzir inovação.
- c) O lado analítico, voltado para a interpretação de dados, e o lado criativo, voltado para a geração de novas ideias.
- d) O lado operacional, com foco em execução de tarefas, e o lado estratégico, com foco em planejamento de longo prazo.

**Resposta certa:** b) O lado administrativo, com foco em produzir eficiência, e o lado adaptativo, com foco em produzir inovação.

**Explicação:** A resposta é o lado administrativo, que produz eficiência, e o lado adaptativo, que produz inovação. O administrativo é formal, burocrático e linear, e o adaptativo é informal, criativo e não convencional. O líder integra os dois.

**Fonte:** Aula de Liderança em Data Science, pág. 63

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-1-9
Área 6 · Liderança em Data Science

De acordo com a Teoria da Liderança na Complexidade (Complexity Leadership) qual é a principal tarefa de uma liderança integradora?

- a) Assegurar o cumprimento rigoroso de regras e procedimentos, garantindo estabilidade e previsibilidade em todas as áreas.
- b) Priorizar exclusivamente a inovação, mesmo que isso comprometa a eficiência e a execução operacional.
- c) Concentrar as decisões estratégicas no topo da hierarquia, reduzindo a autonomia das equipes para evitar conflitos de direção.
- d) Promover a integração entre o lado adaptativo e o lado administrativo da organização.

**Resposta certa:** d) Promover a integração entre o lado adaptativo e o lado administrativo da organização.

**Explicação:** A resposta é promover a integração entre o lado adaptativo e o administrativo. A tarefa principal da liderança integradora é fazer interagir as narrativas formais e as histórias informais, e dessa interação nasce a clareza organizacional, que reduz o estresse e aumenta a produtividade.

**Fonte:** Aula de Liderança em Data Science, pág. 68

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-2-10
Área 6 · Liderança em Data Science

William James, no livro "Pragmatism" (1907), propõe uma distinção entre dois modelos mentais. Quais são eles?

- a) Data-driven (orientado por dados) e hypothesis-driven (orientado por hipóteses).
- b) Exploratório (busca padrões) e confirmatório (testa teorias).
- c) Tender-minded (pessoas sensíveis) e tough-minded (pessoas obstinadas).
- d) Dedutivo (do geral ao específico) e indutivo (do específico ao geral).

**Resposta certa:** c) Tender-minded (pessoas sensíveis) e tough-minded (pessoas obstinadas).

**Explicação:** A resposta é tender-minded (sensíveis) e tough-minded (obstinados), a tipologia psicológica de William James no livro Pragmatism. Os obstinados tendem a ser objetivos, racionais e céticos, e os sensíveis, subjetivistas e favoráveis ao livre arbítrio. Data-driven e dedutivo/indutivo são outros pares de conceitos.

**Fonte:** Aula de Liderança em Data Science, pág. 7

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-2-2
Área 6 · Liderança em Data Science

O neurocientista David Rock identificou três tipos de respostas que líderes costumam adotar diante de situações de crise. Quais são elas?

- a) Under-reacting (calma exagerada), adaptive (adaptação) e over-reacting (ansiedade exagerada).
- b) Avoidant (evitativa), proactive (proativa) e reactive (reativa).
- c) Passive (passiva), balanced (equilibrada) e impulsive (impulsiva).
- d) Defensive (defensiva), collaborative (colaborativa) e aggressive (agressiva).

**Resposta certa:** a) Under-reacting (calma exagerada), adaptive (adaptação) e over-reacting (ansiedade exagerada).

**Explicação:** A resposta é under-reacting (calma exagerada), adaptive (adaptação) e over-reacting (ansiedade exagerada). Na crise, o líder que minimiza e nada muda reage de menos, o que entra em pânico e contata todos obsessivamente reage demais, e o adaptativo se aproxima, empatiza e ajuda a preparar cenários.

**Fonte:** Aula de Liderança em Data Science, pág. 17

**Situação:** explicação conferida com o material das aulas

---

### Questão 157423-2-8
Área 6 · Liderança em Data Science

De acordo com Edgar Morin, filósofo da complexidade, o que caracteriza uma crise?

- a) É um período de transição linear e previsível entre um estado de equilíbrio e outro estado estável.
- b) É uma fase temporária de desordem que se resolve naturalmente sem necessidade de intervenção.
- c) É um momento em que as incertezas aumentam e os determinismos diminuem, exigindo novas formas de pensar.
- d) É uma situação de ruptura total do sistema que impede qualquer tipo de previsibilidade ou planejamento.

**Resposta certa:** c) É um momento em que as incertezas aumentam e os determinismos diminuem, exigindo novas formas de pensar.

**Explicação:** A resposta é que a crise é um momento em que as incertezas aumentam, na definição de Edgar Morin. Isso exige pensar de outro jeito, porque as certezas deixam de funcionar. Não é transição linear, nem desordem que se resolve sozinha, nem ruptura total sem previsibilidade.

**Fonte:** Aula de Liderança em Data Science, pág. 9

**Situação:** explicação conferida com o material das aulas

---

## Metodologias Ágeis I

### Questão 151020-1-1
Área 6 · Metodologias Ágeis I

Considere o Mapa do Problema apresentado em aula e responda: Qual é a sequência correta para preenchimento do Mapa do Problema em projetos ágeis?

- a) Contexto do problema → Efeitos conhecidos → Causas identificadas → Pessoas impactadas → Importância → Realidade x Ideal.
- b) Realidade x Ideal → Pessoas impactadas → Contexto do problema → Importância → Causas identificadas → Efeitos conhecidos.
- c) Causas identificadas → Contexto do problema → Realidade x Ideal → Pessoas impactadas → Efeitos conhecidos → Importância.
- d) Pessoas impactadas → Importância → Contexto do problema → Causas identificadas → Efeitos conhecidos → Realidade x Ideal.

**Resposta certa:** a) Contexto do problema → Efeitos conhecidos → Causas identificadas → Pessoas impactadas → Importância → Realidade x Ideal.

**Explicação:** A resposta é a que começa por Contexto do problema e termina em Realidade x Ideal. O Mapa do Problema parte da situação, passa pelos efeitos e causas e pelas pessoas afetadas, e só então fecha com a importância e o contraste entre o que existe e o que se deseja. As outras opções embaralham essa ordem. Essa ordem também bate com o agrupamento das outras questões sobre o mapa (Consistência e Relevância).

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-10
Área 6 · Metodologias Ágeis I

Durante a aula foram apresentadas as Seis Características da Abordagem de Rugby. Assinale a alternativa que apresenta três dessas características.

- a) Especificações técnicas completas, testes automatizados e integração contínua.
- b) Equipes de projeto auto-organizadas, fases de desenvolvimento sobrepostas e transferência organizacional de aprendizado.
- c) Reuniões diárias obrigatórias, sprints de duração fixa e retrospectivas semanais.
- d) Planejamento detalhado, documentação extensiva e controle hierárquico rigoroso.

**Resposta certa:** b) Equipes de projeto auto-organizadas, fases de desenvolvimento sobrepostas e transferência organizacional de aprendizado.

**Explicação:** A resposta é a que cita equipes auto-organizadas, fases sobrepostas e transferência organizacional de aprendizado. São três das seis características da abordagem de rugby de Takeuchi e Nonaka (as outras são instabilidade embutida, aprendizado múltiplo e controle sutil). As demais opções descrevem práticas de Scrum ou de gestão tradicional.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-2
Área 6 · Metodologias Ágeis I

Em relação à classificação dos problemas como conhecidos, conhecíveis ou incognoscíveis, assinale a alternativa CORRETA:

- a) Problemas conhecidos não podem ser resolvidos com frameworks estruturados.
- b) Problemas conhecíveis exigem descoberta e adaptação contínua.
- c) Problemas conhecidos exigem soluções empíricas baseadas em tentativa e erro.
- d) Problemas incognoscíveis podem ser resolvidos com processos preditivos.

**Resposta certa:** b) Problemas conhecíveis exigem descoberta e adaptação contínua.

**Explicação:** A resposta é que problemas conhecíveis exigem descoberta e adaptação contínua, porque a relação entre causa e efeito existe, mas ainda não está clara e precisa ser investigada aos poucos. Problemas conhecidos têm solução estabelecida e se resolvem bem com frameworks estruturados, e processos preditivos não servem para o incognoscível, o que elimina as demais.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-3
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e responda: Qual dos valores abaixo NÃO faz parte do Manifesto Ágil?

- a) Software funcionando mais que documentação extensa.
- b) Indivíduos e interações mais que processos e ferramentas.
- c) Documentação abrangente mais que software funcionando.
- d) Colaboração com o cliente mais que negociação de contratos.

**Resposta certa:** c) Documentação abrangente mais que software funcionando.

**Explicação:** A resposta é Documentação abrangente mais que software funcionando, porque o Manifesto Ágil faz o contrário: valoriza software funcionando mais que documentação abrangente. As outras três alternativas são valores do manifesto (indivíduos e interações, software funcionando, colaboração com o cliente).

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-4
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre a Gestão da Mudança:

- a) A gestão da mudança concentra sua energia em assegurar que as novas capacidades organizacionais sejam utilizadas e que a organização assuma o novo comportamento.
- b) A gestão da mudança concentra sua energia em assegurar que as estratégias de longo prazo sejam alinhadas com os objetivos financeiros da organização.
- c) A gestão da mudança concentra sua energia em assegurar que os processos operacionais sejam padronizados e continuamente otimizados.
- d) A gestão da mudança concentra sua energia em assegurar que os projetos sejam entregues dentro do prazo, escopo e orçamento estabelecidos.

**Resposta certa:** a) A gestão da mudança concentra sua energia em assegurar que as novas capacidades organizacionais sejam utilizadas e que a organização assuma o novo comportamento.

**Explicação:** A resposta é a que fala em garantir o uso das novas capacidades e a adoção do novo comportamento pela organização. A gestão da mudança trata do lado humano da transição, e não de entrega no prazo, escopo e orçamento, que é o foco da gestão de projetos, nem de otimização de processos ou alinhamento financeiro de longo prazo.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-5
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e responda: Quais elementos compõem o campo “Consistência” do Mapa do Problema?

- a) Problema, missão, indicadores e metas.
- b) Causas, consequências, metas e indicadores.
- c) Contexto, causas, consequências e pessoas impactadas/envolvidas.
- d) Estratégia, visão, escopo e entregas.

**Resposta certa:** c) Contexto, causas, consequências e pessoas impactadas/envolvidas.

**Explicação:** A resposta é Contexto, causas, consequências e pessoas impactadas/envolvidas, que são os elementos que descrevem o problema e dão consistência ao mapa. Importância e Realidade x Ideal ficam no campo de Relevância. Metas, indicadores, missão, visão e estratégia são elementos de outros instrumentos de planejamento.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-6
Área 6 · Metodologias Ágeis I

Julgue os itens como verdadeiros (V) ou falsos (F) e assinale a alternativa que apresenta a sequência CORRETA de V ou F:

( ) Nos processos preditivos, os requisitos são detalhados no começo do projeto.

( ) A abordagem adaptativa aceita a flexibilidade no escopo.

( ) No modelo empírico, tolerância zero é criada para prazo e custos.
Julgue os itens como verdadeiros (V) ou falsos (F) e assinale a alternativa que apresenta a sequência CORRETA de V ou F:
( ) Nos processos preditivos, os requisitos são detalhados no começo do projeto.
( ) A abordagem adaptativa aceita a flexibilidade no escopo.
( ) No modelo empírico, tolerância zero é criada para prazo e custos.

- a) V, V, V.
- b) V, V, F.
- c) V, F, F.
- d) F, V, V.

**Resposta certa:** a) V, V, V.

**Explicação:** A resposta é V, V, V. No preditivo o escopo e os requisitos são detalhados logo no início, e o adaptativo aceita mudar o escopo ao longo do caminho. No modelo empírico/ágil prazo e custo são tratados como restrições firmes (timebox), e o que se ajusta é o escopo. Por isso nenhum item é falso.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-7
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e selecione a alternativa com as palavras que preenchem as lacunas da assertiva abaixo: 

A abordagem preditiva assume que o __________ é fixo, e acomoda as incertezas no __________ e no __________.
Considere os conceitos discutidos em aula e selecione a alternativa com as palavras que preenchem as lacunas da assertiva abaixo:
A abordagem preditiva assume que o __________ é fixo, e acomoda as incertezas no __________ e no __________.

- a) custo / escopo / prazo
- b) escopo / prazo / custo
- c) cronograma / qualidade / risco
- d) prazo / escopo / qualidade

**Resposta certa:** b) escopo / prazo / custo

**Explicação:** A resposta é escopo / prazo / custo. A abordagem preditiva fecha o escopo no planejamento e, quando surgem incertezas, ajusta cronograma e orçamento. É o inverso do ágil, que fixa prazo e custo e deixa o escopo variar.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-8
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e responda: Quais elementos compõem o campo “Relevância” do Mapa do Problema?

- a) Importância e Realidade x Ideal.
- b) Estratégia, visão, escopo e entregas.
- c) Causas, consequências, metas e indicadores.
- d) Problema, missão, indicadores e metas.

**Resposta certa:** a) Importância e Realidade x Ideal.

**Explicação:** A resposta é Importância e Realidade x Ideal. No Mapa do Problema, o campo de Relevância mostra por que vale resolver o problema, ou seja, o quanto ele importa e a distância entre a situação atual e a desejada. Causas, consequências, metas e indicadores pertencem a outros campos ou a outros instrumentos.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-1-9
Área 6 · Metodologias Ágeis I

Durante a aula foram discutidos quatro estágios de disrupção. Quais são eles?

- a) Identificação, incubação, implementação e institucionalização.
- b) Emergência, crescimento, maturidade e declínio.
- c) Planejamento, execução, monitoramento e encerramento.
- d) Viabilidade, volatilidade, durabilidade e vulnerabilidade.

**Resposta certa:** d) Viabilidade, volatilidade, durabilidade e vulnerabilidade.

**Explicação:** O gabarito aponta viabilidade, volatilidade, durabilidade e vulnerabilidade. As demais opções são sequências de outros modelos conhecidos (ciclo de vida de produto, fases de projeto), então por eliminação a marcada é a que sobra, mas não há como conferir esses quatro estágios de disrupção no material recebido.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** Os quatro estágios de disrupção são conteúdo específico da aula e nenhum trecho recebido permite verificar o gabarito.

---

### Questão 151020-2-2
Área 6 · Metodologias Ágeis I

Considere os conceitos apresentados em aula e responda: O que melhor caracteriza uma mudança transformacional?

- a) A implementação de um novo software de controle interno.
- b) Uma alteração de processo dentro do mesmo setor.
- c) A modificação de um hábito operacional.
- d) A redefinição de identidade e modelo mental de uma organização.

**Resposta certa:** d) A redefinição de identidade e modelo mental de uma organização.

**Explicação:** A resposta é a redefinição de identidade e modelo mental da organização. A mudança transformacional altera a forma como a organização se enxerga e opera, em vez de ajustar algo pontual. Novo software, mudança de processo num setor ou de hábito operacional são mudanças incrementais ou de transição.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-2-6
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e assinale a alternativa CORRETA sobre a Gestão de Projetos:

- a) A Gestão de Projetos concentra sua energia em assegurar que as entregas sejam realizadas dentro das restrições.
- b) A Gestão de Projetos assegura que a organização alcance seus objetivos estratégicos de longo prazo.
- c) A Gestão de Projetos concentra sua energia em assegurar que os processos operacionais sejam continuamente otimizados.
- d) A Gestão de Projetos concentra sua energia em assegurar que a organização adote novos comportamentos permanentes.

**Resposta certa:** a) A Gestão de Projetos concentra sua energia em assegurar que as entregas sejam realizadas dentro das restrições.

**Explicação:** A resposta é garantir que as entregas ocorram dentro das restrições (prazo, escopo, custo). Esse é o foco da gestão de projetos. Adoção de novos comportamentos permanentes é gestão da mudança, e otimização contínua de processos e objetivos estratégicos de longo prazo estão fora do alcance de um projeto, que é temporário.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151020-2-7
Área 6 · Metodologias Ágeis I

Considere os conceitos discutidos em aula e responda: Qual das alternativas melhor representa a definição de projeto segundo o PMI (2021)?

- a) Uma ação contínua com escopo variável e resultados previsíveis.
- b) Um conjunto de tarefas administrativas executadas pela equipe funcional.
- c) Um esforço repetitivo para manter as rotinas operacionais.
- d) Um esforço temporário empreendido para criar um produto, serviço ou resultado único.

**Resposta certa:** d) Um esforço temporário empreendido para criar um produto, serviço ou resultado único.

**Explicação:** A resposta é esforço temporário empreendido para criar um produto, serviço ou resultado único, que é a definição do PMBOK. Temporário e único são as palavras que a separam das operações, que são contínuas e repetitivas, como sugerem as outras alternativas.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

## Metodologias Ágeis II

### Questão 151565-1-1
Área 6 · Metodologias Ágeis II

Qual domínio do modelo Cynefin é caracterizado por alta turbulência e pela necessidade de ação imediata?

- a) Complexo.
- b) Claro.
- c) Caótico.
- d) Complicado.

**Resposta certa:** c) Caótico.

**Explicação:** A resposta é o domínio Caótico. No Cynefin, ele tem turbulência alta e nenhuma relação perceptível entre causa e efeito, então a sequência é agir primeiro para estabilizar, depois sentir e responder. No Complexo se experimenta com calma, e no Complicado e no Claro há análise ou regra pronta.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-10
Área 6 · Metodologias Ágeis II

No modelo Cynefin, qual domínio é caracterizado por situações onde as respostas são conhecidas e a relação de causa e efeito é clara?

- a) Complicado.
- b) Complexo.
- c) Caótico.
- d) Claro.

**Resposta certa:** d) Claro.

**Explicação:** A resposta é o domínio Claro (antes chamado de Simples). Aqui causa e efeito são evidentes e as respostas já são conhecidas, então basta categorizar a situação e aplicar a melhor prática (sentir, categorizar, responder).

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-2
Área 6 · Metodologias Ágeis II

Qual domínio do modelo Cynefin requer análise de especialistas e apresenta múltiplas soluções possíveis para um mesmo problema?

- a) Caótico.
- b) Claro.
- c) Complicado.
- d) Complexo.

**Resposta certa:** c) Complicado.

**Explicação:** A resposta é o domínio Complicado. Causa e efeito existem, mas não são óbvios, e exigem análise de especialistas. Por isso pode haver mais de uma boa solução para o mesmo problema (sentir, analisar, responder). No Claro basta aplicar a melhor prática.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-3
Área 6 · Metodologias Ágeis II

No modelo Cynefin, em qual domínio as soluções emergem através de experimentação e há alta imprevisibilidade?

- a) Complicado.
- b) Claro.
- c) Complexo.
- d) Caótico.

**Resposta certa:** c) Complexo.

**Explicação:** A resposta é o domínio Complexo. Ali a causa e o efeito só se entendem em retrospecto, então as soluções emergem de experimentos seguros (sondar, sentir, responder) e a imprevisibilidade é alta. O Caótico também é imprevisível, mas pede ação imediata e não experimentação.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-4
Área 6 · Metodologias Ágeis II

Assinale a alternativa que apresenta uma diferença central do papel do Product Owner em comparação com o Scrum Master:

- a) O Product Owner define as tecnologias a serem utilizadas, já o Scrum Master define as práticas de codificação da equipe.
- b) O Product Owner gerencia o cronograma das entregas, já o Scrum Master gerencia o orçamento disponível para o projeto.
- c) O Product Owner foca nas prioridades para o negócio, já o Scrum Master foca nos processos e no desenvolvimento das pessoas.
- d) O Product Owner lidera a equipe de desenvolvimento, já o Scrum Master lidera a equipe de stakeholders externos.

**Resposta certa:** c) O Product Owner foca nas prioridades para o negócio, já o Scrum Master foca nos processos e no desenvolvimento das pessoas.

**Explicação:** A resposta é que o Product Owner foca nas prioridades de negócio, enquanto o Scrum Master foca nos processos e nas pessoas. O PO responde pelo valor do produto e pelo Product Backlog, e o SM cuida de o Scrum ser entendido e aplicado e de remover impedimentos. Nenhum deles define tecnologia, orçamento nem lidera o time.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-5
Área 6 · Metodologias Ágeis II

Qual estratégia de desenvolvimento pode ser utilizada para validar o problema com os usuários no estágio de Exploration - Discovery?

- a) Lean Six Sigma.
- b) Design Thinking.
- c) Market Testing.
- d) Lean Startup.

**Resposta certa:** b) Design Thinking.

**Explicação:** O gabarito marca Design Thinking, que faz sentido para entender e validar o problema junto aos usuários numa fase de descoberta, por conta da empatia e da imersão. Lean Startup também poderia ser defendida, e não há no material recebido a tabela de estratégias por estágio que desempata.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** DISCUTÍVEL: o gabarito diverge do que o material mostra

**Nota:** Mapeamento estágio x estratégia é conteúdo da aula e não pôde ser verificado; Lean Startup também seria plausível.

---

### Questão 151565-1-6
Área 6 · Metodologias Ágeis II

Na fase de Problem-Solution Fit, qual o objetivo do estágio de Exploration - Prototyping?

- a) Validar o problema com os usuários.
- b) Prototipar soluções iniciais.
- c) Testar o ajuste do problema-solução.
- d) Desenvolver o Produto Mínimo Viável (MVP)

**Resposta certa:** b) Prototipar soluções iniciais.

**Explicação:** A resposta é prototipar soluções iniciais. Dentro do Problem-Solution Fit, a descoberta valida o problema e a prototipação traz as primeiras versões de solução para testar. Desenvolver o MVP vem depois, já no Product-Market Fit.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-7
Área 6 · Metodologias Ágeis II

Na fase de Product-Market Fit, qual é a meta do estágio de Delivery - MVP?

- a) Lançar MVP e coletar feedback dos usuários.
- b) Implementar e testar melhorias críticas.
- c) Testar o ajuste do problema-solução.
- d) Realizar pesquisa de mercado com usuários.

**Resposta certa:** a) Lançar MVP e coletar feedback dos usuários.

**Explicação:** A resposta é lançar o MVP e coletar feedback dos usuários. A etapa de entrega do MVP no Product-Market Fit serve para pôr no ar a versão mínima e aprender com o uso real. Testar o ajuste problema-solução é da fase anterior, e a pesquisa de mercado vem antes do lançamento.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-8
Área 6 · Metodologias Ágeis II

Durante a aula foram apresentados os três estágios da mudança. Quais são eles?

- a) Ideia, planejamento e operação.
- b) Escopo, cronograma e orçamento.
- c) Problem-Solution fit, product-market fit e scale.
- d) Início, meio e fim.

**Resposta certa:** c) Problem-Solution fit, product-market fit e scale.

**Explicação:** A resposta é Problem-Solution fit, Product-market fit e Scale, que são os estágios do ciclo de evolução de um produto, percorridos em sequência. As outras opções falam de fases genéricas de projeto (ideia, planejamento, operação) ou de restrições (escopo, cronograma, orçamento).

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---

### Questão 151565-1-9
Área 6 · Metodologias Ágeis II

Considere os papéis dentro do Scrum e assinale a alternativa que apresenta características CORRETAS relacionadas ao trabalho dos desenvolvedores:

- a) Os desenvolvedores são uma equipe multidisciplinar e com profundos conhecimentos sobre sua área de atuação.
- b) Os desenvolvedores são responsáveis exclusivamente pela codificação do produto, cabendo ao Product Owner realizar os testes e validações de qualidade.
- c) Os desenvolvedores trabalham individualmente em suas especialidades e reportam progresso diário ao gerente de projeto designado para o time.
- d) Os desenvolvedores devem seguir estritamente as orientações do Scrum Master e aguardar suas instruções para iniciar qualquer atividade durante a sprint.

**Resposta certa:** a) Os desenvolvedores são uma equipe multidisciplinar e com profundos conhecimentos sobre sua área de atuação.

**Explicação:** A resposta é que os desenvolvedores formam uma equipe multidisciplinar com conhecimento profundo da sua área. No Scrum eles são auto-gerenciáveis e responsáveis por toda a qualidade do incremento, não só pela codificação. Não respondem ao Scrum Master para começar o trabalho nem a gerente de projeto.

**Fonte:** Conhecimento geral, sem apoio direto nas aulas

**Situação:** explicação geral, não achei trecho que confirme nas aulas

---
