# parser

Язык: Python

Функционал: выполнены все требования, включая bonus 1 и 2

Задачи:

а. Разработать программу на языке Python, выполняющую разбивку входной строки на список строк, так чтобы в каждой из полученных строк было не более указанного количества символов и не нарушались правила разбиения (см. далее).

Формат входной строки:
Обновленный рейтинг за 27.04.2022 по данным из :snake:МЛНИ:
- Новый score пользователя @Панфилкин Артём: 1
- Новый score пользователя @Журов Константин: 1
- Новый score пользователя @Погуляка Даниил: 1337
- Новый score пользователя @Миронов Кирилл: 1
- Новый score пользователя @Бураков Сергей: 1
- Новый score пользователя @Гаджиев Важид#4881: 1
Scoreboard взял отсюда: https://discord.com/channels/690164243685048457/806462228207239179/941307720076783686


Требования к выполнению:

По пункту а:
Входная строка содержится в файле, путь к которому передается через аргумент командной строки с ключом -f
Максимальное количество символов в подстроке задается через аргумент командной строки с ключом -n (по умолчанию параметр имеет значение 200)
При реализации программы должны быть сделаны проверки на некорректность передаваемых данных и в случае некорректно заданных параметров - должны быть выведены user-friendly сообщения об ошибке.
Входная строка должна быть разделена по максимальному количеству символов, с учетом следующих правил:
Не допускается разделение на разные подстроки "по середине" тега пользователя.
Не допускается разделение на разные подстроки ссылок, даты, слов.
В результате работы программы в консоль должны быть распечаты полученные подстроки в следующем формате:
Substring #1:
    Обновленный рейтинг за 27.04.2022 по данным из :snake:МЛНИ:
    - Новый score пользователя @Панфилкин Артём: 1
    - Новый score пользователя @Журов Константин: 1

Substring #2:
    - Новый score пользователя @Погуляка Даниил: 1337
    - Новый score пользователя @Миронов Кирилл: 1
    
Substring #3:
    - Новый score пользователя @Бураков Сергей: 1
    - Новый score пользователя @Гаджиев Важид: 1

Substring #4:
    Scoreboard взял отсюда: https://discord.com/channels/690164243685048457/806462228207239179/941307720076783686

Код должен быть разделен на не менее, чем 3 функции
Функциональность разбиения входной строки и вывод выходных строк должна быть разделена на разные функции в Python, т.е. не допускается использовать print для вывода выходных строк (только для логирования)
Если строка не может быть разбита с учетом заданных ограничений, то в консоль должно быть выведено user-friendly сообщения об ошибке.

Bonus 1:
Добавить параметр командной строки -l, при указании которого добавляется дополнительное правильно на разбиение на подстроки:
Не допускается разбиение "по середине" строки указывающей новый score пользователя, например - Новый score пользователя @Погуляка Даниил: 1337

Bonus 2:
Добавить параметр командной строки -d, при указании которого выходные подстроки сохраняются в различные файлы в директории указанной в данном параметре. Имена файлов задаются в формате substring_<index>.txt

Общие требования

Код должен быть логически структурирован и разделен на функции
