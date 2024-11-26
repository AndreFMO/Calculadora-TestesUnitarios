## Relatório Detalhado do Resultado dos Testes de QTS

A seguir, apresento os resultados do teste realizado para validar as operações matemáticas básicas implementadas no sistema. Além das operações de Adição, Subtração, Multiplicação e Divisão, há também um teste para verificar o tratamento da exceção no caso de divisão por zero, assegurando que o sistema lida corretamente com essa situação.

### 1. Resultado do teste para a operação de Adição:

Este teste verifica a precisão do sistema ao realizar a soma de dois números. O objetivo é garantir que o cálculo da adição seja feito corretamente, conforme as regras matemáticas esperadas.

![Resultado do teste de Adição](imgs-testes-unitarios/soma.png)

### 2. Resultado do teste para a operação de Subtração:

O teste de subtração avalia se o sistema consegue subtrair dois números corretamente, levando em conta os números positivos e negativos, respeitando a lógica da operação.

![Resultado do teste de Subtração](imgs-testes-unitarios/subtracao.png)

### 3. Resultado do teste para a operação de Multiplicação:

Este teste assegura que o sistema calcula corretamente o produto entre dois números, sem erros de arredondamento ou de cálculo, independentemente de serem números inteiros ou decimais.

![Resultado do teste de Multiplicação](imgs-testes-unitarios/multiplicacao.png)

### 4. Resultado do teste para a operação de Divisão:

Neste teste, a divisão entre dois números é verificada para garantir que o cálculo seja preciso. O sistema deve realizar a operação corretamente, levando em consideração tanto inteiros quanto decimais.

![Resultado do teste de Divisão](imgs-testes-unitarios/divisao.png)

### 5. Resultado do teste de Divisão por Zero:

A divisão por zero foi tratada com uma exceção, conforme esperado. Esse teste assegura que o sistema lide corretamente com essa operação inválida, gerando uma mensagem de erro ou outro comportamento adequado.

![Resultado do teste de Divisão por zero](imgs-testes-unitarios/divisao_por_zero.png)
