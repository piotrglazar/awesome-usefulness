# awesome-usefulness
Very useful stuff about programming

# Java
* [High scale Java lib](https://github.com/edwardw/high-scale-java-lib)
* [JCTools](https://github.com/JCTools/JCTools)
* [Awesome Java](https://github.com/piotrglazar/awesome-java)
* [Unix Stream](https://github.com/benas/UnixStream)
* [JavaSlang](http://javaslang.com/)

# Scala
* [Awesome Scala](https://github.com/piotrglazar/awesome-scala)
* [Spire - numeric tools](https://github.com/non/spire)

# Algorithm
* [word2vec](https://github.com/cedias/word2vec)

# Soft
* [Lists](https://github.com/jnv/lists)
* [Awesome awesomeness](https://github.com/bayandin/awesome-awesomeness)
* [Engineering blogs](https://github.com/piotrglazar/engineering-blogs)
* [MagSpoof](https://github.com/samyk/magspoof)

# .NET
* [TailBlazer](https://github.com/RolandPheasant/TailBlazer)

# Misc
* [Interview questions](https://github.com/MaximAbramchuck/awesome-interviews)
* [h2scan](https://github.com/jgrahamc/h2scan)
* [ConEmu](https://github.com/Maximus5/ConEmu)
* [IncludeOS](https://github.com/hioa-cs/IncludeOS)
* [PhDs](https://github.com/nuprl/10PL)
* [Astrophysics source code](http://ascl.net/code/all/order/date/dir/desc/listmode/full)

# Web
* [react bootstrap](https://github.com/react-bootstrap/react-bootstrap)
* [Jump.js](http://callmecavs.github.io/jump.js/)
* [D3](https://github.com/d3/d3-shape)

# DB
* [DGraph](https://github.com/dgraph-io/dgraph)

# Interview
## Trees
Tree is a directed acyclic graph. There top node is called root, bottom nodes are called leaves.
Binary search trees (BST) are the most commonly used kind of trees. A tree must be balanced in order to
keep all operations efficient.
There are two widely known efficient tree implementations: AVL and red-black tree.
In Java, BST is known as SortedSet (interface) with TreeSet as concrete implementation.

## Lists
There are two kinds of lists: array list and linked list.

## Hashmaps
Is usually backed by an array. In order to put an object into a hashmap, one has to compute a hash value
of the object. In Java, in class Object there is a `hashCode` method. It comes together with `equals` method.
The next step is to calculate index, which is hasCode mod array size (`HashMap` uses power of two as table size).
Underlying table contains so-called buckets. A bucked can be a linked list or a tree (depending on the number of collisions).
When a `HashMap` is filled to a certain amount, it grows. 

## Equals and hashCode
The contract between `equals()` and `hashCode()` is:
1. If two objects are equal, then they must have the same hash code.
2. If two objects have the same hash code, they may or may not be equal.
`EqualsVerifier` can be used to test if this contract is satisfied.

## Gang of four design patters
The Gang of Four are the authors of the book, "Design Patterns: Elements of Reusable Object-Oriented Software". 
This important book describes various development techniques and pitfalls in addition to providing twenty-three 
object-oriented programming design patterns. The four authors were Erich Gamma, Richard Helm, Ralph Johnson and John Vlissides.

### Creational Patterns
The first type of design pattern is the creational pattern. Creational patterns provide ways to instantiate single 
objects or groups of related objects. There are five such patterns:

* **Abstract Factory:** Creates an instance of several families of classes. Provide an interface for creating families 
of related or dependent objects without specifying their concrete classes.

* **Builder:** Separates object construction from its representation. Separate the construction of a complex object 
from its representation so that the same construction processes can create different representations.

* **Factory Method:** The factory pattern is used to replace class constructors, abstracting the process of object 
generation so that the type of the object instantiated can be determined at run-time.

* **Prototype:** The prototype pattern is used to instantiate a new object by copying all of the properties of an 
existing object, creating an independent clone. This practise is particularly useful when the construction of a new 
object is inefficient.

* **Singleton:** The singleton pattern ensures that only one object of a particular class is ever created. All further 
references to objects of the singleton class refer to the same underlying instance.

### Structural Patterns
The second type of design pattern is the structural pattern. Structural patterns provide a manner to define 
relationships between classes or objects.

* **Adapter:** The adapter pattern is used to provide a link between two otherwise incompatible types by wrapping the 
"adaptee" with a class that supports the interface required by the client.

* **Bridge:** The bridge pattern is used to separate the abstract elements of a class from the implementation details, 
providing the means to replace the implementation details without modifying the abstraction.

* **Composite:** The composite pattern is used to create hierarchical, recursive tree structures of related objects where 
any element of the structure may be accessed and utilised in a standard manner.

* **Decorator:** The decorator pattern is used to extend or alter the functionality of objects at run-time by wrapping 
them in an object of a decorator class. This provides a flexible alternative to using inheritance to modify behaviour.

* **Facade:** The facade pattern is used to define a simplified interface to a more complex subsystem.

* **Flyweight:** A fine-grained instance used for efficient sharing. Use sharing to support large numbers of 
fine-grained objects efficiently. A flyweight is a shared object that can be used in multiple contexts simultaneously. 
The flyweight acts as an independent object in each context — it’s indistinguishable from an instance of the object 
that's not shared.

* **Proxy:** The proxy pattern is used to provide a surrogate or placeholder object, which references an underlying 
object. The proxy provides the same public interface as the underlying subject class, adding a level of indirection by 
accepting requests from a client object and passing these to the real subject object as necessary.

### Behavioural Patterns
The final type of design pattern is the behavioural pattern. Behavioural patterns define manners of communication 
between classes and objects.

* **Chain of Responsibility:** The chain of responsibility pattern is used to process varied requests, each of which may 
be dealt with by a different handler.

* **Command:** The command pattern is used to express a request, including the call to be made and all of its required 
parameters, in a command object. The command may then be executed immediately or held for later use.

* **Interpreter:** The interpreter pattern is used to define the grammar for instructions that form part of a language or
notation, whilst allowing the grammar to be easily extended.

* **Iterator:** The iterator pattern is used to provide a standard interface for traversing a collection of items in an 
aggregate object without the need to understand its underlying structure.

* **Mediator:** The mediator pattern is used to reduce coupling between classes that communicate with each other. Instead
of classes communicating directly, and thus requiring knowledge of their implementation, the classes send messages via a
mediator object.

* **Memento:** The memento pattern is used to capture the current state of an object and store it in such a manner that 
it can be restored at a later time without breaking the rules of encapsulation.

* **Observer:** The observer pattern is used to allow an object to publish changes to its state. Other objects subscribe 
to be immediately notified of any changes.

* **State:** The state pattern is used to alter the behaviour of an object as its internal state changes. The pattern 
allows the class for an object to apparently change at run-time.

* **Strategy:** The strategy pattern is used to create an interchangeable family of algorithms from which the required 
process is chosen at run-time.

* **Template Method:** The template method pattern is used to define the basic steps of an algorithm and allow the 
implementation of the individual steps to be changed.

* **Visitor:** The visitor pattern is used to separate a relatively complex set of structured data classes from the 
functionality that may be performed upon the data that they hold.

Another version can be found [here](http://geekswithblogs.net/subodhnpushpak/archive/2009/09/18/the-23-gang-of-four-design-patterns-.-revisited.aspx).

## Concurrency

### Volatile keyword
Essentially, volatile is used to indicate that a variable's value will be modified by different threads.
`volatile` variables are not stored in CPU cache. They are fetched from RAM. Java will not reorder operations that
use `volatile` variables. They can be stored or fetched atomically, provided that a value is not greater than 32 bits.
Access to the variable acts as though it is enclosed in a synchronized block, synchronized on itself.
The most typical case when to use a volatile is where:

* you write a variable, such as a flag, in one thread,
* you check that variable in another thread,
* crucially, the value to write doesn't depend on the current value,
* or, you don't care about "missing an update".

In `volatile` context, sometimes `AtomicReferenceFieldUpdater` is mentioned. More info can be found [here](https://www.javamex.com/tutorials/synchronization_concurrency_7_atomic_updaters.shtml).

### Atomic variables
`AtomicInteger` and friends can be used in various concurrent scenarios as counters etc. One of the commonly used
functions is `incrementAndGet()` which is a thread-safe `++x` operation. There is also an `AtomicReference` class that
allows to update a reference atomically. For example, one can replace a reference to an immutable data structure
which can then be used by many threads.
When an object is coupled with boolean or integer flags, one can use `AtomicMarkableReference` or `AtomicStampedReference`.
Since Java 5 one can also use `AtomicIntegerArray`, `AtomicLongArray` and `AtomicReferenceArray` which are more GC
friendly than an array of `AtomicInteger`s.

### Synchronized blocks
Its overall purpose is to only allow one thread at a time into a particular section of code thus allowing us to protect,
for example, variables or data from being corrupted by simultaneous modifications from different threads.
Using a `synchronized` block or `volatile` keyword, threads may work on locally cached copies of variables such as 
count, updating the "main" copy when it suits them. They may also re-order reads and writes, meaning that updating 
a variable may not mean that it is updated when otherwise expected. However, on entry to and exit from blocks 
synchronized on a particular object, the entering/exiting thread also effectively synchronizes copies of all 
variables with main memory.

After Thread A exits a block synchronized on Object X, that Thread B when entering a block also synchronized on Object 
X will see the data as it was visible to thread A when it exited the block.

## Immutable objects
Immutable objects greatly simplify program, since they:
* are simple to construct, test, and use
* are automatically thread-safe and have no synchronization issues
* don't need a copy constructor
* don't need an implementation of clone
* allow hashCode to use lazy initialization, and to cache its return value
* don't need to be copied defensively when used as a field
* make good Map keys and Set elements (these objects must not change state while in the collection)
* have their class invariant established once upon construction, and it never needs to be checked again
* always have "failure atomicity" (a term used by Joshua Bloch): if an immutable object throws an exception, 
it's never left in an undesirable or indeterminate state

Make a class immutable by following these guidelines:
* ensure the class cannot be overridden - make the class final, or use static factories and keep constructors private
* make fields private and final
* force callers to construct an object completely in a single step, instead of using a no-argument constructor combined 
with subsequent calls to setXXX methods (that is, avoid the Java Beans convention)
* do not provide any methods which can change the state of the object in any way - not just setXXX methods, but any 
method which can change state
* if the class has any mutable object fields, then they must be defensively copied when they pass between the class 
and its caller

Immutable classes that can be already found in Java:
* java.lang.String
* java.lang.Integer, java.lang.Byte, java.lang.Character, java.lang.Short etc.
* java.lang.StackTraceElement
* enums
* java.math.BigInteger and java.math.BigDecimal (but subclasses could introduce mutability)
* java.io.File. Note that this represents an object external to the VM (a file on the local system), which may or may 
not exist, and has some methods modifying and querying the state of this external object. 
But the File object itself stays immutable. (All other classes in java.io are mutable.)
* java.util.UUID

# Basic failover, redundancy, consistency
## ACID
### Atomicity
Atomicity requires that each transaction be "all or nothing": if one part of the transaction fails, then the entire 
transaction fails, and the database state is left unchanged. An atomic system must guarantee atomicity in each and 
every situation, including power failures, errors and crashes. To the outside world, a committed transaction appears 
(by its effects on the database) to be indivisible ("atomic"), and an aborted transaction does not happen.

### Consistency
The consistency property ensures that any transaction will bring the database from one valid state to another. Any data 
written to the database must be valid according to all defined rules, including constraints, cascades, triggers, and 
any combination thereof. This does not guarantee correctness of the transaction in all ways the application programmer 
might have wanted (that is the responsibility of application-level code), but merely that any programming errors cannot 
result in the violation of any defined rules.

### Isolation
The isolation property ensures that the concurrent execution of transactions results in a system state that would be 
obtained if transactions were executed sequentially, i.e., one after the other. Providing isolation is the main goal of 
concurrency control. Depending on the concurrency control method (i.e., if it uses strict – as opposed to relaxed – 
serializability), the effects of an incomplete transaction might not even be visible to another transaction.

### Durability
The durability property ensures that once a transaction has been committed, it will remain so, even in the event of 
power loss, crashes, or errors. In a relational database, for instance, once a group of SQL statements execute, the
 esults need to be stored permanently (even if the database crashes immediately thereafter). To defend against power 
 loss, transactions (or their effects) must be recorded in a non-volatile memory.

## CAP theorem
also named Brewer's theorem after computer scientist Eric Brewer, states that it is impossible for a distributed data 
store to simultaneously provide more than two out of the following three guarantees:

### Consistency
Every read receives the most recent write or an error

### Availability
Every request receives a (non-error) response – without guarantee that it contains the most recent write

### Partition tolerance
The system continues to operate despite an arbitrary number of messages being dropped (or delayed) by the network 
between nodes

### Explanation
No distributed system is safe from network failures, thus network partitioning generally has to be tolerated. In the 
presence of a partition, one is then left with two options: consistency or availability. When choosing consistency over 
availability, the system will return an error or a time-out if particular information cannot be guaranteed to be up to 
date due to network partitioning. When choosing availability over consistency, the system will always process the query 
and try to return the most recent available version of the information, even if it cannot guarantee it is up to date due
to network partitioning.

In the absence of network failure – that is, when the distributed system is running normally – both availability and 
consistency can be satisfied.

CAP is frequently misunderstood as if one has to choose to abandon one of the three guarantees at all times. In fact, 
the choice is really between consistency and availability only when a network partition or failure happens; at all other
times, no trade-off has to be made.

## Partitioning
A popular application of partitioning is in a distributed database management system. Each partition may be spread over
multiple nodes, and users at the node can perform local transactions on the partition. This increases performance for
sites that have regular transactions involving certain views of data, whilst maintaining availability and security.

# Garbage collection 
## Garbage Collection Algorithms
### Serial GC (-XX:UseSerialGC): GC on Young Generation and Old Generation
Use the simple mark-sweep-compact cycle for young and tenured generations. This is good for client systems and systems
with low memory footprint and smaller CPU.

### Parallel GC (-XX:UseParallelGC): GC on Young Generation and Old Generation
This uses N threads, which can be configured using -XX:ParallelGCThreads=N, here N is also the number of CPU cores for
garbage collection. It uses these N threads for GC in the Young Generation but uses only one-thread in the Old Generation.

### Parallel Old GC (-XX:UseParallelOldGC): GC on Young Generation and Old Generation
This is same as the Parallel GC, except that it uses N threads for GC in both Old and Young Generation.

### Concurrent Mark and Sweep GC (-XX:ConcMarkSweepGC): GC on Old Generaton
As the name suggests, the CMS GC minimizes the pauses that are required for GC. It is most useful when used to create
highly responsive applications and it does GC only in the Old Generation. It creates multiple threads for GC that work
concurrently with applications threads, which can be specified using the -XX:ParallelCMSThreads=n.

### G1 GC (-XX:UseG1GC): GC on Young and Old Generation (By Dividing Heap into Equal Size Regions)
This is a parallel, concurrent, and incrementally compacting low-pause garbage collector. G1 was introduced in Java 7
with the ultimate vision to replace CMS GC. It divides the heap into multiple, equal sized regions and then performs GC,
usually starting with the region that has less live data, hence "Garbage First".

Garbage collectors can be combined, ie. young generation can have its own garbage collection and old generation can
use a different algorithm. A good article can be found [here](http://www.fasterj.com/articles/oraclecollectors1.shtml).

# Java memory structure
![this should be a picture of java memory structure](https://dzone.com/storage/temp/544006-untitled.jpg)
[Oracle documentation](https://docs.oracle.com/javase/specs/jvms/se7/html/jvms-2.html)

# Java reflection
## Bridge method
[Bridge method](https://docs.oracle.com/javase/tutorial/java/generics/bridgeMethods.html)

# Java quick thread communication
## Disruptor
[LMAX Disruptor](http://lmax-exchange.github.io/disruptor/) code examples can be found [here](https://github.com/LMAX-Exchange/disruptor/wiki/Getting-Started).
## Phaser
Java 7 introduces a flexible thread synchronization mechanism called Phaser. If you need to wait for threads to arrive
before you can continue or start another set of tasks, then Phaser is a good choice. [Code example](https://dzone.com/articles/java-7-understanding-phaser)
