[![Java CI with Gradle](https://github.com/Elena-Yakovleva/JavaPatterns/actions/workflows/gradle.yml/badge.svg)](https://github.com/Elena-Yakovleva/JavaPatterns/actions/workflows/gradle.yml)

### Домашнее задание к занятию «2.3. Patterns»

#### Задача №1: заказ доставки карты (изменение даты)
Вам необходимо автоматизировать тестирование новой функции формы заказа доставки карты:

![](https://github.com/netology-code/aqa-homeworks/raw/master/patterns/pic/order.png)


Требования к содержимому полей, сообщения и другие элементы, по словам заказчика и разработчиков, такие же, они ничего не меняли.

Примечание: личный совет — не забудьте это перепроверить, никому нельзя доверять 😈

Тестируемая функциональность: если заполнить форму повторно теми же данными, за исключением «Даты встречи», то система предложит перепланировать время встречи:

![](https://github.com/netology-code/aqa-homeworks/raw/master/patterns/pic/replan.png)

После нажатия кнопки «Перепланировать» произойдёт перепланирование встречи:

![](https://github.com/netology-code/aqa-homeworks/raw/master/patterns/pic/success.png)

**Важно**: в этот раз вы не должны хардкодить данные прямо в тест. Используйте Faker, Lombok, data-классы для группировки нужных полей и утилитный класс-генератор данных — см. [пример](https://github.com/netology-code/aqa-code/blob/master/patterns/patterns-task1/src/test/java/ru/netology/delivery/data/DataGenerator.java).

Утилитными называют классы, у которых приватный конструктор и статичные методы.

Обратите внимание, что Faker может генерировать не совсем в нужном для вас формате.

