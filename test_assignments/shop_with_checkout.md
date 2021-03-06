## Ruby: функция Checkout для магазина

**Условия**

Дан список товаров:

| Код    | Название   | Цена   |
| ------ | ---------- | ------ | 
| CC     | Кока Кола  | $1.50  |
| PC     | Пепси Кола | $2.00  |
| WA     | Вода       | $0.85  |

Для некоторых продуктов есть определенные правила дисконтирования:

- если покупаете 3 и более бутылки Пепси Колы, то стоимость каждой бутылки Пепси Колы снижается на 20%;

- если покупаете одну бутылку Кока Колы, то вторая даётся бесплатно.
 
**Задача**

Реализуйте класс `Checkout` и необходимые дополнительные классы, которые считают общую стоимость покупки.

**Пример использования:**

```
co = Checkout.new(pricing_rules) 
co.add(item) p
co.total
```

Примеры:

- Input: CC PC WA 

    Output: $4.35 ;

- Input: CC PC CC CC 

    Output: $5.00 ;

- Input: PC CC PC WA PC CC 

    Output: $7.15 ;

Оценивается работоспособность, структура, архитектура, используемые шаблоны проектирования и тесты (используйте RSpec).