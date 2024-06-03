
> Comportamento baseado em especificações, requisitos e funcionamento esperado do programa.

- Não se preocupa em saber a lógica interna e como funciona, mas sim se cumpre o esperado.

##### **Particionamento de Equivalência (EP)** 

Divide os dados em partições (grupos) de equivalência, de uma forma que todos sejam processados da mesma forma pelo objeto de teste. 

As partições podem ser **contínuas** (em sequência) ou **discretas** (variantes), **ordenadas** ou **não ordenada**, **finitas** ou **infinitas**.

As partições não devem se sobrepor de devem ser conjuntos não vazio (leva matemática em conta).

- **Partição Válida:** conteúdos válidos.
- **Partição Inválida:** conteúdos com valores inválidos, que não são permitidos ou rejeitados. 

> A cobertura é medida como o **número de partições executadas** por pelo menos um caso de teste, **dividido** pelo número **total de partições identificadas**. Expressa em %.

Muitos objetos de teste incluem **vários conjuntos de partições**. O critério mais simples no caso de vários conjuntos se chama **Each Choice Coverage** (ECC), esse tipo de cobertura **exige que os casos de teste executem cada partição pelo menos uma vez**.

> Usado em regras de negócio

###### Exemplo

Um sistema de ar condicionado central irá ligar o ar frio quando a temperatura estiver acima de 22C. Ligará o ar quente se abaixo de 16C. E ficará apenas ventilando em outras temperaturas.


15 | 16                                                                                                                                                22 | 23
________________________________
Quente                                                                Ventila                                                                        Frio


##### Análise de Valor Limite (BVA)

Complemento da **partição de equivalência**, mas ela precisa estar em uma **linha ordenada**.

- Situações com dois ou três valores limites, dependendo do risco.
- Dois pontos = menor risco | três pontos = maior risco.

###### Exemplo

Um cidadão é isento de imposto de renda se ganhar até 2 mil reais por mês. Os próximos 3 mil reais pagam 10% sobre toda a quantia. Acima disso, a aliquota será de 27,5%.

a) Quais seriam os testes por valores limites?
- dois valores;
- três valores.


2000  | 2001                                                                                                                          5000 | 5001
_______________________________________________
10%/quantia                                                                                                                        27,4%/quantia                      

1999 | 2000  | 2001                                                                                                    4999 | 5000 | 5001
_______________________________________________
isento                                                               10%/quantia                                              27,4%/quantia                      

b) Quais seriam os testes por particição de equivalência?

1500                                                                      4500                                                                      7500
_______________________________________________
isento                                                               10%/quantia                                              27,4%/quantia 


![[Pasted image 20240530215818.png]]

##### Tabela de Decisão

Usada para testar uma implementação de requisitos com diferentes combinações de condições.

> **Cobertura Máxima:** Número máximo de testes baseado em partição de equivalência, seria a **multiplicação das possibilidades** de cada condição.

> **Cobertura Minima:** Menor número de teste, **número de condições + 1**

![[Pasted image 20240530224311.png]]

##### Teste de Transição de Estado

Muito utilizado quando se tem um diagrama de transição de estado.

> Uma transição é iniciada por um evento que pode ser qualificado adicionalmente por uma condição de proteção.

**Tabela de estados:** suas linhas representam os estados e suas colunas representam eventos.

> **Cobertura de Todos os Estados:** Para atingir **100% de cobertura de todos os estados, os casos de teste devem garantir que todos os estados sejam visitados**. A cobertura é **medida como o número de estados visitados dividido pelo número total de estados e é expressa como porcentagem. 

> **Cobertura de Transições Válidas:** (0-switch) Para garantir 100% de transições válidas, os casos de teste devem executar todas as transições válidas. A cobertura é medida como **número de transições válidas executadas dividido pelo número total de transições válidas e é expressa em porcentagem**.

###### A **cobertura de todos os estados** é **mais fraca** do que a **cobertura de transições válidas**, porque pode ser obtida sem a execução de todas as transições.

![[Pasted image 20240602204234.png]]

**Estados:** 5 (elipses);
**Transições (0-switch):** 8 (setas) --> 8 testes no máximo 

![[Pasted image 20240602205001.png]]

**Transições Mínimo (0-switch):** 2 (setas) 