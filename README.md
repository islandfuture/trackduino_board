# trackduino_board


Благодаря [инструкции от Роботоша](http://robotosha.ru/arduino/install-core-arduino-ide.html)
и Роботрек IDE установленной на Windows - удалось собрать небольшую библиотеку для установки
платы Trackduino v2 на Arduino IDE под MacOS.


## Установка

Скачиваете архив к себе на Мак. Разархивируете. Внутри обнаруживаете две подпапки:
robotrack и tools.

Далее необходимо найти подпапку hardware в папке с Arduino IDE.
В Mac OS папка скрыта внутри пакета приложения. Для того, чтобы найти ее делаем правый клик на приложении Arduino IDE и выбираем "Показать содержимое пакета"
![Показать содержимое пакета](http://robotosha.ru/wp-content/uploads/2015/03/inside_application_macos.png)

Переходим внутри по вложенным подпапкам Contents → Java и находим там папку hardware.
Внутрь нее копируем папку Robotrack. Потом в папке tools/avr/etc находим файл avrdude.conf
и сравниваем его с таким же файлом из этого исходника.
Дописываем что не хватает (на всякий случай делаем копию оригинального файла).

Все! Загружаем Arduino IDE и в Меню Tools -> Boards должен появится раздел Robotrack
и в нем плата Trackduino v2 (http://prntscr.com/mbqzic)

Выбираем ее и начинаем заливать.
