# Стратегия выбора S-пар в алгоритме F4.

Вычисление базиса Грёбнера полиномиального идеала является вычислительно трудной задачей. Для её решения был предложен ряд алгоритмов, и все они опираются на какие-нибудь эвристики на разных шагах. Возникает идея с помощью машинного обучения делать в этих местах оптимальный выбор, и за счёт этого получать базис Грёбнера быстрее.

Одним из наиболее быстрых алгоритмов вычисления базиса Грёбнера является алгоритм F4. Он был предложен французским математиком Ж.-Ш. Фожером в 1999 году (его работу можно найти по ссылке http://www-polsys.lip6.fr/~jcf/Papers/F99a.pdf). В процессе своей работы этот алгоритм допускает свободу в выборе рассматриваемых на текущей итерации S-пар. Это привело к идее применить машинное обучение для создания оптимальной стратегии выбора S-пар.

В файле Strategy.ipynb приведён полный код, использовавшийся для создания стратегии и поставновки экспериментов. Файл выполнен в стиле лабораторной и имеет следующую структуру: сначала идёт весь код, потом продемонстировано его использование с подробными текстовыми комментариями. Файлы формата .pkl -- это сохранённые датасеты, которые можно загружать для обучения на них классификатора. Код использует классы, реализованные в Sage, поэтому вне Sage он работать не будет.
