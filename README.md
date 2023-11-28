# erw-150
FUNAI FUJI ERW 150 Agcen xf150 esphome<br>
Так как мне надоело, что данное устройство после выключения пропадало из wi-fi сети то решил его отвязать от облака Tuya и перенести в Esphome.<br>
Дополнительно получаем отличную работу в Home Assistant.<br>
У меня модель FUNAI FUJI ERW-150 в интернете я нашёл его толи клон толи родителя под маркой Agcen xf150.<br>
Все эти модели умеют управляться как через ИК пульт так и с помощью приложения SmartLife (и его клоны).<br>
Так как я уже успользовал данное устройство в LocalTuya то уже знал какие DP за что отвечали.<br>
<br>
Datapoint 1: switch (value: OFF) #Включение/Выключение<br>
Datapoint 2: enum (value: 0) #Режим работы<br>
Datapoint 4: switch (value: OFF) #Подсветка<br>
Datapoint 5: switch (value: OFF) #Ионизатор<br>
Datapoint 9: int value (value: 24) #Температура входящая<br>
Datapoint 13: switch (value: OFF) #Приглушение подсветки (в самой программе не используется, но я его вывел)<br>
Datapoint 18: bitmask (value: 0) #noname (так и не нашёл для чего оно)<br>
Datapoint 23: enum (value: 0) #Air Quality (показывает в виде 0, 1, 2, 3. Значения качества. Я не использую его в коде, написал свой вариант)<br>
Datapoint 102: enum (value: 1) #Регулировка клапана<br>
Datapoint 103: switch (value: OFF) #Сброс таймера фильтра<br>
Datapoint 104: int value (value: 1) #Положение клапана<br>
Datapoint 7: int value (value: 15) #TVOC<br>
Модуль оригинала я простов снял и собрал всё на esp8266. Просто потому, что у меня он был, а перепаивать чип в оригинале я не хотел.<br>
Собран он на WBR3 и можно его заменить на ESP12F<br>
