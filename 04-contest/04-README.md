Problem up04-1: mz04-1 (upsolving)
Напишите функцию-шаблон prоcess от одного параметра-типа: контейнера STL с двунаправленным итератором. Функция должна вернуть сумму (то есть результат применения operator + или +=) последнего, третьего с конца и пятого с конца элемента контейнера. Если в контейнере недостаточно элементов, берутся только существующие. Если контейнер пуст, результатом будет значение по умолчанию типа элементов.


Problem up04-2: mz04-2 (upsolving)
Напишите шаблонную функцию myfilter, которая принимает объект контейнерного класса и функцию-предикат. Функция возвращает новый объект того же самого контейнерного класса, в который скопированы только те объекты исходного контейнерного класса, которые удовлетворяют заданному предикату.

Стандартными алгоритмами пользоваться запрещено.


Problem up04-3: mz04-3 (upsolving)
Напишите шаблонную функцию myapply, которая принимает два итератора на начало и конец обрабатываемой последовательности, и функцию f. Шаблонная функция myapply применяет заданную функцию ко все элементам в заданном диапазоне итерации.

Напишите функцию myfilter2, которая принимает два итератора на начало и конец обрабатываемой последовательности, и предикат f. Функция myfilter2 возвращает вектор ссылок на элементы входной обрабатываемой последовательности, которые удовлетворяют заданному предикату.

Если к вектору ссылок, который вернула функция myfilter2, применить myapply, то в случае модификации элементов последовательности в функции, переданной в myapply, на самом деле изменятся элементы, обрабатываемой последовательности, переданной при получении вектора ссылок в функцию myfilter2.

Шаблонные функции должны быть применимы к массивам.

Используйте std::reference_wrapper. Стандартными алгоритмами пользоваться запрещено.


Problem up04-4: mz04-4 (upsolving)
Написать шаблонную функцию myremove, принимающую две пары итераторов: диапазон элементов, содержащих номера удаляемых элементов, диапазон элементов, содержащих элементы, подлежащие удалению. Элементы, подлежащие удалению, в диапазоне нумеруются с нуля. Номера элементов отражают позиции элементов на момент начала работы программы. Если номер повторяется более одного раза, все вхождения, кроме первого, игнорируются. Если номер элемента недопустим, он игнорируется.

Функция возвращает итератор на конец сжатой последовательности во втором контейнере.

Для удаляемых элементов может быть запрещено копирование.

