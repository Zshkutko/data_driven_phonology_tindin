# Курсовая работа студентки 2 курса образовательной программы "Фундаментальная и компьютерная лингвистика" Шкутько Златы на тему Фонология тиндинского языка: от словарных данных к обобщениям.
## Алгоритм работы программы:
На входе программа получает файл "tin_slovar.html" в формате html.
На выходе программа создает таблицы с данными в формате csv.
Программа написана в среде Jupyter notebook в формате ipynb, поэтому для ее открытия следует использовать эту же среду.
### Считывание и подготовка данных:
Файл читается построчно. Далее элементы группируются по тэгам <p> на словарные статьи с помощью библиотеки BeautifulSoup. Из словарных статей достаются нужные компоненты и заносятся в таблицу: леммы, морфологии, переводы. Затем в двоичном варианте (1;0) ставятся пометки на заимствование и заимствованные слова не участвуют в дальнейшем анализе. Далее создается вариант лемм в IPA и тоже заносится в таблицу. 3атем выявляются инициаль, финаль слов и тоже заносятся в таблицу.
### Анализ данных
В ходе работы программа производит анализ с помощью различных методов библиотеки pandas. Графики составляются с помощью Matplotlib. Также при анализе используется модуль Re и библиотека Collections.
