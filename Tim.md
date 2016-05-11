##### ChainOfResponsibilities
DiC of symfony2 for example
-  a Spam filter
##### Command
This pattern uses a "Command" to delegate the method call against the Receiver and presents the same method "execute".
-  A text editor : all events are Command which can be undone, stacked
   and saved.
##### Iterator
`class BookListIterator implements \Iterator`
`@link http://php.net/manual/en/iterator.valid.php`
`if $iterator->valid() $expectedBook = array_shift($expected);`
##### Mediator
All components (called Colleague) are only coupled to the MediatorInterface.
#### 03/05/2016 Behavioral
##### Memento
It provides the ability to restore an object to it's previous state (undo
via rollback) or to gain access to state of the object, without revealing
it's implementation (i.e., the object is not required to have a functional
for return the current state).
##### NullLogger
Methods that return an object or null should instead return an object or
`NullObject`. `NullObject` simplify boilerplate code such as
`if (!is_null($obj)) { $obj->callSomething(); }` to just
`$obj->callSomething();` by eliminating the conditional check in
client code.
#### Observer
To implement a publish/subscribe behaviour to an object.
-  a message queue system is observed to show the progress of a job in a GUI
#### 04/05/2016
#### Specification
Builds a clear specification of business rules, where objects can be
checked against. The composite specification class has one method called `isSatisfiedBy`.
`abstract class AbstractSpecification implements SpecificationInterface`
#### State
Encapsulate varying behavior for the same routine based on an object's state.
#### Strategy
To separate strategies and to enable fast switching between them.
-  sorting a list of objects, one strategy by date, the other by id
#### TemplateMethod
let subclasses of this abstract template "finish" the behavior of an algorithm
-  well-suited for framework libraries
-  How to test an abstract template method with PHPUnit.
#### Visitor
outsource operations on objects to other objects.
- `Role::accept`