# О книге

Эта книга задумана мной как максимально полное описание работы .NET CLR, и частично - .NET Framework и призвана в первую очередь заставить посмотреть читателя на его внутреннюю структуру под несколько другим углом: не так, как это делается обычно. Связано это в первую очередь с утверждением, которое может показаться многим очень спорным: любой разработчик обязан пройти школу C/C++. Почему? Да потому что из высокоуровневых эти языки наиболее близки к процессору и программируя на них начинаешь чувствовать работу программы сильнее. Однако, понимая, что мир устроен несколько иначе и у нас зачастую нет никакого времени изучать то, чем мы не будем напрямую пользоваться, я и решил написать эту книгу, в которой объяснение всех вопросов идет с более глубокой чем обычно - позиции и с более сложными или же попросту альтернативными примерами. Которые помимо своей стандартной миссии - на самом простом коде показать как работает тот или иной функционал - сделать реверанс в альтернативную реальность, показав что все сильно сложнее чем может показаться изначально. Зачем? Чтобы и у вас возникло чуство понимания работы CLR до последнего винтика.

*автор, Станислав Сидристый*

# Содержание

  1. Common Language Runtime
  2. [Основы менеджмента памяти: пользовательский слой](./MemoryManagementBasics.md)
      1. Стек потока
      2. Heap
      3. RefTypes, ValueTypes, Boxing & Unboxing
      4. Small Objects Heap
      5. Large Objects Heap
      6. Garbage Collection
      7. Statics
  3. Погружаемся в систему типов
      1. Структура объектов
      2. Структура и назначение таблицы виртуальных методов
      3. Generic классы и интерфейсы: строение типов
      4. Как работает приведение типа. Скорость приведения типа.
      5. Вычисление размера ReferenceType. sizeof(reftype).
      6. TBD
  4. Слой управления памятью: как работает CLR
      1. Подробно про Small Objects Heap
          1. Пример: дамп памяти, влияние pinned objects на аллокацию
      2. Large Objects Heap
          1. Пример: как легко испортить кучу, как этого избегать
      3. Stack потока
          1. Пример: запоминаем строение стека путем его редактирования.
      4. Garbage Collection
          1. Mark & Sweep
          2. Оптимизация поколений
          3. Финлизация
          4. Проблемы, связанные с GC и финализацией
          5. [Шаблон Disposable (Disposable Design Principle)](./Disposable.md)
  5. Слой операционных систем: откуда берется память.
  6. Слой процессора: на чем все основано. Общие правила.

# Лицензия
