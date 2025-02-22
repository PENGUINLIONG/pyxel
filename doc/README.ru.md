# <img src="images/pyxel_logo_152x64.png">

[ [English](../README.md) | [中文](README.cn.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Português](README.pt.md) | [Русский](README.ru.md) | [Deutsch](README.de.md)]

**Pyxel** -- это игровой движок для Python в стиле ретро.

Благодаря своей простоте, вдохновленной старыми игровыми консолями (например, палитра состоит всего из 16 цветов, и только 4 звука могут быть проиграны одновременно), вы можете легко создавать игры в стиле пиксель-арт.

<a href="../pyxel/examples/01_hello_pyxel.py" target="_blank">
<img src="images/01_hello_pyxel.gif" width="48%">
</a>

<a href="../pyxel/examples/02_jump_game.py" target="_blank">
<img src="images/02_jump_game.gif" width="48%">
</a>

<a href="../pyxel/examples/03_draw_api.py" target="_blank">
<img src="images/03_draw_api.gif" width="48%">
</a>

<a href="../pyxel/examples/04_sound_api.py" target="_blank">
<img src="images/04_sound_api.gif" width="48%">
</a>

<a href="images/image_tilemap_editor.gif" target="_blank">
<img src="images/image_tilemap_editor.gif" width="48%">
</a>

<a href="images/sound_music_editor.gif" target="_blank">
<img src="images/sound_music_editor.gif" width="48%">
</a>

Спецификации Pyxel вдохновлены великолепными [PICO-8](https://www.lexaloffle.com/pico-8.php) and [TIC-80](https://tic.computer/).

Pyxel -- программа с открытым кодом и бесплатна для использовния. За дело!

## Характеристики

- Запускается на Windows, Mac и Linux
- Код пишется на Python
- 16-цветная палитра
- 3 набора изображений 256x256 пикселей
- 8 тайлмапов 256x256 пикселей
- 4 канала с 64 определяемыми пользователем звуками
- 8 музыкальных композиций
- Ввод с клавиатуры, мышки или игрового контроллера
- Редактор изображений и звука

### Цветовая Палитра

<img src="images/05_color_palette.png">

<img src="images/pyxel_palette.png">

## Как установить

Предоставляется два варианта Pyxel, в виде пакета и в виде автономной версии.

### Установка сборки в виде пакета

Версия Pyxel в виде пакета представляет собой модуль расширения для Python.

Рекомендуется знакомым с управлением пакетами Python с помощью команды `pip` и разрабатывающим полноценные приложения на Python.

**Windows**

После установки [Python3](https://www.python.org/) (версии 3.7 или выше) необходимо выполнить следующую команду:

```sh
pip install -U pyxel
```

**Mac**

После установки [Python3](https://www.python.org/) (версии 3.7 или выше) необходимо выполнить следующую команду:

```sh
pip3 install -U pyxel
```

**Linux**

После установки пакета SDL2 (`libsdl2-dev` для Ubuntu), [Python3](https://www.python.org/) (версии 3.7 или выше) и `python3-pip` выполните следующую команду:

```sh
sudo pip3 install -U pyxel
```

Если приведённыё выше способ установки не работает, вы можете собрать пакет Pyxel самостоятельно, установив `cmake` и `rust` и затем выполнив следующую последовательность команд:

```sh
git clone https://github.com/kitao/pyxel.git
cd pyxel
make clean all
sudo pip3 install .
```

### Установка автономной версии

Автономная версия Pyxel представляет собой самостоятельное приложение, не зависящее от Python.

Рекомендуется желающим сразу начать писать код, не отвлекаясь на установку и настройку Python, а также тем, кто непосредственно хочет запускать игры.

**Windows**

Необходимо скачать и запустить последнюю версию установщика для Windows (`pyxel-[version]-windows-setup.exe`) со [страницы загрузки](https://github.com/kitao/pyxel/releases).

**Mac**

После установки [Homebrew](https://brew.sh/) необходимо выполнить следующую последовательность команд:

```sh
brew tap kitao/pyxel
brew install pyxel
```

**Linux**

После установки пакета SDL2 (`libsdl2-dev` для Ubuntu) и установки [Homebrew](https://brew.sh/) необходимо выполнить следующую последовательность команд:

```sh
brew tap kitao/pyxel
brew install pyxel
```

Если приведённыё выше способ установки не работает, вы можете попробовать собрать пакет Pyxel самостоятельно.

### Попробуйте примеры

После установки Pyxel, примеры Pyxel будут скопированы в открытую директорию по выполнении этой команды:

```sh
pyxel copy_examples
```

Список примеров, которые будут скопированы:

- [01_hello_pyxel.py](../pyxel/examples/01_hello_pyxel.py) - Простейшее приложение
- [02_jump_game.py](../pyxel/examples/02_jump_game.py) - Игра прыжков с простейшими ресурсными файлами Pyxel
- [03_draw_api.py](../pyxel/examples/03_draw_api.py) - Демонстрация API для рисования
- [04_sound_api.py](../pyxel/examples/04_sound_api.py) - Демонстрация API для работы со звуком
- [05_color_palette.py](../pyxel/examples/05_color_palette.py) - Цветовая палитра
- [06_click_game.py](../pyxel/examples/06_click_game.py) - Игра с кликами мышкой
- [07_snake.py](../pyxel/examples/07_snake.py) - Змейка с BGM
- [08_triangle_api.py](../pyxel/examples/08_triangle_api.py) - Демонстрация API по рисованию треугольных полигонов
- [09_shooter.py](../pyxel/examples/09_shooter.py) - Игра жанра «убей всех» с переходом между экранами
- [10_platformer.py](../pyxel/examples/10_platformer.py) - Платформер с боковым скроллингом и картой
- [11_offscreen.py](../pyxel/examples/11_offscreen.py) - Offscreen rendering with Image class

Эти примеры могут быть запущены следующей командой:

```sh
cd pyxel_examples
pyxel run 01_hello_pyxel.py
```

## Как использовать Pyxel

### Создание Pyxel-приложения

После импортирования модуля Pyxel в ваш код на Python, сначала укажите размер окна с помощью команды `init`, затем запустите Pyxel-приложение с помощью функции `run`.

```python
import pyxel

pyxel.init(160, 120)

def update():
    if pyxel.btnp(pyxel.KEY_Q):
        pyxel.quit()

def draw():
    pyxel.cls(0)
    pyxel.rect(10, 10, 20, 20, 11)

pyxel.run(update, draw)
```

Агрументы функции `run` -- это функции `update` для обновления внутренней игровой логики каждый кадр и функции `draw` для отображения объектов на экране по мере необходимости.

В самом приложении рекомендуется свернуть код Pyxel в один класс (смотрите пример).

```python
import pyxel

class App:
    def __init__(self):
        pyxel.init(160, 120)
        self.x = 0
        pyxel.run(self.update, self.draw)

    def update(self):
        self.x = (self.x + 1) % pyxel.width

    def draw(self):
        pyxel.cls(0)
        pyxel.rect(self.x, 0, 8, 8, 9)

App()
```

Можно также писать простые програмки, используя функции `show` и `flip` для отображения простейшей графики и анимаций.

Функция `show` выводит изображение на экран и ждет нажатия клавиши `ESC`.

```python
import pyxel

pyxel.init(120, 120)
pyxel.cls(1)
pyxel.circb(60, 60, 40, 7)
pyxel.show()
```

Функция `flip` обновляет изображение на экране единожды.

```python
import pyxel

pyxel.init(120, 80)

while True:
    pyxel.cls(3)
    pyxel.rectb(pyxel.frame_count % 160 - 40, 20, 40, 40, 7)
    pyxel.flip()
```

### Запуск Pyxel-приложения

Созданый сценарий на Python может быть запущен путём выполнения следующей команды:

```sh
pyxel run ИМЯ_PYTHON_ФАЙЛА
```

При использовании Pyxel в виде пакета сценарий может быть выполнен как обычный код на Python:

```sh
cd pyxel_examples
python3 ИМЯ_PYTHON_ФАЙЛА
```

(Под Windows, набирайте `python` вместо `python3`)

### Особые клавиши

Следующие особые клавиши можно применять во время выполнения Pyxel-приложения:

- `Esc`<br>
Выйти из приложения
- `Alt(Option)+1`<br>
Выполнить снимок экрана и сохранить его на рабочий стол
- `Alt(Option)+2`<br>
Начать захват экрана игры
- `Alt(Option)+3`<br>
Сохранить видео, полученное захватом экрана на рабочий стол (до 10 секунд)
- `Alt(Option)+0`<br>
Включить/выключить мониториг производительности (fps, время на update, время на draw)
- `Alt(Option)+Enter`<br>
Войти/выйти из полноэкранного режима

### Как создать ресурсный файл

Встроенный Pyxel Editor может создавать изображения и звуки, используемые в Pyxel-приложении.

Он запускается следующей командой:

```sh
pyxel edit [имя_ресурсного_файла]
```

Если указанный ресурсный файл (.pyxres) существует, то он будет загружен. В противном случае будет создан файл с указанным именем.
Если имя файла пропущено, то используется стандартное имя `my_resource.pyxres`

После запуска Pyxel Editor, можно переключаться между различными файлами способом drag-and-drop. Если данное действие произвести, зажав клавишу ``Ctrl(Cmd)``, то будет загружен только редактируемый в этот момент тип ресурса (изображения/карта тайлов/звук/музыка). Это позволяет комбинировать несколько ресурсных файлов в один.

Созданный ресурсный файл может быть загружен в программу с помощью функции `load`.

Редактор Pyxel Editor оснащем следующими режимами редактирования.

**Редактор изображений:**

Режим редактирования наборов изображений.

<img src="images/image_editor.gif">

Изображение (png/gif/jpeg) может быть загружено в выбранный набор путем перетаскивания png файла на экран редактора изображений.

**Редактор тайлмапов:**

Режим редактирования тайлмапов, в котором изоражения расположены в плиточном порядке.

<img src="images/tilemap_editor.gif">

**Редактор звука:**

Режим для редактирования звуковых файлов.

<img src="images/sound_editor.gif">

**Редактор музыки:**

Режим для редактирования музыки, в которой звуки расставлены в порядке проигрывания.

<img src="images/music_editor.gif">

### Другие методы создания ресурсов

Изображения и карты тайлов Pyxel могут также быть созданы следующим образом:

- Создайте изображение из списка строк с помощью функций `Image.set` или `Tilemap.set`.
- Загрузите png файла, выполненный в палитре Pyxel, с помощью функции `Image.load`.

Звуки Pyxel могут также быть созданы следующим образом:

- Создайте звук из строк с помощью функций `Sound.set` или `Music.set`.

Обратитесь к руководству по API (ниже) для получения более подробной информации об использовании этих функций.

### Как распространять приложение

Pyxel предлагает формат распространения приложений (файл Pyxel-приложения), работающий на всех поддерживаемых платформах.

Создать файл Pyxel-приложения (.pyxapp) можно с помощью следующей команды:

```sh
pyxel package корневой_каталог_приложения имя_файл_запускающего_скрипта
```

Если приложение должно включать в себя дополнительные ресурсы или модули, поместите их в каталог приложения.

Созданный файл приложения может быть запущен следующей командой:

```sh
pyxel play ФАЙЛ_PYXEL_ПРИЛОЖЕНИЯ
```

## Руководство по API

### Система

- `width`, `height`<br>
Ширина и высота окна

- `frame_count`<br>
Количество отрисованных кадров

- `init(width, height, [title], [fps], [quit_key], [capture_scale], [capture_sec])`<br>
Инициализирует Pyxel-приложение с указанными размерами экрана (`width`, `height`). Дополнительно могут быть заданы: заголовок окна с помощью параметра `title`, количество кадров в секунду с помощью параметра `fps`, клавиша для выхода из приложения — `quit_key`, коэффициент масштабирования при захвате экрана — `capture_scale` и максимальное время записи при захвате экрана с помощью `capture_sec`.<br>
Пример: `pyxel.init(160, 120, title="My Pyxel App", fps=60, quit_key=pyxel.KEY_NONE, capture_scale=3, capture_sec=0)`

- `run(update, draw)`<br>
Запустить Pyxel-приложение, использующее функцию `update` для обновления внутренней логики и `draw` для рисования.

- `show()`<br>
Отрисовать кадр и ждать выхода из приложения по нажатию клавиши `Esc` (не для использования в настоящих приложениях).

- `flip()`<br>
Принудительно отрисовать кадр (не для использования в настоящих приложениях).

- `quit()`<br>
Завершить работу Pyxel-приложения.

### Ресурсы

- `load(filename, [image], [tilemap], [sound], [music])`<br>
Загрузить ресурсный файл (.pyxres). Если False указано для типа ресурса (``image/tilemap/sound/music``), соответствующий ресурс не будет загружен.

### Ввод

- `mouse_x`, `mouse_y`<br>
Получить положение курсора мышки

- `mouse_wheel`<br>
Получить значение колесика мышки

- `btn(клавиша)`<br>
Получить `Ture`, если `клавиша` нажата, в противном случае получить `False`. ([Список определений клавиш](../pyxel/__init__.pyi))

- `btnp(клавиша, [hold], [period])`<br>
Получить `True`, если `клавиша` нажата в данный кадр, в противном случае получить `False`. В случае, если указаны параметры `hold` и `period`, `True` будет возвращено каждые `period` кадров, когда `key` уже зажата более `hold` кадров

- `btnr(клавиша)`<br>
Получить `True`, если `клавиша` была отпущена в данный кадр, в противном случае получить `False`

- `mouse(видна)`<br>
Установить видимость курсора: если `visible` равно `True`, сделать виндым, если `False`, то невидимым. Даже если курсор не отображается, его позицию всё равно можно получить соответствующими функциями.

### Графика

- `colors`<br>
Список цветов палитры. Цвет кодируется 24-битным целым числом. Используйте `colors.from_list` и `colors.to_list` для установки и получения списка Python.<br>
Пример: `org_colors = pyxel.colors.to_list(); pyxel.colors[15] = 0x112233; pyxel.colors.from_list(org_colors)`

- `image(img, [system])`<br>
Оперировать набором изображений `img` (0-2) (смотрите класс Image).<br>
Пример: `pyxel.image(0).load(0, 0, "title.png")`

- `tilemap(tm)`<br>
Оперировать тайлмапом `tm`(0-7) (смотрите класс Tilemap)

- `clip(x, y, w, h)`<br>
Установить площадь рисования экрана с (`x`, `y`) до ширины `w` и высоты `h`. Сбросить площадь рисования до полного экрана можно с помощью `clip()`

- `camera(x, y)`<br>
Изменить координаты левого верхнего угла экрана на (`x`, `y`). Координаты левого верхнего угла экрана могут быть сброшены в (`0`, `0`) вызовом `camera()`.

- `pal(col1, col2)`<br>
Поменять цвет `col1` с цветом `col2` во время рисования. Восстановить изначальную палитру можно с помощью `pal()`

- `cls(col)`<br>
Заполнить (очистить) экран цветом `col`

- `pget(x, y)`<br>
Получить цвет пикселя по координатам (`x`, `y`)

- `pset(x, y, col)`<br>
Нарисовать пиксель цвета `col` по координатам (`x`, `y`)

- `line(x1, y1, x2, y2, col)`<br>
Нарисовать отрезок цвета `col` из (`x1`, `y1`) в (`x2`, `y2`)

- `rect(x, y, w, h, col)`<br>
Нарисовать прямоугольник ширины, высоты `w` и цвета `h` по координатам (`x`, `y`)

- `rectb(x, y, w, h, col)`<br>
Нарисовать контур прямоугольника ширины, высоты `w` и цвета `h` по координатам (`x`, `y`)

- `circ(x, y, r, col)`<br>
Нарисовать круг радиуса `r` и цвета `col` центром в (`x`, `y`)

- `circb(x, y, r, col)`<br>
Нарисовать окружность радиуса `r` и цвета `col` центром в (`x`, `y`)

- `tri(x1, y1, x2, y2, x3, y3, col)`<br>
Нарисовать треугольник с вершинами в координатах (`x1`, `y1`), (`x2`, `y2`), (`x3`, `y3`) и цвета `col`

- `trib(x1, y1, x2, y2, x3, y3, col)`<br>
Нарисовать контур треугольника с вершинами в координатах (`x1`, `y1`), (`x2`, `y2`), (`x3`, `y3`) и цвета `col`

- `blt(x, y, img, u, v, w, h, [colkey])`<br>
Скопировать область размеров (`w`, `h`), по координатам (`u`, `v`) набора изображений `img`(0-2) по координатам (`x`, `y`) на экране. Если для `w` и/или `h` установлено отрицательное значение, изображение будет развернуто горизонтально и/или вертикально. Если указан параметр `colkey`, соответствующий цвет будет считаться цветом фона (прозрачным цветом)

<img src="images/blt_figure.png">

- `bltm(x, y, tm, u, v, w, h, [colkey])`<br>
Нарисовать из тайлмапа `tm` (0-7) по координатам (`x`, `y`) тайл размером (`w`, `h`), находящийся по координатам (`u`, `v`). Если переданы отрицательные значения `w` и/или `h`, то изображение будет отражено по горизонтали и/или вертикали. Если указан параметр `colkey`, соответствующий цвет будет считаться цветом фона (прозрачным цветом). Размер тайла равен 8x8 точек и хранится в карте тайлов в виде кортежа `(x в банке изображений, y в банке изображений)`.

<img src="images/bltm_figure.png">

- `text(x, y, s, col)`<br>
Нарисовать строку текста `s` цвета `col` по координате (`x`, `y`)

### Аудио

- `sound(snd)`<br>
Оперировать звуком `snd`(0-63).<br>
Пример: `pyxel.sound(0).speed = 60`

- `music(msc)`<br>
Оперировать музыкой `msc`(0-7) (смотрите класс Music)

- `play_pos(ch)`<br>
Получить позицию канала `ch` (0-3) в виде кортежа `(номер звука, номер ноты)`. Возвращает `None` если проигрывание выключено.

- `play(ch, snd, loop=False)`<br>
Проиграть звук `snd` (0-63) на канале `ch` (0-3). Если `snd` — список, он будет проигран по порядку. Если в в качестве значения `loop` передано `True`, проигрывание будет зациклено.

- `playm(msc, loop=False)`<br>
Проиграть трек `msc` (0-7). Если в в качестве значения `loop` передано `True`, проигрывание будет зациклено.

- `stop([ch])`<br>
Остановить воспроизведение на канале `ch` (0-3). `stop()` останавливает воспроизведение на всех каналах.

### Класс Image

- `width`, `height`<br>
Ширина и высота изображения

- `data`<br>
Данные изображения (матрица 256x256)

- `get(x, y)`<br>
Получить данные изображения в точке (`x`, `y`)

- `set(x, y, data)`<br>
Установить данные изображения в точке (`x`, `y`) списком строк.<br>
Пример: `pyxel.image(0).set(10, 10, ["0123", "4567", "89ab", "cdef"])`

- `load(x, y, filename)`<br>
Загрузить файл изображения (png/gif/jpeg) в координаты (`x`, `y`).

### Класс Tilemap

- `width`, `height`<br>
Ширина и высота тайлмапа

- `refimg`<br>
Банк изображений (0-2), на который ссылается карта тайлов

- `set(x, y, data)`<br>
Установить данные карты тайлов в точке (`x`, `y`) списком строк.<br>
Пример: `pyxel.tilemap(0).set(0, 0, ["000102", "202122", "a0a1a2", "b0b1b2"])`

- `pget(x, y)`<br>
Получить тайл в координатах (`x`, `y`). Возвращаемое значение представляет собой кортеж `(x в банке изображений, y в банке изображений)`.

- `pset(x, y, tile)`<br>
Задать тайл в координатах (`x`, `y`). Тайл передаётся в виде кортежа `(x в банке изображений, y в банке изображений)`.

### Класс Sound

- `notes`<br>
Список нот (0-127). Чем больше значение, тем выше нота. Значение 33 соответствует ноте «ля» второй октавы 'A2' (440Hz). Пауза задаётся значением -1.

- `tones`<br>
Список тонов (0:Треугольник / 1:Квадрат / 2:Пульс / 3:Шум)

- `volumes`<br>
Список громкости(0-7)

- `effects`<br>
Список эффектов (0:Нет / 1:Слайд / 2:Вибрато / 3:Затихание)

- `speed`<br>
Длительность воспроизведения. 1 — самая быстрая, чем выше значение, тем ниже скорость воспроизведения. При значении, равном 120 длительность воспроизведения одной ноты составляет 1 секунду.

- `set(notes, tones, volumes, effects, speed)`<br>
Установить ноты, тоны, громкость и эффекты с помощью строк. Если длины строк для тона, громкости и эффектов короче строки для нот, они зацикливаются.

- `set_notes(notes)`<br>
Установить ноты с помощью строки, составленной по форме 'CDEFGAB'+'#-'+'0123' или 'R'. Регистр и пробелы игнорируются.<br>
Пример: `pyxel.sound(0).set_note("G2B-2D3R RF3F3F3")`

- `set_tones(tones)`<br>
Установить тоны строкой, составленной из 'TSPN'. Регистр и пробелы игнорируются.<br>
Пример: `pyxel.sound(0).set_tone("TTSS PPPN")`

- `set_volumes(volumes)`<br>
Установить громкость с помощью строки, составленной из '01234567'. Регистр и пробелы игнорируются.<br>
Пример: `pyxel.sound(0).set_volume("7777 7531")`

- `set_effects(effects)`<br>
Установить эффекты с помощью строки, составленной из 'NSVF'. Регистр и пробелы игнорируются.<br>
Пример: `pyxel.sound(0).set_effect("NFNF NVVS")`

### Класс Music

- `sequences`<br>
Двумерный список описаний звуков (0-63) по каналам

- `set(seq0, seq1, seq2, seq3)`<br>
Установить список звуков (0-63) для всех каналов. Пустой список означает, что канал не используется для проигрывания.<br>
Пример: `pyxel.music(0).set([0, 1], [2, 3], [4], [])`

### Расширенный APIs

Pyxel имеет «расширенные API», не упомянутые в этом документе, так как они «могут смутить пользователя» или «требуют специальных знаний для использования».

Если вы уверены в своих силах, используйте [это](../pyxel/__init__.pyi) в качестве подсказки!

## Как сделать вклад в развитие проекта?

### Сообщение о проблемах

Используйте [трекер проблем](https://github.com/kitao/pyxel/issues) для отправки отчётов о проблемах или предложений по улучшению/добавлению новых возможностей. Перед созданием новой задачи, убедитесь что схожие открытые задачи отсутствуют.

### Ручное тестирование

Ручное тестирование кода и написание отчетов о проблемах, предложений по улучшению в [трекере проблем](https://github.com/kitao/pyxel/issues) приветствуется!

### Опубликование запроса на слияние

Патчи/фиксы принимаются в форме запросов на слияние (pull-запрос, PR). Убедитесь, что проблема, к которой относится запрос на слияние изменений, открыта в трекере проблем.

Опубликованный pull-запрос считается опубликованным под лицензией [MIT License](../LICENSE).

## Прочая информация

- [Сервер Discord (Англоязычный)](https://discord.gg/FC7kUZJ)
- [Сервер Discord (Японский - 日本語版)](https://discord.gg/qHA5BCS)

## Лицензия

Pyxel разпространяется по лицензией [MIT License](../LICENSE). Он может быть использован в проприетарном программном обеспечении при условии того, что все копии этого программного обеспечения или значительные его части содержат копию MIT License terms and the copyright notice.
