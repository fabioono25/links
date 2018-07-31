Table of Contents
* [Functional Programming](#functional-programming)
* [Hexagonal Architecture Pattern](#hexagonal-architecture-pattern)
* [Big-O Notation](#big-o-notation)
* [Searching Techniques](#searching-techniques)
  * [Linear Search](#linear-search)
  * [Binary Search](#binary-search)
* [Sorting Algorithms](#searching-algorithms)
  * [Merge Sort](#merge-sort)
  * [Insertion Sort](#insertion-sort)  
  * [Bubble Sort](#bubble-sort)    
  * [Quick Sort](#quick-sort)    
  * [Heap Sort](#heap-sort)      
  * [Counting Sort](#counting-sort)      
* [Authentication and Authorization](#authentication-and-authorization)

### Functional Programming

[Software sem bugs, reduzindo falhas em produção com práticas de programação funcional (em C#) - Elemar Junior]
(https://www.infoq.com/br/presentations/software-sem-bugs-reduzindo-falhas-em-producao-com-programacao-funcional?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global)

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

[Big O Notation with Gayle Laakmann McDowell](https://www.youtube.com/watch?v=v4cd1O4zkGw)

[Big-O notation in 5 minutes — The basics](https://www.youtube.com/watch?v=__vX2sjlpXU&vl=pt)

http://www.corejavainterviewquestions.com/idiots-guide-big-o/

![](https://github.com/fabioono25/links/blob/master/images/big_o.PNG)

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

### Searching Techniques

##### Linear Search

In this type of search, a sequential search is made over all items one by one. Every item is checked and if a match is found then that particular item is returned, otherwise the search continues till the end of the data collection.

Linear search has O(N) complexity.

![](https://github.com/fabioono25/study/blob/master/images/linear_search.gif)

##### Binary Search

With this strategy, the target value is compared with de middle element of a SORTED array. This means a gain of performance.

Binary search has a O(log n) complexity running time.

![](https://github.com/fabioono25/study/blob/master/images/binarySearch.gif)

### Sorting Algorithms

![](https://github.com/fabioono25/study/blob/master/images/sorting_algorithms.PNG)

##### Merge Sort

https://brilliant.org/wiki/merge/

Is a comparison-based algorithm that focuses on how to merge together two pre-sorted arrays such that the resulting array is also sorted.
Steps: merging and sorting. Divide-and-conquer approach to merge and sort a list.

![](https://github.com/fabioono25/study/blob/master/images/merge_sort.gif)
![](https://github.com/fabioono25/study/blob/master/images/Merge-Sort.png)

##### Insertion Sort

https://brilliant.org/wiki/insertion/

![](https://github.com/fabioono25/study/blob/master/images/insertion_sort.gif)

##### Bubble Sort

https://brilliant.org/wiki/bubble-sort/

![](https://github.com/fabioono25/study/blob/master/images/bubble_sort.gif)

##### Quick Sort

https://brilliant.org/wiki/quick-sort/

![](https://github.com/fabioono25/study/blob/master/images/quick_sort.gif)

##### Heap Sort

https://brilliant.org/wiki/heap-sort/

![](https://github.com/fabioono25/study/blob/master/images/heap_sort.gif)

##### Counting Sort

https://brilliant.org/wiki/counting-sort/

![](https://github.com/fabioono25/study/blob/master/images/counting_sort.gif)
  

### Authentication and Authorization

- [Authentication](https://stackoverflow.com/questions/6556522/authentication-versus-authorization): the mechanism determines the user's identity before revealing the sensitive information. With this process it's possible validation of the identity of a registered user who is accessing a service or application; 
- [Authorization](https://techdifferences.com/difference-between-authentication-and-authorization.html): this process ensures that an authenticated user has the necessary privileges to access a specific resource or operation within an application

![](https://github.com/fabioono25/study/blob/master/images/authenticationAuthorization.jpg)

![](https://github.com/fabioono25/study/blob/master/images/jwt.jpg)


