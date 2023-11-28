# erw-150
FUNAI FUJI ERW-150 Agcen xf150 esphome
<br>
Так как мне надоело, что данное устройство после выключения пропадало из wi-fi сети то решил его отвязать от облака Tuya и перенести в Esphome.
<br>
Дополнительно получаем отличную работу в Home Assistant.
<br>
У меня модель FUNAI FUJI ERW-150 в интернете я нашёл его толи клон толи родителя под маркой Agcen xf150.
<br>
Все эти модели умеют управляться как через ИК пульт так и с помощью приложения SmartLife (и его клоны).
<br>
Так как я уже успользовал данное устройство в LocalTuya то уже знал какие DP за что отвечали.
<br>
Datapoint 1: switch (value: OFF) #Включение/Выключение
Datapoint 2: enum (value: 0) #Режим работы
Datapoint 4: switch (value: OFF) #Подсветка
Datapoint 5: switch (value: OFF) #Ионизатор
Datapoint 9: int value (value: 24) #Температура входящая
Datapoint 13: switch (value: OFF) #Приглушение подсветки (в самой программе не используется, но я его вывел)
Datapoint 18: bitmask (value: 0) #noname (так и не нашёл для чего оно)
Datapoint 23: enum (value: 0) #Air Quality (показывает в виде 0, 1, 2, 3. Значения качества. Я не использую его в коде, написал свой вариант)
Datapoint 102: enum (value: 1) #Регулировка клапана
Datapoint 103: switch (value: OFF) #Сброс таймера фильтра
Datapoint 104: int value (value: 1) #Положение клапана
Datapoint 7: int value (value: 15) #TVOC
Модуль оригинала я простов снял и собрал всё на esp8266. Просто потому, что у меня он был, а перепаивать чип в оригинале я не хотел.
Собран он на WBR3
