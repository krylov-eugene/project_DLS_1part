# Общая информация
**В данном проекте я произвожу генерацию обуви из её очертаний**

Полный код проекта расположен в файле [handbagGAN.ipynb](https://github.com/kudaxech/project_DLS_1part/blob/main/handbagGAN.ipynb)\
Код для самостоятельной генерации расположен в [selfGen.ipynb](https://github.com/kudaxech/project_DLS_1part/blob/main/selfGen.ipynb)\
Ссылки на веса модели расположены в папке [weights_links](https://github.com/kudaxech/project_DLS_1part/blob/main/weights_links)

----------
В данной работе используется архитектура cGAN-a pix2pix. Вот оригинальная [статья](https://doi.org/10.48550/arXiv.1611.07004) по ней.\
Датасет взят [отсюда](http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/)

----------
Все ячейки, которые откуда-то заимствовались, сопровождаются ссылками на источники. Заимствовались: загрузка датасета с помощью tensorflow; код, позволяющий рисовать и сохранять изображения в googlecolab; код конвертации RGBA в RGB. Весь остальной код написан самостоятельно.

----------
Код тренировки модели приведен в файле [handbagGAN.ipynb](https://github.com/kudaxech/project_DLS_1part/blob/main/handbagGAN.ipynb), в разделе "Создание модели и обучение". 

# Генерация изображений
Сгенерировать изображения самостоятельно можно, используя скрипт [selfGen.ipynb](https://github.com/kudaxech/project_DLS_1part/blob/main/selfGen.ipynb).
Для этого необходимо переопределить переменную *GEN_PATH*, которая является путем до весов генератора. Затмем остается просто запустить весь код в этом ноутбуке и вызвать функцию *draw_and_show_result()*. После этого нарисовать в появившейся черной рамке то, из чего вы бы хотели получить ботинок, нажать кнопку *finish*, немного подождать (~4 сек. на cpu) и после этого ниже выведется результат работы модели.
