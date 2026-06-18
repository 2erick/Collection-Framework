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

class Map <<Interface>>

class SortedMap <<Interface>>

class ArrayList

class LinkedList

class Vector

class Stack

class PriorityQueue

class ArrayDequeue

class HashSet

class LinkedHashSet

class TreeSet

class TreeMap

class HashTable

class LinkedHashMap

class HashMap

Collection ..|> Iterable

List ..|> Collection

Queue ..|> Collection

Set ..|> Collection

Dequeue ..|> Queue

SortedSet ..|> Set

SortedMap ..|> Map

TreeMap ..|> SortedMap

ArrayList --|> List

LinkedList --|> List

Vector --|> List

Stack ..|> Vector

PriorityQueue --|> Queue

ArrayDequeue --|> Dequeue

HashSet --|> Set

LinkedHashSet --|> Set

TreeSet --|> SortedSet

HashTable --|> Map

LinkedHashMap --|> Map

HashMap --|> Map

```

Iterable -> Collection