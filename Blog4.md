# Processamento de Histograma

## Introdução

O histograma é uma ferramenta utilizada no processamento digital de imagens para representar a distribuição dos níveis de intensidade dos pixels de uma imagem.

Ele mostra a quantidade de pixels que possuem cada valor de intensidade.

## Histograma

O histograma possui dois eixos principais:

**Eixo horizontal**: representa os níveis de intensidade, variando de 0 até L - 1.
**Eixo vertical**: representa a quantidade de pixels que possuem determinada intensidade.

A função do histograma é representada por:

h(rk) = nk

Onde:

rk = k-ésimo valor de intensidade;
nk = número de pixels da imagem com intensidade rk.

## Normalização do Histograma

O histograma pode ser normalizado dividindo a quantidade de pixels de cada intensidade pelo número total de pixels da imagem.

A fórmula é:

p(rk) = nk / (M × N)

Onde M × N representa o número total de pixels da imagem.

O valor p(rk) representa uma estimativa da probabilidade de ocorrência daquele nível de intensidade. A soma de todos os valores de um histograma normalizado é igual a 1.

## Análise do Histograma

A análise do histograma permite identificar algumas características básicas de uma imagem:

**Imagem escura**: maior concentração de pixels em baixas intensidades.
**Imagem clara**: maior concentração de pixels em altas intensidades.
**Imagem de baixo** contraste: intensidades concentradas em uma faixa pequena.
**Imagem de alto** contraste: intensidades distribuídas por uma faixa maior.

## Equalização de Histograma

A **equalização de histograma** tem como objetivo redistribuir os níveis de intensidade utilizando a **função de distribuição acumulada (CDF).**

O objetivo é produzir uma imagem com uma distribuição de intensidades mais uniforme, podendo melhorar o contraste da imagem.

A probabilidade de ocorrência de cada intensidade é calculada por:

p(rk) = nk / (M × N)

A partir dessa distribuição, é calculada a função de transformação utilizada na equalização do histograma.

A transformação pode ser representada por:

Sk = T(rk)

A equalização também é chamada de **linearização do histograma.**

## Aplicações

O processamento de histogramas pode ser utilizado para:

Realce de imagens digitais;
Obtenção de estatísticas da imagem;
Auxílio em processos de compressão;
Auxílio em processos de segmentação;
Melhoria da distribuição de contraste através da equalização.

## Conclusão

O processamento de histogramas é uma técnica importante no processamento digital de imagens. Através do histograma, é possível analisar como os níveis de intensidade estão distribuídos em uma imagem e identificar características como brilho e contraste.

A **equalização de histograma** permite redistribuir essas intensidades utilizando a distribuição acumulada, buscando uma distribuição mais uniforme dos níveis de intensidade.
