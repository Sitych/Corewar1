<!-- 1) check.c убрать избыточные проверки на совпадающие символы -->
<!-- 2) дописать usage -->
<!-- 3) защита от подачи не файлов (папок и так далее) -->
4) обработка подачи файла с пустым названием (".s")
5) разнести чеки по разным файлами

6) Нужно передавать структуру и инициализировать флаги (-а, -h, -j)
7) ft_file_read: !!!либо должен вернуть оригинальный файл со всеми пустыми строками для обработки ошибок!!!, либо должен вернуть два файла (оригинальный и рабочий)
8) Упростить (переписать) parse_header.c
9) посчитать количество строк с инструкциями в файле с девственным видом и передать в parse_body в качестве int all_lines
10) подумать над финальным видом структуры t_body

НЕ СТЕСНЯЕМСЯ ДОПИСЫВАТЬ ПО ХОДУ ДЕЛА
1) Предложение error.h заменить на глобал массив строк с ошибками вместо define

DONE:
1) В check.c добавлена проверка, что символы не пробелы. Добавлена проверка, что EXEC_MAGIC не больше UINT32
2) В error.h добавлен usage. Файл с именем .s тоже нормально читается
