Пишем юниты
**1. Создайте скрипт который создаёт папку заполняет её файлами ( имена 1-4 ) и записывает в них информацию о текущей дате, версии ядра, имени компьютера и списе всех файлов в домашнем каталоге пользователя от которого выполняется скрипт( не забудьте сдлеать проверку на существование файлов и папок)**

<img width="325" height="24" alt="image" src="https://github.com/user-attachments/assets/c4a6e00a-e20d-4cc9-9535-b7aa8fde72df" />

Скрипт собирает инфу о системе и пишет её в файлы.

Сначала он заходит в домашнюю папку. Потом создаёт папку `info_dir`, если её нет.

Затем собирает четыре типа данных:
1. Текущая дата и время
2. Версия ядра
3. Имя компа в сети
4. Что лежит в домашней папке

Дальше циклом создаёт четыре файла: info1.txt, info2.txt, info3.txt, info4.txt.
В каждый файл закидывает соответствующую инфу, перезаписывая старое содержимое.

В итоге в папке info_dir появляются файлы с актуальной системной информацией.

<img width="505" height="710" alt="image" src="https://github.com/user-attachments/assets/c01c8a18-f6b8-443b-a723-69d981d7d5c9" />

<img width="561" height="377" alt="image" src="https://github.com/user-attachments/assets/d52eff22-84b3-488f-b251-7440aecd5ab8" />
<img width="569" height="319" alt="image" src="https://github.com/user-attachments/assets/a13a2e08-78c5-467b-bccc-26ff60b372f8" />
<img width="639" height="746" alt="image" src="https://github.com/user-attachments/assets/c06875e9-2728-4156-8f6f-26461dcec35d" />
