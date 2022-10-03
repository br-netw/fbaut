# conbat - COnfig BAckup Tool\*
\*рабочее название

Программа для автоматического резервного копирования файлов.
## Зависимости
- `Python 3.10` или выше (но может сработать и с более ранними версиями)
- `git`, если нужен соответствующий функционал
## Краткий гайд по использованию
1. Создайте папку где-либо на своём ПК. Копии будут храниться там.
2. Запустите программу: `python3 main.py`
3. Укажите местоположение папки с бэкапами: `> set_rc {полный_путь_к_созданной_папке}`
4. При необходимости можно создать git-репозиторий для удалённых бэкапов.
    1. Сначала создайте репозиторий на GitHub и скопируйте ссылку на него.
    2. Запустите следующую команду: `> git_init {ссылка_на_репозиторий_гх}`
5. Добавьте нужные файлы/папки в список копируемых: `> cache {полный_путь_к_копируемому_объекту}`. Можно перечислять несколько штук через пробел.
6. Запустите копирование: `> backup`

**При последующих запусках программы выполняйте только шаги 3 и 6, если нет надобности добавлять новые файлы.**
