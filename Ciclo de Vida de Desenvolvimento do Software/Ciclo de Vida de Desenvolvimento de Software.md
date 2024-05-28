
Representação abstrata e de alto nível do processo de desenvolvimento de software.

**Sigla em PT-BR:** CVDS 
**Sigla em ENG:** SDLC

##### Exemplos de modelos

> **Modelos de desenvolvimento sequencial:** cascata e em V.
> **Modelos de desenvolvimento iterativo:** modelo espiral e prototipagem.
> **Modelos de desenvolvimento incremental:** processo unificado racional (RUP).

**Atenção: o RUP é incremental, porém não é ágil!**

##### Métodos Ágeis 

**01.** Desenvolvimento orientado por testes de aceite (ATDD)
**02.** Desenvolvimento orientado pelo comportamento (BDD)
**03.** Domain-driven design (BDD)
**04.** Extreme programming (XP)
**05.** Feature-driven development (FDD)
**06.** Kanban, Lean IT, Scrum e TDD

##### Impacto dos CVDS nos testes

A escolha do ciclo de vida, tem impacto sobre:

- **Escopo** e **cronograma** as atividades de teste;
- Nível de **detalhamento da documentação** de teste;
- Escolha de **técnicas de teste** e da **abordagem de teste**;
- Extensão da automação de testes;
- O papel e responsabilidades de um testador.

Nos modelos de **desenvolvimento sequencial**, nas fases iniciais, os testadores normalmente participam de **revisões de requisitos, da análise de testes e do projeto de testes**.

> Os testes dinâmicos (código executável) não podem ser realizados no início do SDLC.

**Para cada atividade de desenvolvimento de software, há uma atividade de teste correspondente**

> TDD, BDD e ATDD seguem a abordagem shift-left, pois os teses são definidos antes do código

##### TDD

Testes são escritos primeiro e o código é feito para satisfazer os testes.

##### ATDD (Desenvolvimento Orientado por Testes de Aceite)

Foco no comportamento descrito pelo cliente.

##### BDD (Desenvolvimento Orientado pelo Comportamento)

Comportamentos de teste escritos de forma simples: Dado/Quando/Então, após isso os testes são traduzidos em exxecutáveis. 