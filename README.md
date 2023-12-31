# Проведение А/В тестов
### Предварительное проведение А/А тестов
У нас есть данные А/А-теста с '2023-07-23' по '2023-07-29'. Мы делаем симуляцию, как будто мы провели 10000 А/А-тестов. На каждой итерации сформированы подвыборки без повторения в 500 юзеров из 2 и 3 экспериментальной группы, проводим сравнение этих групп при помощи т-теста

Порядок действий:
- Построила гистограмму распределения получившихся 10000 p-values.
- Посчитала, какой процент p values оказался меньше либо равен 0.05
- Выводы по проведенному А/А-тесту, корректно ли работает наша система сплитования.

### Проведение А/В тестирования
Эксперимент проходил с 2023-07-30 по 2023-08-05 включительно. Для эксперимента были задействованы 2 и 1 группы. В группе 2 был использован один из новых алгоритмов рекомендации постов, группа 1 использовалась в качестве контроля. 
Гипотеза заключается в том, что новый алгоритм во 2-й группе приведет к увеличению CTR. 

Порядок действий:
- Проведение А/А тест
- Построение гистограммы распределения целевой метрики для обеих групп
- Выбор теста и его реализация
- Выводы

### Проведение А/В теста, использую метрики отношений
Анализируем тест между группами 0 и 3 по метрике линеаризованных лайков и тест между группами 1 и 2 по той же метрике
Эксперимент проходил с 2023-07-30 по 2023-08-05 включительно

