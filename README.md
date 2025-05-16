# Santander Dev Week 2023
Projeto desenvolvido como parte da Santander Dev Week 2023, promovida pela DIO. Nesta jornada, tive a oportunidade de colocar em prática conceitos modernos do ecossistema Java, construindo uma API RESTful completa.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }

    class Account {
        +String number
        +String agency
        +Number balance
        +Number limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +Number limit
    }


    class News {
        +String icon
        +String description
    }

    User "1" *-- "1" Account
    User "1" *-- "N" Feature
    User "1" *-- "1" Card
    User "1" *-- "N" News
```

## Observações Finais
Este projeto foi reproduzido com fins educacionais, acompanhando o conteúdo da DIO.
