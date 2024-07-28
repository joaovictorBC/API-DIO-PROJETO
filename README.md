## Diagrama de classes

```mermaid

classDiagram
    class Bank {
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }

    class Account {
        +int number
        +String agency
        +float balance
        +float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +float limit
    }

    class News {
        +String icon
        +String description
    }

    Bank --> Account
    Bank --> Feature
    Bank --> Card
    Bank --> News
