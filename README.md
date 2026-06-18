# Collection-Framework

Java Collection Framework, um conjunto de interfaces e classes que simplificam o trabalho com estruturas de dados como listas, conjuntos, filas e mapas.

Estrutura que agrupa elementos objetos em uma estrutura de dados, o elemento precisa ser objeto.

Não aceita primitivo. Use warape se necessario.

Pode ter homogeneas e heterogenias. Se utilizarmos o polimorfismo conseguimos o heterogeneo.

```mermaid
classDiagram

class Iterable <<Interface>>
class Collection <<Interface>>
class List <<Interface>>
class Queue <<Interface>>
class Set <<Interface>>
class Dequeue <<Interface>>
class SortedSet <<Interface>>

class ArrayList
class LinkedList
class Vector
class Stack
class PriorityQueue
class ArrayDequeue
class HashSet
class LinkedHashSet
class TreeSet

Collection ..|> Iterable
List ..|> Collection
Queue ..|> Collection
Set ..|> Collection
Dequeue ..|> Queue
SortedSet ..|> Set

ArrayList --|> List
LinkedList --|> List
Vector --|> List
Stack ..|> Vector
PriorityQueue --|> Queue
ArrayDequeue --|> Dequeue
HashSet --|> Set
LinkedHashSet --|> Set
TreeSet --|> SortedSet

```

## Map

```mermaid
classDiagram

class Map <<Interface>>
class SortedMap <<Interface>>

class HashMap
class LinkedHashMap
class TreeMap
class HashTable

SortedMap ..|> Map
TreeMap ..|> SortedMap
HashMap --|> Map
LinkedHashMap --|> Map
HashTable --|> Map
```


Todas essas classe e interfaces então dentro do `java.utils`

## Docs Collections Java

[Collection (Java Platform SE 8 )](https://docs.oracle.com/javase/8/docs/api/java/util/Collection.html)
