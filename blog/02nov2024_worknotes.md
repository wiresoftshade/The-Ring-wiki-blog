2 ноября 2024

# Оставлю тут вот что: У меня получилось! 

_О переходе на движок версии 5.4 с 4.27_

Долго пришлось ставить все назад... _Студия почему-то удалила каждую софтину, что была установлена с EpicGamesLauncher. И три движка и игры._

Движки поставил, студию переставил. И к моей печали все выглядело так же как было с теми же проблемами. 
Я стал по-порядку делать, что сказал Ваня: 

**(1)** Сначала проверял на пустом проекте. Создал один пустой с++ компонент. Хотя пустой проект у меня так и не компилился, я решил вернуться к проекту `TheAsteroids`. 
**(2)** Пробовать менять `Target` файл как Ваня писал в двух первых сообщениях. 
Не компилился. Потом я уж совсем отчаялся, но закрыл движок и в открытой студии нажал `Build`. 
Ничего хорошего уже не ожидая, увидел как стали появляться строки такого вида: 

```log 
...
2>[2/15] Compile [x64] SharedPCH.UnrealEd.Project.ValApi.Cpp17.cpp (0:29.78 at +0:00)
2>[3/15] Compile [x64] TheAsteroids.cpp (0:00.78 at +0:29)
2>[4/15] Compile [x64] TheAsteroids.init.gen.cpp (0:00.79 at +0:29)
2>[5/15] Compile [x64] OrbitData.cpp (0:00.85 at +0:29)
2>[6/15] Compile [x64] OrbitPars.cpp (0:00.87 at +0:29)
2>[7/15] Compile [x64] OrbitParameters.cpp (0:00.89 at +0:29)
2>[8/15] Compile [x64] OrbitParameters.gen.cpp (0:01.00 at +0:29)
2>[9/15] Compile [x64] OrbitSolver.gen.cpp (0:01.01 at +0:29)
2>[10/15] Compile [x64] OrbitPars.gen.cpp (0:01.03 at +0:29)
2>[11/15] Compile [x64] OrbitSolver.cpp (0:01.09 at +0:29)
2>[12/15] Compile [x64] OrbitData.gen.cpp (0:01.12 at +0:29)
...
```

А потом я увидел это: 

```log
2>---------------------- Done ----------------------
2>
2>    Rebuild All: 1 succeeded, 0 failed, 0 skipped
2>
2>1 build system warning(s):
2>   - License not activated
2>
2>Total time in XGE executor: 32.01 seconds
2>Total execution time: 35.68 seconds
2>Done building project "TheAsteroids.vcxproj".
========== Build: 1 succeeded, 0 failed, 0 up-to-date, 1 skipped ==========
========== Build completed at 3:14 and took 36.932 seconds ==========
```

Давно не ощущал такого "камня с плеч") Сначала не верил даже. Я вообще не понял почему он собрался. Стал просматривать все файлы... Короче в результате все запускается, кораблик летает. Сработало, но я совершенно не знаю почему😠. Бесит😄.

Теперь у меня будет: 
- трассировка лучей, 
- крутые тени, 
- big world coordinate system, 
- substrate. 
- nanite
- lumen
- нов. input
- и новые проблемы) Как же без них)

Много текста, много эмоций) 

![alt text](images/photo_2024-11-03_18-01-12.jpg)
