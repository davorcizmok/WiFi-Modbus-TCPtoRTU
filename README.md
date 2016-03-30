# WiFi-Modbus-TCPtoRTU
WiFi ESP8266 gateway Modbus TCP to Modbus RTU 

Задание:
- устройство подключаются через беспроводное соединение (WIFI) по интерфейсу uart или rs-485 к различным устройствам для передачи протокола Modbus.
- Устройство должно быть небольших размеров и записываться от устройства подключения.
- Устройство должно обеспечить подключение не более 4 мастер устройств одновременно.
- Устройство должно поддерживать совмещение запросы от мастера (Когда в одном TCP пакете присутствует больше одного Modbus запроса).
- Устройство должно поддерживать одно соединение telnet для настройки и диагностики.

Реализация:
- железная часть взята плата китайского производства ESP-01 с модулем WiFi ESP8266 1 MB.
- Программа пишется на espressos SDK под arguing.
- Используется platform io.

Первая версия программы протестировать на с использованием программ Modbus pull и Modbus slave.

Осталось реализовать:

- Описать метод и функцию настройки через telnet.
- Сохранение в энергонезависимую память настроек порта uart и настроек точки доступа. Для закончиности устройства.
- Сделать модель корпуса для реализации отдельного устройства с интерфейсом rs-485 для печати на 3d принтере.
- Сделать схему питания и самого rs-485 интерфейса.
