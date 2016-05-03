#### ChainOfResponsibilities

DiC of symfony2 for example

#### Iterator
`class BookListIterator implements \Iterator`
`@link http://php.net/manual/en/iterator.valid.php`
`if $iterator->valid() $expectedBook = array_shift($expected);`

#### Mediator is the concrete Mediator


### 03/05/2016

#### Memento
It provides the ability to restore an object to it's previous state (undo
via rollback) or to gain access to state of the object, without revealing
it's implementation (i.e., the object is not required to have a functional
for return the current state).

#### Behavioral\NullLogger

Methods that return an object or null should instead return an object or
`NullObject`. `NullObject` simplify boilerplate code such as
`if (!is_null($obj)) { $obj->callSomething(); }` to just
`$obj->callSomething();` by eliminating the conditional check in
client code.


