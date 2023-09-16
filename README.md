# Климатическая система бани
Climate control algorithm for 2-floor building with bedroom

Программа управления отоплением и вентиляцией двухэтажного дома с тремя зонами контроля (1 этаж, спальня на 2 этаже, туалет с собственным термостатом по Modbus) для программируемого реле (мини-ПЛК) Овен ПР200. Разработка осуществляется в среде OWEN Logic.
## Описание системы
Управление осуществялется с целью минимизации потребления электроэнергии при поддержании комфорных условий проживания. Программа ориентирована на тарифное расписание Московской области с временем действия ночного тарифа 23:00 - 7:00.

### Исполнительные устройства:
* через внешние контакторы:
  * конвекционный электрообогреватель 1 этажа (через внешний контактор);
  * конвекционный электрообогреватель 2 этажа (через внешний контактор);
  * водонагреватель (через внешний контактор);
  * инфракрасный потолочный обогреватель в туалете (через термостат, управляемый по Modbus);
* через встроенные реле:  
  * ночники;
  * вентилятор подачи атмосферного воздуха;
  * вентилятор внутренней циркуляции;
* кондиционер через modbus модуль WirenBoard WB-MIRv2.

### Устройства ввода:
* датчики движения на 1 и 2 этажах;
* реле контроля тока (Меандр РКТ-1) в линии освещения;
* контакт открытия форточки (предположительно геркон);
* датчики температуры (NTC термистор на 1кОм):
  * улицы;
  * 1 этажа;
  * 2 этажа (только нижний) - два на разном уровне для программного перемещения точки поддержания температуры;
* термометр-гигрометр с экраном и передачей данных по Modbus - верхний датчик температуры на 2 этаже.
## Совместная разработка и использование
Так как проект абсолютно индивидуальный, разрабатываемый специально для моей бани, не вижу смысла в его развитии силами сообщества. Вы можете свободно использовать его как целиком, так и его отдельные идеи.
