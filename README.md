## Описание проекта

Игра memory cards в тематике смешариков.

### Структура

В проекте используется паттерн MVC со следующими составляющими:

#### Model:
* GameField (игровое поле) (ячейки, )
    * width (ширина поля в клетках)
    * height (высота поля в клетках)    
    * cells (двумерный массив ячеек)
 
* Cell (ячейка) (состояния - открыто, закрыто, не играет)
    * status
    * x (координата по горизонтали)
    * y (координата по вертикали)
    * id (уникальный идентификатор для определения одинаковых карточек)
* Timer (Таймер) (показывает сколько секунд осталось у игрока)
    * seconds (сколько времени у игрока осталось)

* MoveCounter (счётчик ходов)
    * count (количество сделанных ходов)


#### Controller:

* MoveController (получает ячейку, с которой взаимодействует игрок)

* WinnerController (проверяет закончилась ли игра)

#### View:

* WindowView (в нём отображается игровое поле)
    * cellSize (размер ячейки в пикселях)

#### Ресурсы:

* Картинки игровых персонажей
* Картинка "рубашки" карт
* Картинка фона