---

## Front matter

title: "Отчёт по лабораторной работе №4. Создание и процесс обработки программ на языке ассемблера NASM"

subtitle: "Арихитектура вычеслительных систем"

author: " Колосов Даниил Дмитриевич. НБИбд-02-22."
## Generic otions
lang: ru-RU
toc-title: "Содержание"
## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl
## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
 name: russian
 options:
 - spelling=modern
 - babelshorthands=true
polyglossia-otherlangs:
 name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
 - parentracker=true
 - backend=biber
 - hyperref=auto
 - language=auto
 - autolang=other*
 - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
 - \usepackage{indentfirst}
 - \usepackage{float} # keep figures where there are in the text
 - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоение процедуры компиляции и сборки программ, написанных на ассем-
блере NASM.

# Задание


1. В каталоге ~/work/arch-pc/lab04 с помощью команды cp создайте копию
файла hello.asm с именем lab4.asm


2. С помощью любого текстового редактора внесите изменения в текст про-
граммы в файле lab4.asm так, чтобы вместо Hello world! на экран выво-
дилась строка с вашими фамилией и именем.

3. Оттранслируйте полученный текст программы lab4.asm в объектный
файл. Выполните компоновку объектного файла и запустите получивший-
ся исполняемый файл.

4. Скопируйте файлы hellо.asm и lab4.asm в Ваш локальный репозиторий

в каталог ~/work/study/2022-2023/"Архитектура компьютера"/arch-

pc/labs/lab04/. Загрузите файлы на Github.


# Выполнение лабораторной работы


1. Создадим каталог для работы с программами на языке ассемблера NASM

![Рис 1](image/рис1.png){ #fig:001 width=90% }

2. В данном каталоге создаем файл с именем hello.asm.

![Рис 2](image/рис2.png){ #fig:002 width=90% }

3. И откроем этот файл с помощью текстового редактора gedit

![Рис 3](image/рис31.png){ #fig:003 width=90% }

4. Вводим текст из материалов по лабораторной работе №4

![Рис 4](image/рис32.png){ #fig:004 width=90% }


5. NASM превращает текст программы в объектный код.

![Рис 5](image/рис6.png){ #fig:005 width=90% }


5. Скомпилирует исходный файл hello.asm в obj.o и проверяем.

![Рис 6](image/рис7.png){ #fig:006 width=90% }

6. Чтобы получить исполняемую программу, объектный файл необходимо передать на обработку компоновщику


![Рис 7](image/рис8.png){ #fig:007 width=90% }


7. Запустить на выполнение созданный исполняемый файл, находящийся в
текущем каталоге, можно, набрав в командной строке: 

![Рис 8](image/рис9.png){ #fig:008 width=90% }

8. Создайте копию файла 

![Рис 9](image/рис10.png){ #fig:009 width=90% }

9. Проведем подобные действия, которые мы делали с файлом hello.asm, с файлом lab4.asm, чтобы вывести на экран имя и фамилию. Оттрансилурем данный файл в объектный и запустим.

![Рис 10](image/рис12.png){ #fig:010 width=90% }

![Рис 11](image/рис11.png){ #fig:011 width=90% }

9. Загрузим файлы в репозиторий


# Вывод


Мы освоили процедуры компиляции и сборки программ, написанных на ассемблере NASM.


::: {#
:::

