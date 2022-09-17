# simple-pc-analize

---

<img src="image/apps.png" />

Консольная программа для сбора информации о компьютере и записи ее в файл журнала.

Программа предназначена только для **ОС Windows**. Для реализации использован **Python** версии **3.8.9 и старше**.

<img src="image/win-7-icon.svg" /> <img src="image/win-10-icon.svg" /> <img src="image/python-3.8.9-icon.svg" />

<a name="Oglavlenie"></a>

## Оглавление

1. [Введение](#Intro)
2. [Зависимости](#Dependencies)
3. [Компиляция](#Compilation)
4. [Использование](#Uses)
5. [Обо мне](#About)

## <a name="Intro">Введение</a>

Данная программа предназначена для сбора минимально необходимой информации о ПК для какой-либо организации. Да, существуют масса утилит подобного характера. Однако, именно эта программа должна заменить использование сразу нескольких приложений. 

В подавляющем большинстве случаев в *Windows* существуют масса сбоев различных драйверов при частом к ним обращении из приложений пользователей. 

В достаточно старых ПК (например, с оперативной памятью DDR-2) довольно часто происходят сбои связанные с принтерами. 

В организациях при частых операциях, связанных с файлами, необходимо регулярно контролировать **уровень фрагментации локальных дисков**, а также состояние **SMART** этих дисков и оставшееся свободное место.

При использовании доступов к тем или иным базам данных в организациях часто можно встретить переадресацию в файле **hosts**, который также необходимо контролировать. В связи с чем возникает и следующая необходимость контролировать доступ к веб-адресам этих баз данных. В случаях сбоя - сразу же устранять неисправность.

Далеко не все утилиты диагностики подерживают весь указанный функционал. А если учесть постоянное расширение доступов к различным ресурсам и необходимость контроля последних - очевидна необходимость универсального решения, которое и призвана решить данная программа.

---

[К оглавлению](#Oglavlenie)

## <a name="Dependencies">Зависимости</a>

В программе автоматически определяется архитекутура **ОС**.

Внутри директории **src** программы обязательно должны присутствовать следующие папки и файлы. Без них программа работать не будет. Скачанные архивы и **exe** файлы для работы не нужны, т.е. их в последствии можно будет удалить.

* ListPrinters ([Git ссылка](https://github.com/maximalisimus/ListPrinters.git))
* FastPing ([Git ссылка](https://github.com/maximalisimus/FastPing.git))
* udefrag-x64 ([Sourceforge.net](https://sourceforge.net/projects/ultradefrag/files/stable-release/))
* udefrag-x86 ([Sourceforge.net](https://sourceforge.net/projects/ultradefrag/files/stable-release/))
* smartmontools ([Sourceforge.net](https://sourceforge.net/projects/smartmontools/files/smartmontools/))
* ping-list.txt
* structure.txt

<img src="image/scr-1.png" width="800px">

А теперь о каждом пункте отдельно. Начнем с конца.

**structure.txt** - Вы можете не использовать структурирование файлов журнала по структуре организации, но файл в папке с программой обязательно должен присутствовать. 

**ping-list.txt** - то же самое касательно пингов различных веб адресов. Пинги можно отключить соответствующим ключом, или просто оставить в файле буквально 1...2 строчки. Однако, файл обязательно должен присутствовать.

<img src="image/BorlandCpp.png" height="32"> <img src="image/printers_icon.ico" height="32"> **ListPrinters** - отдельная программа написанная на **C++Buileder**-ре <img src="image/cpp-builder-icon.svg">.
 
 Компилировать её не нужно. Написана мною. Просто скачайте последнюю [Relese версию](https://github.com/maximalisimus/ListPrinters/releases/download/v1.0.0.0/ListPrinters-win-x86.exe) в папку **src**. Не нужно создавать никаких директорий. Данный *exe* является архивом, который упакован *7z* как *sfx* архив. Внутри уже имеются все необходимые файлы и папки для работы программы. 
 
 Поэтому просто запустите его внутри **src** папки и распакуйте.
 
 <img src="image/scr-3.png" width="800px">
 
 <img src="image/BorlandCpp.png" height="32"> <img src="image/icmp-icon.ico" height="32"> **FastPing** - также отдельная программа написанная на **C++Buileder**-ре <img src="image/cpp-builder-icon.svg">.

 Компилировать её не нужно. Написана тоже мною. Просто скачайте последнюю [Relese версию](https://github.com/maximalisimus/FastPing/releases/download/v1.0.0.0/FastPing-win-x86.exe) в папку **src**. Не нужно создавать никаких директорий. Данный *exe* является архивом, который упакован *7z* как *sfx* архив. Внутри уже имеются все необходимые файлы и папки для работы программы. 
 
 Поэтому просто запустите его внутри **src** папки и распакуйте.

<img src="image/scr-2.png" width="800px">

**udefrag-x64** и **udefrag-x86** являются частью утилиты **UltraDefrag Files**.  Эту портативную версию утилиты в зависимости от архитектуры можно скачать с сайта *SorceForge.Net*. Однако, вся утилита не нужна. 

В списке выше указана ссылка на все версии утитилы, чтобы можно было выбрать последнюю. На данный момент последней является версия **7.1.4**.

Скачать необходимо 2 архива:
* с окончанием *bin.i386.zip*, например [этот](https://sourceforge.net/projects/ultradefrag/files/stable-release/7.1.4/ultradefrag-portable-7.1.4.bin.i386.zip/download)
* и с окончанием *bin.amd64.zip*, например [этот](https://sourceforge.net/projects/ultradefrag/files/stable-release/7.1.4/ultradefrag-portable-7.1.4.bin.amd64.zip/download)

Далее, в папке *src* создайте 2 директории - *udefrag-x64* и *udefrag-x86*. После этого распакуйте файлы программы *Ultra defrag* в эти папки по архитектурам. Нужны не все файы. 

Вот список необходимых файлов любого архива:
* conf
* po
* scripts
* lua5.1a.dll
* lua5.1a.exe
* lua5.1a_gui.exe
* udefrag.dll
* udefrag.exe
* zenwinx.dll

Папка **reports** создаётся автоматически в процессе работы.

<img src="image/scr-4.png" width="800px">

<img src="image/scr-5.png" width="800px">

**smartmontools** - 

---

[К оглавлению](#Oglavlenie)

## <a name="Compilation">Компиляция</a>



---

[К оглавлению](#Oglavlenie)

## <a name="Uses">Использование</a>



---

[К оглавлению](#Oglavlenie)

## <a name="About">Обо мне</a>

The author of this development **Shadow**: [maximalisimus](https://github.com/maximalisimus).

Author's name: **maximalisimus**: [E-Mail](mailto:maximalis171091@yandex.ru).

Date of creation: **19.08.2022**