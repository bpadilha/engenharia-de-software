# Método Ágil TDD (Test Driven Development)

Apesar de muitas empresas ainda não utilizarem técnicas de teste de software para o desenvolvimento dos seus produtos, alegando o atraso, o tempo ou o custo para esta tarefa, as pesquisas indicam que os testes ajudam na garantia de qualidade do software.

## O que é o TDD?

O TDD é parte da metodologia XP e também utilizado em diversas outras metodologias, além de poder ser utilizada livremente.

O TDD transforma o desenvolvimento, pois deve-se primeiro escrever os testes, antes de implementar o sistema. Os testes são utilizados para facilitar no entendimento do projeto, segundo Freeman os testes são usados para clarear a ideia em relação ao que se deseja em relação ao código. Segundo Kent Beck apud Freeman “Finalmente, consegui separar o projeto lógico do físico. Sempre me disseram para fazer isso, mas nunca ninguém tinha explicado como”, o TDD é a forma de se fazer isso. A criação de teste unitários ou de componentes é parte crucial para o TDD.

Segundo Presmann, “Os componentes individuais são testados para garantir que operem corretamente. Cada componente é testado independentemente, sem os outros componentes de sistema. Os componentes podem ser entidades simples, tais como funções ou classes de objetos, ou podem ser grupos coerentes dessas entidades”.

## Qual o benefício em utilizar o TDD?

Em primeira instância, torna o processo mais confiável, mas reduz custos, pois desenvolvemos e já sabemos o erro, pois como os testes são criados antes do processo de desenvolvimento, conseguimos testar constantemente. Outro ponto é que se os testes foram criados, isso quer dizer que foram entendidas as regras de negócio durante a fase de desenvolvimento dos testes unitários.

Além disso, evita retrabalho da equipe, que ao final reduz custo e tem maior chance de sucesso.

O Ciclo do TDD é simples: criamos um teste -> Fazemos a codificação para passar no teste -> Refatoramos nosso código

![ Ciclo do TDD](https://arquivo.devmedia.com.br/artigos/Fabio_Gomes_Rocha/TDD/TDD_1.jpg)

Notemos aqui que o teste visa auxiliar a codificação, reduzindo consideravelmente os problemas na fase de desenvolvimento. No TDD é indicado que o projeto de teste unitário ocorra antes da fase de codificação/implementação.

O Teste antes da codificação, ou test-first, segundo Sommerville, “a escrita de testes primeiro define implicitamente tanto uma interface como uma especificação do comportamento para a funcionalidade que está sendo desenvolvida”.

Note que ao criar o teste antes de implementar a unidade, são reduzidos problemas como mal entendimento de requisitos ou interfaces, pois como criar um teste se eu não sei o que devo testar?

Neste caso o desenvolvedor, para implementar os testes iniciais, deve compreender com detalhes a especificação do sistema e as regras de negócio, só assim, será possível escrever testes para o sistema. Imagine o caso de querer testar um pneu criado para o carro, se não entendi que o pneu é redondo, por exemplo, criarei um teste para um pneu quadrado, não podendo ser realizado o teste. Desta forma, é de extrema importância, para o desenvolvedor, o entendimento dos requisitos do cliente. Além disso, não adianta criar testes que não validem o código como um todo para reduzir o tempo, é necessário criar testes para o conjunto completo de unidades, só assim o TDD vai funcionar como deve, devendo fornecer uma cobertura completa aos testes.

Além disso, os testes devem seguir o modelo F.I.R.S.T.

* **F** (Fast) - Rápidos: devem ser rápidos, pois testam apenas uma unidade;
* **I** (Isolated) - Testes unitários são isolados, testando individualmente as unidades e não sua integração;
* **R** (Repeateble) - Repetição nos testes, com resultados de comportamento constante;
* **S** (Self-verifying) - A auto verificação deve verificar se passou ou se deu como falha o teste;
* **T** (Timely) - O teste deve ser oportuno, sendo um teste por unidade.
