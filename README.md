# SOLID em JAVA
Conteudo da aula:
# 1.3) Principios de orientação a Objetos

- coesão 
- Encapsulamento
- Acoplamento


Coesão: união harmonica entre uma coisa e outra.
quando está tratando do mesmo assunto no código

Por exemplo de má prática:
- ter atributos no endereço numa classe do Funcionario
- Metodos de formatar CEP // CompletarEndereço

Classes não coesas tendem a crescer indefinidademente a 
medida que as tornam dificieis de manter

# 1.5) Encapsulamento

Ato de incluir ou proteger alguma coisa em uma cápsula.
Encapsulamento é blindar uma classe para proteger de influencias externas
que podem violar a regra de negócio

Exemplo: 
- uso de modificadores de acesso private e protected
- Uso de Setter pode burlar a regra de negócio


# 1.7) Acoplamento
A ação de acoplar, argumento pares

Quando você tem 2 componentes que estão ligados entre si causando dependencia entre eles,
quando uma classe chama outra classe

O problema é quando esse acoplamento se torna uma dependencia muito forte

Normalmente a lógica ficaria fora da classe.

Classes acopladas causam fragilidade no código da aplicação, o que dificulta sua manutenção.



## Coesão:
- Uma classe coesa faz bem uma única coisa
- Classes coesas não devem ter várias responsabilidades
## Encapsulamento:
- Getters e setters não são formas eficientes de aplicar encapsulamento
- É interessante fornecer acesso apenas ao que é necessário em nossas classes
- O encapsulamento torna o uso das nossas classes mais fácil e intuitivo
## Acoplamento:
- Acoplamento é a dependência entre classes
- Acoplamento nem sempre é ruim, e que é impossível criar um sistema sem nenhum acoplamento
- Devemos controlar o nível de acoplamento na nossa aplicação (falaremos mais sobre isso)




# 2.3) SRP - Single Responsability Principle 
A classe deveria ter apenas um unico motivo para mudar


- Que classes/métodos/funções/módulos devem ter uma única responsabilidade bem definida;
- Que, segundo o Princípio de Responsabilidade Única (SRP), uma classe deve ter um e apenas um motivo para ser alterada;
- Como realizar uma refatoração no nosso sistema, para aplicar o SRP;
- Como extrair uma classe.



# 3.4) OCP - Open closed Principle

Abertas a extensão porem fechadas a modificação

- Que cada classe deve conhecer e ser responsável por suas próprias regras de negócio;
- Que o princípio Aberto/Fechado (OCP) diz que um sistema deve ser aberto para a extensão, mas fechado para a modificação
- Isso significa que devemos poder criar novas funcionalidades e estender o sistema sem precisar modificar muitas classes já existentes
- Uma classe que tende a crescer "para sempre" é uma forte candidata a sofrer alguma espécie de refatoração.


Favorecer a composição não a herança


# 4.5) LSP - Liskov Substitution Principle

"Se q(x) é uma propriedade demonstravél dos objetos de x de tipo T, então q(y) deve ser verdadeira para ojetos y de tipo S, onde S é um subtipo de T"

- Que, embora a herança favoreça o reaproveitamento de código, ela pode trazer efeitos colaterais quando não utilizada da maneira correta;
- Que o Princípio de Substituição de Liskov (LSP) diz que devemos poder substituir classes base por suas classes derivadas em qualquer lugar, sem problema.

# 5.3) DIP - Dependency Inversion Principle

Abstrações não devem depender de implementações
implementações devem depender de abstrações

Caso uma determinada implementação mude, não seremos afetados, pois dependemos apenas de sua interface.

# 5.5) ISP - Interface Segregation Principle

Uma classe não deveria ser forçada a depender de métodos que não utilizará

Iremos implementar uma interface somente quando utilizaremos todos os metodos se não deveremos criar uma interface específica e extender da interface generica


- Que é mais interessante e mais seguro para o nosso código depender de interfaces (classes abstratas, assinaturas de métodos e interfaces em si) do que das implementações de uma classe;
- Que as interfaces são menos propensas a sofrer mudanças enquanto implementações podem mudar a qualquer momento;
- Que o Princípio de Inversão de Dependência (DIP) diz que implementações devem depender de abstrações e abstrações não devem depender de implementações;
- Que as interfaces devem definir apenas os métodos que fazem sentido para seu contexto;
- Que o Princípio de Segregação de Interfaces (ISP) diz que uma classe não deve ser obrigada a implementar um método que ela não precisa;
- Os conceitos aprendidos neste treinamento formam o acrônimo SOLID:
	- Single Responsibility Principle
	- Open Closed Principle
	- Liskov Substitution Principle
	- Interface Segregation Principle
	- Dependency Inversion Principle
