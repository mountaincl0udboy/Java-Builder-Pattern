# Builder-Pattern
Builder pattern was introduced to solve some of the problems with Factory and Abstract Factory design patterns when the Object contains a lot of attributes.

There are three major issues with Factory and Abstract Factory design patterns when the Object contains a lot of attributes.

- Too Many arguments to pass from client program to the Factory class that can be error prone because most of the time, the type of arguments are same and from client side its hard to maintain the order of the argument.
- Some of the parameters might be optional but in Factory pattern, we are forced to send all the parameters and optional parameters need to send as NULL.
- If the object is heavy and its creation is complex, then all that complexity will be part of Factory classes that is confusing.  

We can solve the issues with large number of parameters by providing a constructor with required parameters and then different setter methods to set the optional parameters. The problem with this approach is that the Object state will be inconsistent until unless all the attributes are set explicitly.

Builder pattern solves the issue with large number of optional parameters and inconsistent state by providing a way to build the object step-by-step and provide a method that will actually return the final Object.

Builder Design Pattern in Java
Let’s see how we can implement builder design pattern in java.

- First of all you need to create a static nested class and then copy all the arguments from the outer class to the Builder class. We should follow the naming convention and if the class name is Computer then builder class should be named as ComputerBuilder.
- Java Builder class should have a public constructor with all the required attributes as parameters.
- Java Builder class should have methods to set the optional parameters and it should return the same Builder object after setting the optional attribute.
- The final step is to provide a build() method in the builder class that will return the Object needed by client program. For this we need to have a private constructor in the Class with Builder class as argument.

## Contact me
- [Instagram](https://www.instagram.com/ogkkk.exe/)


# Шаблон-Builder
Шаблон Builder был введен для решения некоторых проблем с шаблонами проектирования Factory и Abstract Factory, когда объект содержит много атрибутов.

Есть три основных проблемы с шаблонами проектирования Factory и Abstract Factory, когда объект содержит много атрибутов.

- Слишком много аргументов для передачи из клиентской программы в класс Factory, что может быть подвержено ошибкам, потому что в большинстве случаев тип аргументов одинаков, и со стороны клиента сложно поддерживать порядок аргумента.
- Некоторые параметры могут быть необязательными, но в шаблоне Factory мы вынуждены отправлять все параметры, а необязательные параметры необходимо отправлять как NULL.
- Если объект тяжелый и его создание сложное, то вся эта сложность будет частью классов Factory, что сбивает с толку.

Мы можем решить проблемы с большим количеством параметров, предоставив конструктор с обязательными параметрами, а затем различные методы установки для установки необязательных параметров. Проблема с этим подходом заключается в том, что состояние объекта будет несогласованным до тех пор, пока все атрибуты не будут установлены явно.

Шаблон Builder решает проблему с большим количеством необязательных параметров и несогласованным состоянием, предоставляя способ пошагового построения объекта и предоставляя метод, который фактически возвращает окончательный объект.

Шаблон проектирования Builder в Java
Давайте посмотрим, как мы можем реализовать шаблон проектирования Builder в java.

- Прежде всего вам нужно создать статический вложенный класс, а затем скопировать все аргументы из внешнего класса в класс Builder. Мы должны следовать соглашению об именах, и если имя класса — Computer, то класс Builder должен называться ComputerBuilder.
- Класс Java Builder должен иметь общедоступный конструктор со всеми необходимыми атрибутами в качестве параметров.
- Класс Java Builder должен иметь методы для установки необязательных параметров и должен возвращать тот же объект Builder после установки необязательного атрибута.
- Последним шагом является предоставление метода build() в классе построителя, который будет возвращать объект, необходимый клиентской программе. Для этого нам нужно иметь частный конструктор в классе с классом Builder в качестве аргумента.

## Связь со мной
- [Instagram](https://www.instagram.com/ogkkk.exe/)
