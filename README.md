Table of Contents
* [Functional Programming](#functional-programming)
* [Hexagonal Architecture Pattern](#hexagonal-architecture-pattern)
* [Big-O Notation](#big-o-notation)

### Functional Programming

Software sem bugs, reduzindo falhas em produção com práticas de programação funcional (em C#) - Elemar Junior
https://www.infoq.com/br/presentations/software-sem-bugs-reduzindo-falhas-em-producao-com-programacao-funcional?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global

- Abordagem declarativa vs imperativa
- Immutability (vantagens na programação paralela)
- Intensive Caching
- High-order functions
- Lazyness
- Option
- Either (validações garantidas por design)
- Functions (funções com implementações concretas ao invés de classes)

### Hexagonal Architecture Pattern
https://staging.cockburn.us/hexagonal-architecture/
![](https://github.com/fabioono25/study/blob/master/images/hexagonal_architecture.jpg)

- Avoid business logic into user interface (system can't be tested properly)
- Highly tied between logic and external entities (front/database) cause problems
- Rule: code pertaining to the "inside" part shout no leak into the "outside" part
- API: purpose of conversation between two devices
- Adapter: provides a way to convert API definition to the signals needed by the device and vice versa
- Test adapters, HTTP adapters, GUI adapters (user-side API - port)

![](https://github.com/fabioono25/study/blob/master/images/Hexagonal-architecture-complex-example.gif)

### Big-O Notation

https://www.youtube.com/watch?v=__vX2sjlpXU&vl=pt

http://www.corejavainterviewquestions.com/idiots-guide-big-o/

- Simplify analysis of an algorithm's efficiency;
- Types of measurement (worst, best, average case);
- O(1)/Constant Complexity: constant time - irrelevant of the size of the data - Queue;
- O(log n)/Logarithmic Complexity: grows but not proportionately - Binary Search;
- O(n)/Linear Complexity: time taken grows proportionately - LinkedList finding some element;
- O(n log n): Logarithmic + Linear, normally there's 2 parts of the sort - merge sort;
- O(n^2)/Quadratic Complexity: extra slow - Bubble Sort;
- O(2^n)/Exponential Growth: algorithm takes twice as long for every new element added;
- O(1) -> O(n) -> O(n^2)

![](https://github.com/fabioono25/links/blob/master/images/bigO_complexity.PNG)

![List of Some Common Asymptotic Notations](https://github.com/fabioono25/links/blob/master/images/Asymptotic_notations.PNG)
