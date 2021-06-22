# Design Pattern

## Padrão de projeto de software

Em Engenharia de Software, um padrão de desenho (portugues europeu) ou padrão de projeto (portugues brasileiro) (do ingles **design pattern**) é uma solução geral para um problema que ocorre com frequencia dentro de um determinado contexto no projeto de software. Um padrão de projeto não é um projeto finalizado que pode ser diretamente transformado em código fonte ou de máquina, ele é uma descrição ou modelo (template) de como resolver um problema que pode ser usado em muitas situações diferentes. padrões são melhores práticas formalizadas que o programador pode usar para resolver problemas comuns quando projetar uma aplicação ou sistema. padrões de projeto orientados a objeto normalmente mostram relacionamentos e interações entre classes ou objetos, sem especificar as classes ou objetos da aplicação final que estão envolvidas. padrões que implicam *orientação a objetos* ou estado mutável mais geral, não são tão aplicáveis em *linguagens de programação funcional*.

Padrões de projeto residem no domínio de módulos e interconexões. Em um nível mais alto há padrões arquiteturais que são maiores em escopo, usualmente descrevendo um padrão global seguido por um sistema inteiro.[1]

As características obrigatórias que devem ser atendidas por um padrão de projeto é composto basicamente por 4 (quatro) elementos que são:

...

- Nome do padrão;
- Problema a ser resolvido;
- Solução dada pelo padrão; e
- Consequencias.
- Os padrões de projeto:
...

- visam facilitar a reutilização de soluções de desenho - isto é, soluções na fase de projeto do software
- estabelecem um vocabulário comum de desenho, facilitando comunicação, documentação e aprendizado dos sistemas de software.

## Hist�ria

O arquiteto Christopher Alexander, em seus livros (1977/1979) Notes on the Synthesis of Form, The Timeless Way of Building e A Pattern Language, estabelece que um padrão deve ter, idealmente, as seguintes características:

- **Encapsulamento:** um padrão encapsula um problema ou solução bem definida. Ele deve ser independente, específico e formulado de maneira a ficar claro onde ele se aplica.
- **Generalidade:** todo padrão deve permitir a construção de outras realizações a partir deste padrão.
- **Equilíbrio:** quando um padrão é utilizado em uma aplicação, o equilíbrio dá a razão, relacionada com cada uma das restrições envolvidas, para cada passo do projeto. Uma análise racional que envolva uma abstração de dados empíricos, uma observação da aplicação de padrões em artefatos tradicionais, uma série convincente de exemplos e uma análise de soluções ruins ou fracassadas pode ser a forma de encontrar este equilibrio.
- **Abstração:** os padrões representam abstrações da experiência empirica ou do conhecimento cotidiano.
- **Abertura:** um padrão deve permitir a sua extensão para níveis mais baixos de detalhe.
- **Combinatoriedade:** os padrões são relacionados hierarquicamente. padrões de alto nível podem ser compostos ou relacionados com padrões que endereçam problemas de nível mais baixo.

Além da definição das características de um padrão, Alexander definiu o formato que a descrição de um padrão deve ter. Ele estabeleceu que um padrão deve ser descrito em cinco partes:

- **Nome:** uma descrição da solução, mais do que do problema ou do contexto;
- **Exemplo:** uma ou mais figuras, diagramas ou descrições que ilustrem um protótipo de aplicação;
- **Contexto:** a descrição das situações sob as quais o padrão se aplica;
- **Problema:** uma descrição das forças e restrições envolvidos e como elas interagem;
- **Solução:** relacionamentos estáticos e regras dinâmicas descrevendo como construir artefatos de acordo com o padrão, frequentemente citando variações e formas de ajustar a solução segundo as circunstâncias. Inclui referências a outras soluções e o relacionamento com outros padrões de nível mais baixo ou mais alto.

Os patterns de Alexander procuravam prover uma fonte de ideias provadas para indivíduos e comunidades para serem usadas em construções, mostrando assim o quanto belo, confortável e flexível os ambientes podem ser construídos.

Em 1987, a partir dos conceitos criados por Alexander, os programadores Kent Beck e Ward Cunningham propuseram os primeiros padrões de projeto para a área da ciência da computação. Em um trabalho para a conferência OOPSLA, eles apresentaram alguns padrões para a construção de aplicações comerciais em linguagem Smalltalk.[5] Nos anos seguintes Beck, Cunningham e outros seguiram com o desenvolvimento destas ideias.

Porém, o movimento ao redor de padrões de projeto só ganhou popularidade em 1995 quando foi publicado o livro Design Patterns: Elements of Reusable Object-Oriented Software. Os autores desse livro, Erich Gamma, Richard Helm, Ralph Johnson e John Vlissides, são conhecidos como a "Gangue dos Quatro" (Gang of Four) ou simplesmente "GoF".

Posteriormente, vários outros livros do estilo foram publicados, merecendo destaque Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development, que introduziu um conjunto de padrões conhecidos como GRASP (General Responsibility Assignment Software Patterns).

## Características de um padrão de projeto

Embora um padrão seja a descrição de um problema, de uma solução genérica e sua justificativa, isso não significa que qualquer solução conhecida para um problema possa constituir um padrão, pois existem características obrigatárias que devem ser atendidas pelos padrões:[3]

1. Devem possuir um NOME, que descreva o problema, as soluções e conseqçãncias. Um nome permite definir o vocabulário a ser utilizado pelos projetistas e desenvolvedores em um nível mais alto de abstração.

2. Todo padrão deve relatar de maneira clara a qual (is) PROBLEMA(s) ele deve ser aplicado, ou seja, quais são os problemas que quando inserido em um determinado contexto o padrão conseguirá resolve-lo.Alguns podendo exigir pré-condições.

3. Solução descreve os elementos que compõem o projeto, seus relacionamentos, responsabilidades e colaborações. Um padrão deve ser uma SOLUçãO concreta, ele deve ser exprimido em forma de gabarito (algoritmo) que, no entanto pode ser aplicado de maneiras diferentes.

4. Todo padrão deve relatar quais são as suas CONSEQUÊNCIAS para que possa ser analisada a solução alternativa de projetos e para a compreensão dos benefícios da aplicação do projeto.

não pode ser considerado um padrão de projeto trecho de códigos específicos, mesmo que para o seu criador ele reflita um padrão, que soluciona um determinado problema, porque os padrões devem estar a um nível maior de abstração e não limitado a recursos de programação. Um padrão de projeto nomeia, abstrai e identifica os aspectos chaves de uma estrutura de projeto comum para torna-la útil para a criação de um projeto orientado a objetos reutilizável.[3]

## padrões GoF ('Gang of Four')

De acordo com o livro: "padrões de Projeto: soluções reutilizáveis de software orientado a objetos", os padrões "GoF" são divididos em 24 tipos. Em função dessa grande quantidade de padrões, foi necessário classificá-los de acordo com as suas finalidades.

São 3 as classificações/famílias:

- **padrões de criação:** Os padrões de criação são aqueles que abstraem e/ou adiam o processo criação dos objetos. Eles ajudam a tornar um sistema independente de como seus objetos são criados, compostos e representados. Um padrão de criação de classe usa a herança para variar a classe que é instanciada, enquanto que um padrão de criação de objeto delegará a instanciação para outro objeto. Os padrões de criação tornam-se importantes é medida que os sistemas evoluem no sentido de dependerem mais da composição de objetos do que a herança de classes. O desenvolvimento baseado na composição de objetos possibilita que os objetos sejam compostos sem a necessidade de expor o seu interior como acontece na herança de classe, o que possibilita a definição do comportamento dinamicamente e a ênfase desloca-se da codificação de maneira rígida de um conjunto fixo de comportamentos, para a definição de um conjunto menor de comportamentos que podem ser compostos em qualquer número para definir comportamentos mais complexos. Há dois temas recorrentes nesses padrões. Primeiro todos encapsulam conhecimento sobre quais classes concretas são usadas pelo sistema. Segundo ocultam o modo como essas classes são criadas e montadas. Tudo que o sistema sabe no geral sobre os objetos é que suas classes são definidas por classes abstratas. Consequentemente, os padrões de criação dão muita flexibilidade no que é criado, quem cria, como e quando é criado. Eles permitem configurar um sistema com objetos �produto� que variam amplamente em estrutura e funcionalidade. A configuração pode ser estática (isto é, especificada em tempo de compilação) ou dinâmica (em tempo de execução).

- **padrões estruturais:** Os padrões estruturais se preocupam com a forma como classes e objetos são compostos para formar estruturas maiores. Os de classes utilizam a herança para compor interfaces ou implementações, e  os de objeto descrevem maneiras de compor objetos para obter novas funcionalidades. A flexibilidade obtida pela composição de objetos provém da capacidade de mudar a composição em tempo de execução o que não é possível com a composição estática (herança de classes).
- **padrões comportamentais:** Os padrões de comportamento se concentram nos algoritmos e atribuições de responsabilidades entre os objetos. Eles não descrevem apenas padrões de objetos ou de classes, mas também os padrões de comunicação entre os objetos. Os padrões comportamentais de classes utilizam a herança para distribuir o comportamento entre classes, e os padrões de comportamento de objeto utilizam a composição de objetos em contrapartida a herança. Alguns descrevem como grupos de objetos que cooperam para a execução de uma tarefa que não poderia ser executada por um objeto sozinho.

Padrões "GoF" organizados nas suas 3 classificações/famílias:

- Padrões de criação
  - Abstract Factory
  - Object pool
  - Builder
  - Factory Method
  - Prototype
  - Singleton

- Padrões estruturais
  - Private class data
  - Adapter
  - Bridge
  - Composite
  - Decorator
  - Fa�ade (ou Facade)
  - Business Delegate
  - Flyweight
  - Proxy

- padrões comportamentais[3]
  - Chain of Responsibility
  - Command
  - Interpreter
  - Iterator
  - Mediator
  - Memento
  - Observer
  - State
  - Strategy
  - Template Method
  - Visitor

Existem outros critérios de classificação dos padrões de projeto:

- **Finalidade:** reflete o que um padrão faz.
- **Escopo:** especifica se o padrão é aplicado à classe ou objeto.
- **padrões com escopo de classe:** utilizam a hierarquia para compor ou variar os objetos, mantendo a capacidade do sistema de se flexibilizar. Se realizarmos uma comparação com o outro tipo de classificação isso costuma acontecer quando se trata de um padrão de criação.
- **padrões com escopo de objeto:** encontrados no relacionamento entre os objetos definidos em tempo de execução. Realizando uma comparação com o outro tipo de classificação vemos que esses padrões aparecem muito nos padrões estruturais e comportamentais.

[Artigo original](https://pt.wikipedia.org/wiki/Padr%C3%A3o_de_projeto_de_software)
