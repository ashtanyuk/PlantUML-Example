# Пример использования PlantUML

```plantuml
@startuml
class FruitBox {
    Fruit* content[]
    printFruitInfo(Fruit*)
    addFruit(Fruit*)
    getCost()
}
class Fruit {
    info()
    getCost()
}
class Apple {
    info()
    getCost()
}
class Banana {
    info()
    getCost()
}

Fruit <|-- Apple
Fruit <|-- Banana
FruitBox o- Fruit
@enduml
```