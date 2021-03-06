# HW1_3D_Platformer
__Платформы__: ПК (Windows 10)   
__Технологии__: Unreal Engine 4.24.3  
__Язык__: английский   
__Аудитория__:   
*	Люди, владеющими базовыми знаниями о работе с компьютером
*	Малый доход
*	Отсутствует мощный ПК
*	Нужно отвлечься на малое количество времени
*	Устойчивая психика  
__Жанр__: 3D платформер  
__Настроение__: общий сеттинг должен напоминать о природе – спокойствие, умиротворенность. Элементы для усложнения игры добавить чувство приключения – напряженность, осторожность.  
__Эмоции__: по мере усложнения игры (повышения уровня) у игроков чувство спокойствия сменяется напряжением и раздражительностью. Иногда возникает испуг.  
__Возрастное ограничение__: 10+   
__Количество пользователей__: single-player   
__Длительность игры__: 5 минут  
__Главная игровая механика__: собрать максимальное возможное количество игровых момент, избегаю препятствий   
 
## Описание игровых механик и управления
Передвижение персонажем: ASD –влево- резко вниз -вправо, Space – прыжок.  
Игрок может двигаться внутри линии равномерно, с помощью клавиш A и D. Для изменения линии внутри платформы, когда есть стены, нужно прыгнуть (нажать Space) и в воздухе, с помощью клавиш A и D, выбрать нужную линию. Данная идея была взята из Subway Surf и Fall Guys. Помогает сделать движение разнообразным, увеличивает возможность разнообразия геймплея.

## Взаимодействия с предметами
Игрок должен соприкоснуться с различными предметами с помощью персонажа.  
Результат взаимодействия зависит от типа предмета:
*	Каменное кольцо – увеличение игрового счетчика “Coins” на 1
*	Сосуд с золотой жидкостью – прохождение через стены на 3 сек.
*	Изумруд – замедление всех движущихся объектов.
*	Куст – смерть игрового персонажа и начало уровня заново.
*	Стрелы – смерть игрового персонажа и начало уровня заново.
Идея с препятствиями и монетами была взята из Subway Surf. Делает игру интереснее и сложнее. У игроков появляется цель.

## Карта игрового процесса 
[См. изображение map](https://drive.google.com/drive/folders/1KM-xP-96VGggze-o45CarkxPHAtFyzry?usp=sharing)

## Визуал 
[См. папку Images](https://drive.google.com/drive/folders/1KM-xP-96VGggze-o45CarkxPHAtFyzry?usp=sharing) 
 
 ## Дизайн уровней 
Количество уровней: Неограниченное количество.  
Уровни генерируются по ходу игры. После того, как игрок прошел 10 плит, генерируется новый уровень.   
В игре существуют 4 вида плит:
*	Плита обычная.
*	Плита с пуском.
*	Плита с подъемом.
*	Плита с пропастью.

Во время игры на плите может генерироваться:
*	Ничего
*	Монетки. 
*	Сосуд. 
*	Изумруд. 
*	Стрела. 

## Баланс
Название|	Значение min|	Значение max|	С каждым новым уровнем изменяется| 	Комментарий
--------|-------------|-------------|----------------------------------|-------------
HP|	1 |	1 |	0	
Скорость игрока|	600 |	2000|	*1.03|	По ходу игры увеличивается
Вероятность монеток|	0.5 |	0.5 |	0	|
Вероятность сосуда|	0.0083|	0.078 |	-0.005 |	По ходу игры уменьшается
Вероятность изумруда |	0.0083 |	0.078	| -0.005|	По ходу игры уменьшается
Вероятность стрела|	0.0 |	0.9|	+0.05|	По ходу игры увеличивается
Вероятность ничего| 	0.03|	0.33|	-0.02|	По ходу игры уменьшается
Вероятность куста| 	0.03|	0.33|	-0.02|	По ходу игры уменьшается
Вероятность обычной плиты|	0.03|	0.32|	-0.02|	По ходу игры уменьшается
Вероятность плиты с подъемом|	0.03|	0.32|	-0.02|	По ходу игры уменьшается
Вероятность плиты с пуском|	0.03|	0.32|	-0.02|	По ходу игры уменьшается
Вероятность плиты с пропастью|	0.05|	0.9|	+0.05|	По ходу игры увеличивается

## Ссылки на используемые assert и учебный материал
[Ancient Treasures](https://www.unrealengine.com/marketplace/en-US/product/9efde82ef29746fcbb2cb0e45e714f43)  
[Human Vocalization](https://www.unrealengine.com/marketplace/en-US/product/human-vocalizations)
[Туториал, по которому делался проект](https://www.youtube.com/playlist?list=PLZlv_N0_O1gbY4FN8pZuEPVC9PzQThNn1) 
