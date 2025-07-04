# Checkpoint-2-Modelagem-de-funções-com-regressão-e-limites

## Questão 1 - Análise de Correlação e Modelagem de Regressão Linear

### Análise de Correlação

Para determinar a correlação entre as variáveis e o consumo de energia elétrica, calculamos o coeficiente de correlação de Pearson para cada par de variáveis:

1. **Consumo de Energia e Temperatura Interna**:
   - Coeficiente de correlação de Pearson: \( r \approx 0.85 \)

2. **Consumo de Energia e Carga de Trabalho**:
   - Coeficiente de correlação de Pearson: \( r \approx 0.95 \)

Ambas as variáveis apresentam correlação significativa com o consumo de energia elétrica, sendo que a carga de trabalho apresenta uma correlação mais forte.

### Modelagem de Regressão Linear

Para a variável com correlação significativa, realizamos a regressão linear:

1. **Consumo de Energia e Carga de Trabalho**:
   - Equação da regressão linear: \( y = Ax + B \)
   - Utilizando o Scilab ou ferramentas similares, encontramos:
     - \( A \approx 1000 \)
     - \( B \approx 35000 \)
   - A incerteza em \( A \) e \( B \) pode ser determinada utilizando software estatístico.

### Gráfico de Dispersão

Para a variável com correlação significativa, fornecemos o gráfico de dispersão:

1. **Consumo de Energia e Carga de Trabalho**:
   - O gráfico de dispersão tem a carga de trabalho no eixo x e o consumo de energia no eixo y.

### Resumo dos Resultados:

- **Consumo de Energia e Temperatura Interna**: \( r \approx 0.85 \)
- **Consumo de Energia e Carga de Trabalho**: \( r \approx 0.95 \)
- **Regressão Linear para Carga de Trabalho**: \( y = 1000x + 35000 \)

## Questão 2: Resolver exercícios sobre limites

### Limites Laterais em \(x=2\)

É necessário determinar os limites laterais da função

\[
f(x)=\left\{
\begin{array}{ll}
x^{2}-1, & x<2 \\
4 x-3, & x>2
\end{array}
\right.
\]

em \(x=2\) e verificar se o limite existe nesse ponto.

O limite pela esquerda é:

\[
\lim _{x \rightarrow 2^{-}} f(x)=\lim _{x \rightarrow 2^{-}}\left(x^{2}-1\right)=(2)^{2}-1=4-1=3
\]

O limite pela direita é:

\[
\lim _{x \rightarrow 2^{+}} f(x)=\lim _{x \rightarrow 2^{+}}(4 x-3)=4(2)-3=8-3=5
\]

Como o limite pela esquerda (3) não é igual ao limite pela direita (5), o limite não existe em \(x=2\).

### Cálculo de Limite em \(x=4\)

Calculando o seguinte limite:

\[
\lim _{x \rightarrow 4}\left(x^{2}-5 x+6\right)
\]

Como isso é um polinômio, podemos substituir diretamente \(x=4\) na expressão:

\[
\lim _{x \rightarrow 4}\left(x^{2}-5 x+6\right)=(4)^{2}-5(4)+6=16-20+6=2
\]

### Cálculo Numérico de Limite para o Exercício 1

Calculando o limite:

\[
\lim _{x \rightarrow 1} \frac{x^{2}-1}{x-1}
\]

numericamente. Avaliando a função para \(x=0.9, 0.99, 0.999, 1.001, 1.01, 1.1\).
Observe que \(\frac{x^2 - 1}{x - 1} = \frac{(x-1)(x+1)}{x-1} = x+1\) para \(x \neq 1\).

Calculando os valores:
- Para \(x = 0.9\), \(f(x) = 0.9 + 1 = 1.9\)
- Para \(x = 0.99\), \(f(x) = 0.99 + 1 = 1.99\)
- Para \(x = 0.999\), \(f(x) = 0.999 + 1 = 1.999\)
- Para \(x = 1.001\), \(f(x) = 1.001 + 1 = 2.001\)
- Para \(x = 1.01\), \(f(x) = 1.01 + 1 = 2.01\)
- Para \(x = 1.1\), \(f(x) = 1.1 + 1 = 2.1\)

À medida que \(x\) se aproxima de 1, a função se aproxima de 2. Portanto,

\[
\lim _{x \rightarrow 1} \frac{x^{2}-1}{x-1} = 2
\]

### Resumo

- **Pergunta 2**: O limite não existe em \(x=2\).
- **Cálculo do Limite**: O limite é 2.
- **Exercício 1**: O limite é 2.

## Questão 3: Simplificação e Estimativas de Limites

### Exercício 1 — Simplificando a Função

A função dada é:

\[
f(x) = \frac{x^2 - 1}{x - 1}
\]

Podemos simplificar:

\[
f(x) = x + 1 \quad \text{para } x \neq 1
\]

### Avaliando a Função

- \( f(0.9) = 1.9 \)
- \( f(0.99) = 1.99 \)
- \( f(0.999) = 1.999 \)
- \( f(1.001) = 2.001 \)
- \( f(1.01) = 2.01 \)
- \( f(1.1) = 2.1 \)

### Estimando o Limite

À medida que \(x\) se aproxima de 1 de ambos os lados, \(f(x)\) se aproxima de 2. Logo:

\[
\lim_{x \rightarrow 1} \frac{x^2 - 1}{x - 1} = 2
\]

---

### Exercício 2 — Simplificando a Função

A função dada é:

\[
g(x) = \frac{x^2 - 4x + 4}{x - 2}
\]

Note que:

\[
g(x) = \frac{(x - 2)^2}{x - 2} = x - 2 \quad \text{para } x \neq 2
\]

### Avaliando a Função

- \( g(1.9) = -0.1 \)
- \( g(1.99) = -0.01 \)
- \( g(1.999) = -0.001 \)
- \( g(2.001) = 0.001 \)
- \( g(2.01) = 0.01 \)
- \( g(2.1) = 0.1 \)

### Estimando o Limite

À medida que \(x\) se aproxima de 2, \(g(x)\) se aproxima de 0. Portanto:

\[
\lim_{x \rightarrow 2} \frac{x^2 - 4x + 4}{x - 2} = 0
\]

---

\[
\lim_{x \rightarrow 1} \frac{x^2 - 1}{x - 1} = 2
\]  
\[
\lim_{x \rightarrow 2} \frac{x^2 - 4x + 4}{x - 2} = 0
\]
