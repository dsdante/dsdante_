Kaggle: [dsdante](https://www.kaggle.com/dsdante)  
Docker: [dsdante/skab-pytorch](https://hub.docker.com/repository/docker/dsdante/skab-pytorch/general)

Запуск на CPU: `docker run -p 8000:8000 dsdante/skab-pytorch`  
Запуск с CUDA: `sudo docker run -p 8000:8000 --gpus all dsdante/skab-pytorch`

В дополнение к методу `POST /predict`, принимающему CSV в виде массива строк, также реализован метод `POST /predict/file`, принимающий файлы `*.csv` и бинарные файлы pickle, содержащие `pandas.DataFrame` или `Iterable[pandas.DataFrame]`.
