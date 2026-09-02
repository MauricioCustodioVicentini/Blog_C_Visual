# Transformações de Intensidade

## Computação Visual — Ciência da Computação

Este projeto apresenta um estudo sobre **Transformações de Intensidade**, um conceito do processamento digital de imagens realizado no domínio espacial.

As transformações de intensidade atuam diretamente nos pixels de uma imagem, realizando operações como alteração de contraste, transformação de negativos, aplicação de logaritmos e transformações de potência (gama).

## Objetivo

O objetivo desta atividade é compreender como diferentes funções de transformação podem modificar os níveis de intensidade de uma imagem, permitindo melhorar o contraste e destacar determinadas características.

## Principais transformações

### 1. Transformação Linear

Inclui principalmente:

* **Identidade:** mantém as intensidades da imagem original.
* **Negativo:** inverte os níveis de intensidade da imagem.

A transformação do negativo pode ser representada por:

`s = (L - 1) - r`

onde `L` representa a intensidade máxima da imagem.

### 2. Transformação Logarítmica

A transformação logarítmica é utilizada para **expandir as baixas intensidades** e **comprimir as altas intensidades**.

Dessa forma, detalhes presentes em regiões mais escuras podem se tornar mais visíveis, enquanto regiões muito claras podem ter seus níveis de intensidade comprimidos.

### 3. Transformação de Potência (Gama)

A transformação de potência é representada por:

`s = c · r^γ`

O valor de `γ` determina o comportamento da transformação.

* **γ < 1:** tende a clarear regiões de baixa intensidade e é útil para imagens escuras ou com baixo contraste.
* **γ > 1:** tende a realçar regiões de alta intensidade e pode ser utilizada em imagens com excesso de brilho.

### 4. Alargamento de Contraste

O alargamento de contraste expande a faixa de níveis de intensidade da imagem, sendo útil principalmente em imagens que apresentam baixo contraste. Esse problema pode ocorrer devido à iluminação inadequada ou às limitações do sensor utilizado na captura.

### 5. Fatiamento de Níveis de Intensidade

Essa técnica busca destacar uma determinada faixa de intensidades da imagem.

Pode ser utilizada, por exemplo, para realçar:

* Massas de água em imagens de satélite;
* Falhas em imagens de raio X;
* Regiões de interesse em imagens médicas.

### 6. Fatiamento por Planos de Bits

As imagens digitais são formadas por bits. Em uma imagem de 8 bits, por exemplo, existem **8 planos de 1 bit**, que representam diferentes contribuições para a aparência final da imagem.

Os planos mais significativos possuem maior influência na formação da imagem. A técnica também pode ser utilizada na compressão e reconstrução de imagens utilizando determinados planos de bits.

## Conclusão

As transformações de intensidade são importantes ferramentas do processamento digital de imagens. Por meio delas é possível modificar os níveis de intensidade dos pixels, melhorar o contraste, destacar regiões de interesse e tornar determinados detalhes mais visíveis.

Nesta atividade, foram abordadas as principais técnicas de transformação de intensidade, incluindo transformações lineares, logarítmicas, de potência, alargamento de contraste, fatiamento de níveis e fatiamento por planos de bits.
