
## Relatório Detalhado dos Testes de API da Calculadora

Os testes realizados têm como objetivo verificar se a API da calculadora está funcionando corretamente para as operações de **soma**, **subtração**, **multiplicação** e **divisão**, além de validar o tratamento de exceções, especialmente no caso de uma **divisão por zero**.

### 1. **Resultado do teste para a operação de Soma**

Este teste verifica se a operação de soma entre dois números retorna o resultado esperado. O cálculo é realizado a partir dos parâmetros `numero1` e `numero2` passados na URL da requisição.

![Resultado do teste de Adição](imgs-testes-unitarios/soma.png)

### 2. **Resultado do teste para a operação de Subtração**

O teste de subtração verifica se a diferença entre dois números é calculada corretamente. Da mesma forma que a soma, os parâmetros `numero1` e `numero2` são fornecidos pela URL da requisição.

![Resultado do teste de Subtração](imgs-testes-unitarios/subtracao.png)

### 3. **Resultado do teste para a operação de Multiplicação**

Este teste valida o cálculo da multiplicação entre dois números fornecidos na requisição. A operação deve retornar o produto dos números passados.

![Resultado do teste de Multiplicação](imgs-testes-unitarios/multiplicacao.png)

### 4. **Resultado do teste para a operação de Divisão**

Este teste valida a operação de divisão entre dois números, com a verificação de que o sistema calcula corretamente o quociente entre os números fornecidos na URL da requisição.

![Resultado do teste de Divisão](imgs-testes-unitarios/divisao.png)

### 5. **Resultado do teste de Divisão por Zero**

Este teste valida a operação de **divisão por zero**. O objetivo é verificar se o sistema lida corretamente com o cenário onde o divisor é igual a zero, uma vez que essa operação não é definida matematicamente. O teste assegura que o sistema reconhece esse caso e realiza o tratamento adequado, interrompendo a operação de divisão quando o divisor é zero.

![Resultado do teste de Divisão por Zero](imgs-testes-unitarios/divisao_por_zero.png)

