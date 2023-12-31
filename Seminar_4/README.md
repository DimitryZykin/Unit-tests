# Урок 4. Зависимости в тестах
## Задание 1. Ответьте письменно на вопросы:

1)  Почему использование тестовых заглушек может быть полезным при написании модульных тестов?

- Для отладки. Использование тестовых заглушек позволяет лучше контролировать процесс отладки, поскольку вы можете изменять поведение заглушки для имитации различных сценариев и условий, что может помочь быстрее определить и исправить ошибки.
- В целях повторного использования. Заглушки могут быть использованы для создания модульных тестов, которые можно легко повторять и адаптировать для различных сценариев тестирования.
- При изоляции. Тестовые заглушки позволяют изолировать тестируемый модуль от внешних зависимостей, что упрощает тестирование и делает его более надежным.
- Управление сложностью: При использовании тестовых заглушек вы можете сосредоточиться на тестировании одного конкретного аспекта или функции модуля, не отвлекаясь на другие внешние зависимости.
- Для ускорение разработки. При использовании заглушек вам не нужно заботиться о создании и настройке реальных зависимостей для каждого модульного теста, что ускоряет процесс разработки и позволяет быстрее проверять и добавлять новые функциональные возможности.
- Покрытие кода. Тестирование каждого модуля с использованием тестовых заглушек помогает гарантировать, что весь код покрывается тестами, что снижает вероятность ошибок и улучшает качество продукта.

2) Какой тип тестовой заглушки следует использовать, если вам нужно проверить, что метод был вызван с определенными аргументами?
Тстовые заглушки Mockito или EasyMock, которые позволяют создавать моки или заглушки методов, а затем контролировать и проверять их поведение.

3) Какой тип тестовой заглушки следует использовать, если вам просто нужно вернуть определенное значение или исключение в ответ на вызов метода?
Возвращающие заглушки, которые возвращают указанное значение или выбрасывают указанное исключение при вызове метода.

4) Какой тип тестовой заглушки вы бы использовали для имитации  взаимодействия с внешним API или базой данных?
Имитационные заглушки — это тип тестовых заглушек, которые используются для имитации работы внешних сервисов, таких как API или базы данных, в процессе тестирования. Они позволяют заменить реальные зависимости на fake-объекты, которые возвращают заранее определенные результаты или вызывают заданные методы, имитируя тем самым работу внешних систем. Это упрощает процесс тестирования и ускоряет разработку, позволяя сосредоточиться на проверке внутреннего функционала приложения, не заботясь о подключении и настройке внешних зависимостей.

## Задание 2.

У вас есть класс BookService, который использует интерфейс BookRepository для получения информации о книгах из базы данных. Ваша задача написать unit-тесты для BookService, используя Mockito для создания мок-объекта BookRepository.
