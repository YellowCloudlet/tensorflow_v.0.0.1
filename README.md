Как использовать:
1. Архив recognizer(сет с изображениями и готовой к работе нейронкой) тут **<https://mega.nz/#!oXZyyQYa!vCkfxXlNFZvXRaMXiityHtcab88gS_Iy2ph3MgRWS08>** Что бы воспользоваться ею нужен Docker и Tensorflow.(И Python, но для работы с Tensorflow лучше использовать Anaconda) .
2. Открыть консоль, и запустить контейнер командой **docker run -it -v ~/recognizer/:/recognizer/ gcr.io/tensorflow/tensorflow:latest-devel** (Используя Windows или Linux нужно сначала перейти в папку куда был разархивирован архив ***recognizer.zip*** . В моем случае это была корневая папка, то есть /home/cooper/ или же просто **~**)
3. После вывода в консоли следующего **root@95ee4b451ef5:~#** пишем **cd /recognizer** .
4. Получив в консоли следующее **root@95ee4b451ef5:/recognizer#** мы можем приступать к работе и тестировать наши изображения.
5. Далее используем сам скрипт: пишем **python label_image.py handFolder/Bad/7333127.jpg** . 
6. Должно выдать содержание типа
   `bad (score = 0.99934)
    lefthand (score = 0.00042)
    righthand (score = 0.00024)`
    (Выше представлен пример использования скрипта на картинках правой/левой руки а так же их общего изображения)
