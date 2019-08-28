### Polymorphism in Ruby

The term polymorphism means having many forms. In Ruby, polymorphism is carried out by using Inheritance. Polymorphism is achieved by using method overriding.

```
class Animal
    def eat # this method will overrides on other inherited classes
        puts "Animal eats grasses, water, milk, etc"
    end
end

class Cat < Animal
    def eat
        puts "Cat eats milk & water"
    end
end

class Cow < Animal
    def eat
        puts "Cow eats grasses & water"
    end
end
```

```
animal = Animal.new
animal.eat
=> Animal eats grasses, water, milk, etc

animal = Cat.new
animal.eat
=> Cat eats milk & water

animal = Cow.new
animal.eat
=> Cow eats grasses & water
```