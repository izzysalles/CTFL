
**Nível:** mesma coisa que falar de uma etapa, um momento dentro de uma sprint **(QUANDO)**.
- Relacionado a outras atividades dentro do SDLC

**Tipo:** tipo de teste aplicável na situação **(O QUE)**.

##### Níveis de Teste

Teste de **C**omponente (unidade);
Teste de **I**ntegração de Componentes (integração de unidades);
- Depende muito de abordagens como **bottom-up, top-down ou big-bang** (teste final e sem simulador).

![[Pasted image 20240528150245.png]]
 > The top-down integration testing works through **significant to minor components**, whereas the bottom-up approach works through **small to essential components** or modules.
 
 Teste de Integração de **Sistemas** (API);
 Teste de **Aceite** (necessidade de negócio do usuário).

> **CISA**

**Teste Alfa e Beta:** teste feito pelo cliente para experimentar o produto antecipadamente, no **Alfa** os produtos necessários para o teste são **fornecidos pela empresa** (máquinas e etc). No **Beta** o software é disponibilizado para teste na **máquina do próprio usuário**. 

##### Tipos de Teste

Existem muitos tipos de teste que podem ser aplicados em projetos, para a CTFL são abordados:

**Teste Funcional:** verifica a integridade funcional, se o componente ou sistema executa o que foi pedido (integridade, correção e adequação).

**Teste Não Funcional:** avalia atributos que não sejam características funcionais de um componente ou sistema, testa o quão bem um sistema se comporta, este tipo de teste é independente do negócio. **Podem acontecer desde o início do ciclo de vida do software.**

**Teste Caixa-Preta:** baseado em **documentações/especificações**, o principal objetivo é verificar o comportamento do sistema em relação as suas especificações.

**Teste Caixa-Branca:** teste de baixo nível, onde se olha o **código** para ver as regras nele presentes e checar os dados. Escrever testes baseados no código. 

**Teste de Confirmação:** repetição dos testes anteriores ^ (retestar uma funcionalidade após encontrar um defeito).

> Todos tipos de teste podem acontecer em qualquer nível!

##### ISO/IEC 25010

Fornece a classificação das **características não funcionais** de qualidade de software:

- **U**sabilidade;
- **C**ompatibilidade;
- **C**onfiabilidade;
- **E**ficiência;
- Capacidade de **M**anutenção;
- **P**ortabilidade
- **S**egurança

> **UCCEMPS**

**Teste de Regressão:** checa se funcionalidades antigas continuam funcionando, testando tudo de novo. É aconselhável realizar primeiro uma **análise de impacto** para otimizar a extensão do teste de regressão.

**Teste de Manutenção:** um dos testes mais realizados, existem diversos tipos de manutenção como corretivas, adaptativas ou performance. A **análise de impacto** também é levada em consideração.

