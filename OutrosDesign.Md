# Design Patterns

## Outros Design Patterns

- Padrões arquiteturais
  - Interceptor
  - Mvc (Model View Controler)
  - Mvvm (Model View ViewModel)
  - Mvp (Model View Presenter)
  - n-tier (Arquitetura multicamada)
  - Specification
  - Publish�subscribe
  - Inversion of control (Inversão de controle)
  - Dependency Injection (Injeção de dependência)
  - Intercepting filter
  - Lazy loading
  - Mock object (objeto mock)
  - Method chaining
  - Unit of work
  - Delegation

## Padrões

Os padrões GRASP, sigla para General Responsibility Assignment Software Patterns (or Principles), consistem de um conjunto de práticas para atribuição de responsabilidades a classes e objetos em projetos orientados a objeto.

Os padrões GRASP (General Responsibility Assignment Software Patterns), são responsáveis pela descrição de princípios de fundamental importância para a atribuição de responsabilidades em projetos orientados a objetos, oferecendo um melhor desempenho do código, e trabalhando acerca de solucionar problemas, garantindo melhor interface do projeto.

Sendo assim, é importante sabermos que a qualidade do projeto orientado a objetos está diretamente relacionada com a distribuição dessas obrigações, que promovem a não sobrecarga de objetos já que ocorre nesse processo a delegação de atividades, ou seja, cada objeto terá uma função específica, de modo que, o que ele não souber fazer será repassado para o objeto que está mais preparado para fazer.

Todos esses padrões servem para a resolução de problemas comuns e bastante tópicos de desenvolvimento de software orientado a objeto. Portanto, tais técnicas apenas documentam e normatizam as práticas já consolidadas, testadas e conhecidas no mercado.

Os padrões GRASP estão mais como uma ferramenta mental ou uma filosofia de design, mas que ainda assim são úteis para o aprendizado e desenvolvimento de um bom design de software. Note que alguns padrões GoF implementam soluções correspondentes com padrões GRASP.

## Tipos de Padrões Grasp

Dentro do GRASP podemos encontrar vários padrões relacionados aqueles de caráter básicos e avançados.

- Padrões Básicos:
  - Information Expert (ver Especialista na Informação);
  - Creator (ver Factory Method);
  - High Cohesion (ver Coesão);
  - Low Coupling(ver Acoplamento);
  - Controller(ver Model-view-controller).

- Padrões Avançados:
  - Polymorphism (ver Polimorfismo);
  - Pure Fabrication;
  - Indirection (ver Indireção);
  - Protected Variations (ver Variações Protegidas).
  - Information Expert

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | É conhecido por ser o princípio fundamental para atribuir responsabilidade. | Qual é o princípio geral para a atribuição de responsabilidades aos objetos? | Atribua a responsabilidade ao especialista: a classe que tem as informações necessírias para assumir a responsabilidade. |  
 | Encapsulamento é mantido;  |
 | Fraco acoplamento (facilidade de manutenção); |
 | Alta coesão (objetos fazem tudo relacionado é sua própria informação). |

### Creator

 | O que é? | Possíveis Problemas | Solução | Benefícios  |
 | ---  | --- | --- | --- |
 | É uma das atividades mais comuns em um sistema de orientação a objetos. Atribui qual classe é responsável por criar os objetos. | Quem deve ser responsável por criar uma nova instância de uma classe? | Atribua à classe a responsabilidade de criar uma instância da outra classe. | Facilidade no desenvolvimento do projeto e compreensão. |

### High Cohesion

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | É um padrão avaliativo que tenta manter os objetos adequadamente focado, gerenciado e compreensável. | Como manter a complexidade sob controle?  |
 | Classes que fazem muitas tarefas não relacionadas são: |
 |  Mais difíceis de entender; |
 | Mais difíceis de manter e de reusar; |
 | são mais vulneráveis à mudança. |
 | Atribuir uma responsabilidade para que a coesão se mantenha alta. |
 | Melhor claridade e facilidade de compreensão do projeto; |
 | Simplificação da manutenção; |

### Low Coupling

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | É um padrão de avaliação, que determina como atribuir responsabilidades para apoiar. | Como prover baixa dependância entre classes, reduzir o impacto de mudanças e obter alta reutilização? | Atribui as responsabilidades de modo que o acoplamento entre classes permaneça baixo. |  
 | Menor dependância entre as classes; |
 | Mudar de uma classe que tem menor impacto sobre outras classes; |
 | Maior potencial de reutilização. |

### Controller

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | O padrão controlador atribui a responsabilidade de lidar com os eventos do sistema para uma classe que representa a um cenário de caso de uso do sistema global. | Quem deve ser o responsável por lidar com um evento de uma interface de entrada? | Atribuir responsabilidades para receber ou lidar com um evento do sistema para: |
 | Uma classe que representa todo o sistema ou subsistema; |
 | Uma classe que representa cenário de caso de uso (controlador de caso de uso ou de sessío). |
 | Diminui a sensibilidade da camada de apresentação em relação à lógica de domínio; |
 | Oportunidade para controlar o estado do caso de uso; |

### Polymorphism

 | O que é? | Possíveis problemas | Soluções | Benefícios |
 | ---  | --- | --- | --- |
 | É um princípio, no qual subclasses de uma superclasse são capazes de invocar métodos, que comportam-se de maneira diferente para cada classe derivada | Como tratar alternativas baseadas no tipo? Como criar componentes de software �plugáveis� ? | É aconselhável atribuir responsabilidades aos tipos usando operações polimórficas, isso quando alternativas ou comportamento relacionados variam com o tipo(classe). | Facilita a manutenção e inserção de um novo tipo de classe |

### Pure Fabrication

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | É uma classe que não representa um conceito no domínio do problema deve atender as seguintes características : baixo acoplamento e potencial de reutilização dos mesmos derivados. | Quando não se quer violar �Alta Coesão� e �Baixo Acoplamento� e o �Expert� não oferece soluções apropriadas que objeto deve ter responsabilidade? | Criar classes artificiais de baixa coesão e alto acoplamento(classes puras). | Apresenta vantagens como a criação de classes muito coesas e remove características não coesas das classes de domínios de negícios. |

### Indirection

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | Suporta baixo acoplamento(e reusa potencial)entre dois elementos, atribuindo a responsabilidade de mediação entre eles a um objeto intermediário. | Como evitar acoplamento direto entre duas ou mais classes?Como evitar baixo acoplamento e manter alta possibilidade de reuso através do desacoplamento de objetos? | A um objeto intermediário que faz mediação entre componentes e serviãos de modo que esses não sejam diretamente acoplados será atribuída a responsabilidade. | Visa atribuir responsabilidades, de modo que, olha para determinada responsabilidade determinando assim, as informações necessírias para cumpri-la e, consecutivamente, determina o local de armazenamento dessa informação. |

### Protected Variations

 | O que é? | Possíveis Problemas | Solução | Benefícios |
 | ---  | --- | --- | --- |
 | É um princípio básico na motivação de grande parte dos mecanismos e padrões na programação e no projeto, para fornecer flexibilidade e proteção contra variações. | Como projetar objetos,subsistemas e sistemas, de modo que, as variações ou instabilidades nesses elementos não sejam responsáveis por impactos indesejáveis em outros elementos? |
 | Identificar pontos de variação e atribuir responsabilidades para criar uma interface estável em volta desses pontos; |
 | Evitar o envio de mensagens a objetos muito distantes. |
 | Promove a contenção de variações e instabilidades, durante o projeto de objetos e sistemas, para que não ocorra a expansão de impactos a outros elementos. |

## Cr�ticas

Segundo alguns usuários, alguns "padrões de projeto" são apenas evidências de que alguns recursos estão ausentes em uma determinada linguagem de programação (Java ou C++ por exemplo). Nesta linha, Peter Norvig demonstra que 16 dos 23 padrões do livro 'Design Patterns' são simplificados ou eliminados nas linguagens Lisp ou Dylan, usando os recursos diretos destas linguagens.[9]

Segundo outros, excessos nas tentativas de fazer o código se conformar aos 'Padrões de Projeto' aumentam desnecessariamente a sua complexidade.[10]

### Bibliografia

- Christopher Alexander (1964). Notes on the Synthesis of Form. Estados Unidos: Harvard University Press. ISBN 0-674-62751-2
- Christopher Alexander (1979). The Timeless Way of Building. Estados Unidos: Oxford University Press. ISBN 0-19-502402-8
- Christopher Alexander (1977). A Pattern Language. Estados Unidos: Oxford University Press. ISBN 0-19-501919-9
- Craig Larman (2004). Applying UML and Patterns. An Introduction to Object-Oriented Analysis and Design and Iterative Development 1 ed. Estados Unidos: Prentice Hall. p. 736. ISBN 0-13-148906-2
- Gregor Hohpe, Bobby Woolf (2004). Enterprise Integration Patterns. Designing, Building, And Deploying Messaging Solutions 1 ed. Estados Unidos: Addinson-Wesley. p. 659. ISBN 0-321-20068-3
- Pablo Dall'Oglio (2007). PHP Programando com Orientação a Objetos. Inclui Design Patterns 1 ed. são Paulo: Novatec. p. 576. ISBN 978-85-7522-137-2
- Alexandre Altair de Melo e Mauricio G. F. Nascimento (2007). PHP Profissional. Aprenda a desenvolver sistemas profissionais orientados a objetos com padrões de projeto 1 ed. são Paulo: Novatec. p. 464. ISBN 978-85-7522-141-9

[Artigo original](https://pt.wikipedia.org/wiki/Padr%C3%A3o_de_projeto_de_software)
