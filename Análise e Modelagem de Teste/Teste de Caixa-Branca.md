
Técnicas relacionadas ao código:
- Teste de instruções;
- Teste de ramificação.

Existem mais técnicas, úteis em diferentes situações, mas para CTFL apenas as duas acima serão cobradas.

> Ao fazer o **teste de ramificação**, você faz junto o **teste de instrução**, mas o contrário não é possível.

- **Ponto Forte:** Toda a implementação do software é levada em conta durante o teste e facilita na detecção de defeitos quanto a especificação do software;
- **Ponto Fraco:** Se o software não implementar um ou mais requisitos, o teste de caixa-branca não pode detectar defeitos resultantes ausentes.

> As técnicas de caixa branca podem ser usadas em **testes estáticos**.

> Adequado para **revisar códigos** que ainda não estão prontos para execução.

##### Teste de Instrução e Cobertura 

Tem como objetivo projetar casos de teste que exercitem as instruções do código até que um nível aceitável de cobertura seja alcançado.

> A **cobertura** é **medida** como o número de instruções exercidas pelos casos de teste dividido pelo número total de instruções executáveis no código. Expressa em porcentagem. 

**Teste muito simplório, pois verifica apenas se passou por cada linha de código.**

Não garante que toda lógica de decisão tenha sido testada, pois pode não executar todas as decisões presentes no código (else).

##### Teste de Ramificação

No teste de transição, os itens de cobertura são ramificações e o objetivo é modelar casos de teste para executar ramificações no código até que um nível aceitável de cobertura. (if/else/for/switch/loop)

A **cobertura é medida** como o número de ramificações exercidas pelos casos de teste dividido pelo número total de ramificações e é expressa em %.

> Não vai detectar todos os defeitos, vai cobrir a cobertura de instrução, mas pode não detectar defeitos que exijam a execução de um caminho específico do código.

![[Pasted image 20240602214420.png]]

![[Pasted image 20240602215222.png]]Calcular ambos os blocos, mas utilizar o maior.

> **Instrução <= Ramificação**
> **100% de Ramificação = 100% de Instrução** 