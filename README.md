content_v2 = """
# Checkpoint-2-Modelagem-de-funções-com-regressão-e-limites

## Questão 1:

## Questão 2: Resolver exercícios sobre limites

### Limites Laterais em \(x=2\)

Precisamos determinar os limites laterais da função

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

Precisamos calcular o seguinte limite:

\[
\lim _{x \rightarrow 4}\left(x^{2}-5 x+6\right)
\]

Como isso é um polinômio, podemos substituir diretamente \(x=4\) na expressão:

\[
\lim _{x \rightarrow 4}\left(x^{2}-5 x+6\right)=(4)^{2}-5(4)+6=16-20+6=2
\]

### Cálculo Numérico de Limite para o Exercício 1

Precisamos calcular o limite:

\[
\lim _{x \rightarrow 1} \frac{x^{2}-1}{x-1}
\]

numericamente. Vamos avaliar a função para \(x=0.9, 0.99, 0.999, 1.001, 1.01, 1.1\).
Observe que \(\frac{x^2 - 1}{x - 1} = \frac{(x-1)(x+1)}{x-1} = x+1\) para \(x \neq 1\).

Vamos calcular os valores:
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
"""

# Salvando o novo conteúdo em um arquivo .md
file_path_v2 = "/mnt/data/Checkpoint-2-Modelagem-de-funções-com-regressão-e-limites.md"
with open(file_path_v2, "w") as file:
    file.write(content_v2)

file_path_v2
