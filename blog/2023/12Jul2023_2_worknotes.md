12 июля 2023 г. 

# Про кораблик. Моделька, anims, jets

DONE [Моделька корабля игрока](https://app.asana.com/0/1200236593655828/1202432063092074)

Про модельку: Сделан драфт. Анимация радиатора. ветка в работе. нужна анимация открывания ракет. На той неделе был занят анимациями радиаторов. Сначала сделал в блюпринте на логике при помощи процед. построй. мешек, но было не точно и трудно управлять. Выкинул все и сделал скелетал меш чисто для радиаторов. Сделал анимацию. причем одну. В анриле сделал композицию, чтобы крутилась в другую сторону. Теперь надо то же повторить для Ракетниц на носу. Все в один СКМ и чтобы анимации было две. Чтоб запускать их отдельно или вместе на одном скелете. Надо будет понять как так делать.  

**Что как работает:** Итак есть ShipProxy в нем главная mesh к нему "аттачим" Skeletal mesh. 

Получилось разделение на статичную, но симулируемую физикой часть корабля и анимируемую часть. 

**Есть проблема** с отсутствием не директной тени у СКМ, но ее можно решить аттачем не рендереных мешек к нужным костям
[Логика работы Реакт, струй двигателей Thruster и RCS](https://app.asana.com/0/1200236593655828/1202477326355182)
Немного оформил маленькие струи до кучи. Использовал искры из стартер контента. пока такая заглушка будет. Не знаю пока как решать основной двигатель. там крупный вид и надо чтоб объем был красиво заполнен. не знаю пока. 

**Сделаны** просто партиклы, запускаются логикой только при поступательном движении корабля. 

**Не поставлены** на места и **не работают** при поворотах.

![alt text](images/12Jul2023_image.jpg)

![alt text](images/12Jul2023_image2.jpg)

*Дополнение wiReSoftshade · 17 Jul, 2023*

Допилил анимацию открывания ракетниц. Только вот что делать с анимациями. Не знаю как воспроизводить вразнобой. Понял, что нужно делать AnimationBlueprint но там надо разбираться.