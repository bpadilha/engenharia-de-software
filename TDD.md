# Métodos Ágeis – TDD

O desenvolvimento de software é um trabalho exigente e passível de falhas. Nas abordagens tradicionais de programação a maioria dos erros acontecem durante a fase de compilação. Estas abordagens levam a que bugs sejam detectados numa fase posterior, muitas das vezes quando a aplicação está a ser usada pelo user.

É neste contexto que surge o **Test Driven Development (TDD)**, que é uma técnica de desenvolvimento de software, muitas vezes associada a metodologias ágeis, que consiste em pequenas iterações de desenvolvimento onde o caso de teste, que cobre uma funcionalidade da aplicação, é escrito antes de ser implementada a própria funcionalidade.

O **Test Driven Development (TDD)** ou em português Desenvolvimento Orientado por Testes -  é uma técnica de desenvolvimento de software que se relaciona com o conceito de verificação e validação e se baseia em um ciclo curto de repetições.

Mais do que simplesmente testar seu código, **TDD** é uma filosofia, uma cultura, sendo considerado um novo jeito de programar, sendo esta uma técnica empregada no desenvolvimento de softwares baseado em testes que são escritos antes mesmo do código de produção.

As técnicas de teste de software para o desenvolvimento de produtos, muito embora muitas empresas não as utilizarem alegando o atraso, o tempo ou o custo para esta tarefa, vem sendo indicadas pelas pesquisas como grande ajuda na garantia de qualidade do software.

Basicamente o TDD se baseia em pequenos ciclos de repetições, onde para cada funcionalidade do sistema um teste é criado antes. Este novo teste criado inicialmente falha, já que ainda não temos a implementação da funcionalidade em questão e, em seguida, implementamos a funcionalidade para fazer o teste passar.


Os Métodos Ágeis, ou **Desenvolvimento Ágil de Software (DAS)**, tem se popularizado, na última década, por meio de métodos como **Extreme Programming (XP)** e **Scrum** e isso fez com que fossem aplicadas no desenvolvimento de sistemas computacionais de diversos tamanhos, complexidades técnica e de domínio, e de rigor quanto à confiabilidade.

A necessidade de processos de desenvolvimento de software que sejam mais rigorosos e que possuam uma quantidade adequada de modelagem e documentação, se evidencia, em especial, no que concerne ao projeto arquitetural, com o objetivo de garantir maior qualidade no seu resultado final.  A confiabilidade pode ser alcançada adicionando elementos de tratamento de exceções às fases iniciais do processo de desenvolvimento e à reutilização de componentes.

O tratamento de exceções tem sido uma técnica muito utilizada na depuração de erros em sistemas de software.  

O TDD transforma o desenvolvimento, pois deve-se primeiro escrever os testes, antes de implementar o sistema. Os testes são utilizados para facilitar no entendimento do projeto, segundo Freeman os testes são usados para clarear a ideia em relação ao que se deseja em relação ao código. Segundo Kent Beck apud Freeman “Finalmente, consegui separar o projeto lógico do físico. Sempre me disseram para fazer isso, mas nunca ninguém tinha explicado como”, o TDD é a forma de se fazer isso. A criação de teste unitários ou de componentes é parte crucial para o TDD. Segundo Presmann, “Os componentes individuais são testados para garantir que operem corretamente. Cada componente é testado independentemente, sem os outros componentes de sistema. Os componentes podem ser entidades simples, tais como funções ou classes de objetos, ou podem ser grupos coerentes dessas entidades”.

Mas não é só o teste unitário que vai trazer o sucesso a aplicação, é necessário testar o sistema como um todo. De acordo com Sommerville, “Os componentes são integrados para compor o sistema. Esse processo está relacionado com a busca de erros que resultam das interações não previstas entre os componentes”.


Um sistema é um conjunto de unidades integradas e por este motivo é importante os testes unitários para ver se no micromundo tudo funciona. Mas, também temos de testar a integração, ou seja, ao integrar dois ou mais componentes, devemos realizar testes para verificar se a integração funciona, uma vez que erros podem ocorrer, justamente no processo de montagem/integração de componentes.

O benefício em utilizar o TDD, em primeira instância, é porque torna o processo mais confiável, com redução de custos, pois como os testes são criados antes do processo de desenvolvimento, conseguimos testar constantemente.
Outro ponto é que se os testes foram criados, isso quer dizer que foram entendidas as regras de negócio durante a fase de desenvolvimento dos testes unitários.
Além disso, evita retrabalho da equipe, que ao final reduz custo e tem maior chance de sucesso.

O Ciclo do TDD é simples: **criamos um teste -> Fazemos a codificação para passar no teste -> Refatoramos nosso código**, conforme figura a seguir:

![Ciclo TDD](https://arquivo.devmedia.com.br/artigos/Fabio_Gomes_Rocha/TDD/TDD_1.jpg)

O processo de desenvolvimento de software segundo o TDD, também conhecido por ciclo Red/Green/Refactor, resume-se à execução repetida dos passos: escrever um teste unitário que falhe antes de escrever qualquer código funcional (Red); escrever o código funcional até que o teste unitário passe (Green); no final, caso seja necessário, efectuar uma reestruturação do código, remover as redundâncias e melhorando a própria estrutura do mesmo, assegurando que os testes unitários continuam todos a ter sucesso (Refactor).  O TDD recomenda ainda a automatização dos testes de forma que o seu código seja sempre compilado e executado como parte integrante do processo normal de builds. Desta forma, garante-se que a adição de uma nova funcionalidade ou a reestruturação de código não quebram as funcionalidades já implementadas.

Para que funcione, necessário que seja efetuado todo o Ciclo de desenvolvimento Red, Green, Refactor:

*	Escrevemos um Teste que inicialmente não passa **(Red)**
* Adicionamos uma nova funcionalidade do sistema
*	Fazemos o Teste passar **(Green)**
*	Refatoramos o código da nova funcionalidade **(Refactoring)**
*	Escrevemos o próximo Teste

![Ciclo TDD](https://arquivo.devmedia.com.br/marketing/img/18533/TDD.png)

O teste visa auxiliar a codificação, reduzindo consideravelmente os problemas na fase de desenvolvimento.

A indicação é de que no TDD, o projeto de teste unitário ocorra antes da fase de codificação/implementação.

O Teste antes da codificação, ou test-first, segundo Sommerville, “a escrita de testes primeiro define implicitamente tanto uma interface como uma especificação do comportamento para a funcionalidade que está sendo desenvolvida”.

Ao criar o teste antes de implementar a unidade, são reduzidos problemas como mal entendimento de requisitos ou interfaces.

O desenvolvedor, para implementar os testes iniciais, deve compreender com detalhes a especificação do sistema e as regras de negócio, só assim, será possível escrever testes para o sistema.

Importante frisar que, não adianta criar testes que não validem o código como um todo para reduzir o tempo, é necessário criar testes para o conjunto completo de unidades, só assim o TDD vai funcionar como deve, devendo fornecer uma cobertura completa aos testes.

Além disso, os testes devem seguir o modelo **F.I.R.S.T.**

* **F** (Fast) - Rápidos: devem ser rápidos, pois testam apenas uma unidade;
* **I** (Isolated) - Testes unitários são isolados, testando individualmente as unidades e não sua integração;
* **R** (Repeateble) - Repetição nos testes, com resultados de comportamento constante;
* **S** (Self-verifying) - A auto verificação deve verificar se passou ou se deu como falha o teste;
* **T** (Timely) - O teste deve ser oportuno, sendo um teste por unidade.

Entre os vários motivos para o uso do TDD, podemos afirmar que temos diversos ganhos com esta estratégia, tais quais:

*	Feedback rápido sobre a nova funcionalidade e sobre as outras funcionalidades existentes no sistema
*	Código mais limpo, já que escrevemos códigos simples para o teste passar
*	Segurança no Refactoring pois podemos ver o que estamos ou não afetando
*	Segurança na correção de bugs
*	Maior produtividade já que o desenvolvedor encontra menos bugs e não desperdiça tempo com depuradores
*	Código da aplicação mais flexível, já que para escrever testes temos que separar em pequenos "pedaços" o nosso código, para que sejam testáveis, ou seja, nosso código estará menos acoplado.

A médio prazo (e dependendo do sistema a curto prazo) este tempo de desenvolvimento com TDD é menor que o tempo de manutenção corrigindo bugs e mesmo para adicionar funcionalidades novas. Isto devido, resumidamente, a:

*	Confiança do desenvolvedor na correção de bugs, pois qualquer passo errado será mostrado pelos testes
*	Tempo de desenvolvimento menor na adição de funcionalidades, já que o sistema é mais flexível e o código mais limpo
*	Menor tempo do desenvolvedor ao corrigir bugs após aquelas incessantes brigas com o pessoal de qualidade depois da famosa frase "Mas na minha máquina funciona!"
*	Possibilidade de Integração Contínua, com builds automáticos e feedbacks rápidos de problemas.

As vantagens da utilização do TDD superam fortemente as desvantagens. O argumento de que é necessário implementar mais código do que nas abordagens tradicionais não chega para superar as vantagens de obter um produto final com menos bugs e com períodos de manutenção mais curtos.
O TDD não será certamente a solução para todos os problemas, contudo, ajuda os programadores a melhorar a forma como programam, entregando soluções mais fiáveis, modulares, flexíveis, de mais fácil manutenção indo ao encontro dos requisitos do Cliente.

## Referências

**BARTIÉ, Alexandre**. **Garantia de qualidade de software**. Rio de Janeiro: Campus, 2002.

**FREEMAN, Steve. Pryce, Nat**. **Desenvolvimento de Software Orientado a objetos, Guiado por Testes**. Rio de Janeiro: Alta Books, 2012.

**PRESSMAN, Roger S**. **Engenharia de Software: Uma abordagem Profissional**. Porto Alegre: Bookman, 2011.

**SILVEIRA, Paulo et al**. **Introdução à arquitetura e design de software: uma visão sobre a plataforma Java**. Rio de Janeiro: Campus, 2012.

**SOMMERVILLE, Ian**. **Engenharia de software**. São Paulo:Person, 2010.
