
## Relatório Detalhado dos Testes de API da Calculadora

Os testes realizados têm como objetivo verificar se a API da calculadora está funcionando corretamente para as operações de **soma**, **subtração**, **multiplicação** e **divisão**, além de validar o tratamento de exceções, especialmente no caso de uma **divisão por zero**.

### 1. **Resultado do teste para a operação de Soma**

Este teste verifica se a operação de soma entre dois números retorna o resultado esperado. O cálculo é realizado a partir dos parâmetros `numero1` e `numero2` passados na URL da requisição.

- **Requisição:** `GET /soma?numero1=10&numero2=5`
- **Resultado Esperado:** 10 + 5 = 15
- **Status da Resposta:** 200 OK
- **Resposta do Corpo:** `{"resultado":15.0}`

![Resultado do teste de Adição](imgs-testes-unitarios/soma.png)

### 2. **Resultado do teste para a operação de Subtração**

O teste de subtração verifica se a diferença entre dois números é calculada corretamente. Da mesma forma que a soma, os parâmetros `numero1` e `numero2` são fornecidos pela URL da requisição.

- **Requisição:** `GET /subtracao?numero1=10&numero2=5`
- **Resultado Esperado:** 10 - 5 = 5
- **Status da Resposta:** 200 OK
- **Resposta do Corpo:** `{"resultado":5.0}`

![Resultado do teste de Subtração](imgs-testes-unitarios/subtracao.png)

### 3. **Resultado do teste para a operação de Multiplicação**

Este teste valida o cálculo da multiplicação entre dois números fornecidos na requisição. A operação deve retornar o produto dos números passados.

- **Requisição:** `GET /multiplicacao?numero1=10&numero2=5`
- **Resultado Esperado:** 10 * 5 = 50
- **Status da Resposta:** 200 OK
- **Resposta do Corpo:** `{"resultado":50.0}`

![Resultado do teste de Multiplicação](imgs-testes-unitarios/multiplicacao.png)

### 4. **Resultado do teste para a operação de Divisão**

Este teste valida a operação de divisão entre dois números, com a verificação de que o sistema calcula corretamente o quociente entre os números fornecidos na URL da requisição.

- **Requisição:** `GET /divizao?numero1=10&numero2=5`
- **Resultado Esperado:** 10 / 5 = 2
- **Status da Resposta:** 200 OK
- **Resposta do Corpo:** `{"resultado":2.0}`

![Resultado do teste de Divisão](imgs-testes-unitarios/divisao.png)

### 5. **Resultado do teste de Divisão por Zero**

Este teste tem como objetivo verificar se a aplicação trata corretamente o caso de divisão por zero. Como a divisão por zero é indefinida, a API deve retornar uma mensagem de erro apropriada com o código de status **400 BadRequest**.

- **Requisição:** `GET /divizao?numero1=10&numero2=0`
- **Resultado Esperado:** Erro, pois não é possível dividir por zero.
- **Status da Resposta:** 400 BadRequest
- **Resposta do Corpo:** `Erro: Não é permitido dividir por zero.`

![Resultado do teste de Divisão por Zero](imgs-testes-unitarios/divisao_por_zero.png)

---

### Considerações Finais:

Os testes mostraram que todas as operações da calculadora funcionam conforme o esperado:

1. As operações de **soma**, **subtração**, **multiplicação** e **divisão** retornam os resultados corretos.
2. O **tratamento de erro** para divisão por zero está implementado corretamente, retornando um erro com a mensagem adequada e o status **400 BadRequest**.

Esses testes asseguram que a API da calculadora está funcionando corretamente e tratando as exceções de maneira adequada.
