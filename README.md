# tensorflow_v.0.0.1
Simple tensorflow project with Python, Docker and Tensorflow

Как использовать:
1. Открыть консоль, и запустить контейнер командой docker run -it -v ~/recognizer/:/recognizer/ gcr.io/tensorflow/tensorflow:latest-devel (Используя Windows или Linux нужно сначала перейти в папку куда был разархивирован архив recognizer.zip. В моем случае это была корневая папка, то есть /home/cooper/ или же просто ~)
2. После вывода в консоли следующего root@95ee4b451ef5:~# пишем cd /recognizer.
3. Получив в консоли следующее root@95ee4b451ef5:/recognizer# мы можем приступать к работе и тестировать наши изображения.
4. Далее используем сам скрипт: пишем python label_image.py handFolder/Bad/7333127.jpg. Должно выдать содержание типа
    bad (score = 0.99934)
    lefthand (score = 0.00042)
    righthand (score = 0.00024)
    (Выше представлен пример использования скрипта в работе с картинками левой/правой руки а так же их общим изображением)
