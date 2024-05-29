
O teste não é executado ao contrário do dinâmico. Neste teste documentos, código ou até diagramas são analisados e revisados **manualmente**. Apenas na **análise estática usamos ferramenta.**

>**Objetivo:** melhorar a qualidade, antecipar defeitos, analisar legibilidade, integridade, testabilidade e consistência. 

Pode ser aplicado tanto para **verificação** quanto para **validação**.

**Definição de pronto (ready):** sinalização de algo pronto para teste.

A **Análise Estática**, pode identificar problemas **antes** dos **testes dinâmicos**, o que gera **economia** para o projeto. (Programas feitos para isso)

##### Produtos de Trabalho Examináveis por Teste Estático

> **Quase todos os produtos de trabalho podem ser examinados por meio de testes estáticos**, como: código-fonte, planos de teste, casos de teste, documentação, contratos.

Um produto **não apropriado** para teste estático seriam aqueles **difíceis de serem interpretados pelos seres humanos** e que **não podem ser analisados nem por ferramentas**. 

##### Teste Estático VS. Teste Dinâmico

- Alguns tipos de defeitos só podem ser encontrados por testes estáticos ou dinâmicos;
- Os testes estáticos encontram defeiros diretamente, já os **dinâmicos causam falhas e a partir delas os defeitos são determinados**;
- O teste dinâmico só pode ser aplicado a produtos executáveis;
- **Teste estático** pode ser usado para **medir características de qualidade que não dependem da execução do software**.

##### Defeitos Típicos

**Defeitos nos Requisitos**
Inconsistências, ambiguidades, contradições, omissões, imprecisões, duplicações.

**Defeitos de Projeto**
Estruturas de banco de dados ineficazes, modularização deficiente.

**Defeitos de Codificação**
Código duplicado, variáveis não declarada

**Desvio de padrões**
Falta de adesão às nomenclaturas no código

**Especificações Incorretas da Interface** (não é uma interface gráfica)

**Tipos específicos de vulnerabilidade de segurança**

**Imprecisões na cobertura da base de testes**
Testes ausentes para um critério de aceite
