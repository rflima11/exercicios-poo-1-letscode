# Polimorfismo

1. O que é polimorfismo? Descreva com suas palavras em uma frase. 
> Polimorfismo é o conceito da Orientação a Objetos onde podemos representar os casos de "É UM" através da subbstituição do tipo específico pelo geral, ou a parte pelo todo, ainda, a subclasse pela superclasse. 
2. Explique porque o polimorfismo pode ser uma estratégia útil.
3. Em Java, declaramos uma variável usando a sintaxe `[Tipo] [variável] = [valor]`. Considerando a representação de herança onde `Animal` é a superclasse e `Cachorro` a subclasse, quais são TODAS as formas possíveis de declarar uma variável para a nova instância `new  Cachorro()`?
```java
Cachorro cachorro = new Cachorro();
Animal cachorro = new Cachorro();
Object cachorro = new Cachorro();
```
4. É possível aplicar o princípio do polimorfismo tanto para interfaces quanto para classes. 
	a) **V**
	b) F
5. Quando definimos uma relação de herança entre duas classes, a classe-filha possui disponível os métodos herdados de sua classe-pai mais os métodos definidos nela mesmo.
	a) **V**
	b) F
6. Quando usamos polimorfismo, os métodos específicos da classe-filha ficam inacessíveis, pois estamos representando aquele objeto através da classe-pai.
	a) **V**
	b) F
7. Considere a interface `Animal` com os métodos `alimentar` e `respirar`. Considere também a classe `Cachorro` que implementa a interface `Animal`, e define seus próprios métodos `brincar` e `comunicar`. Quais métodos estarão disponíveis ao declarar a variável `Cachorro cachorro = new Cachorro`? 
> Todos os métodos estarão disponíveis porque a variável é do mesmo tipo da instância. Não está sendo usado o recurso de polimorfismo aqui. 
8. Criamos uma classe Cachorro com os seus métodos próprios `brincar` e `comunicar`. Além disso, `Cachorro` implementa a interface `Animal` que possui definição para o método `alimentar`. Se aplicarmos o princípio do polimorfismo declarando uma variável do tipo `Animal cachorro = new Cachorro()`, quais métodos estarão disponíveis na variável `cachorro`? 
> Quando o polimorfismo é aplicado, temos disponível na variável a apenas os métodos definidos na superclasse ou na interface. 
9. Ao criar uma classe chamada `Aluno` e invocar que uma variável `Aluno aluno =  new Aluno();` para exibir em console através de `System.out.println(aluno);`, o resultado é semelhante a `Aluno@6a6824be`. Por quê? 
10. Ao declarar uma variável do tipo `Aluno aluno = new Aluno();`, e exibi-la em console através de `System.out.println(aluno);` o resultado foi `Aluno@6a6824be`. Considerando que a classe `Aluno` possui os atributos nome e matrícula, como poderíamos definir um método que exiba corretamente essas informações em console? 
