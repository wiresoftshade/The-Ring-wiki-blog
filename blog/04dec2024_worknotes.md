4 декабря 2024 г.

# Изменил масштаб кораблика Hummer. Что из этого получилось

Мне нравится новый размер корабля. Струи газа движков выглядят лучше. 

## Что сделано

- переэкспортил меши (SM, SKM) с установкой параметра экспорта и изменением `Import Uniform Scale = 5.0`. 
- заскейлил коллизии, удалил старые файлы с кусочками коллизий.
- переэкспортил анимации так же со скейлом
- передвинул референсные точки с который в конструкторе кораблика расставляются пушки и лазеры.
- расширил диапазон внешней камеры игрока.
- поправил масштабы на карте BaseMetrics.

**надо будет при домоделивании не забыть, что весь масштаб увеличился на 5.0**

## Какие остались проблемы

- увеличился вес кораблика. Так и не понял как поправить это. Не понятно что влияет на него. Надо будет потестить где-то в пустом проекте это. 
- кораблик в сценах с орбитами закручивает. Есть подозрение, что он сталкивается с камерой. Это надо проверить. Колизия с камерой не изученая вешь у меня. Надо почитать про это. Либо он сталкивается с чем-то еще, потоому как на пустой сцене без колец и др станций все нормально работает.
- так же у него как буд-то есть постоянный момент закручивания. Тоже не понятно с чем связано.