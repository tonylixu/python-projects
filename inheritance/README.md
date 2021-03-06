### Multiple Inheritance
Multiple inheritance is a touchy subject. In principle, it's very simple: a subclass that inherits from more than one 
parent class is able to access functionality from both of them. In practice, this is less useful than it sounds and many 
expert programmers recommend against using it.

As a rule of thumb, if you think you need multiple inheritance, you're probably wrong, but if you know you need it, you'are probably right.

Multiple inheritance works all right when mixing methods from different classes, but it gets very messey when we have to call methods on the superclass.

### Mixin
The simplest and most useful form of multiple inheritance is called a `mixin`. A `mixin` is generally a superclass that is not meant to exist on its own, but it meant to be inherited by some other class to provide extra functionality.

```python
class EmailableContact(Contact, MailSender):
    pass
```


