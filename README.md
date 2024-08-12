# QSO Logger
QSO Logger — это прототип аппаратного журнала способного передавать данные на QSO.SU и выступать в роле агента для взаимодействия с ПО для цифровых видов связи.

## Установка для Ubuntu:

1) Установите зависимости:

```console
apt install git qtbase5-dev qt5-qmake qtbase5-dev-tools libsqlite3-dev build-essential
```

2) Склонируйте репозиторий:

```console
git clone https://github.com/qsosu/logger.git
```

3) Перейдите в папку с репозиторием, создайте папку build, зайдите в неё и подготовьтесь компилировать:

```console
cd logger/ && mkdir build/ && cd build/ && qmake ../QSOSU-desktop-app.pro
```

4) Запустите компилятор (Дле `<кол-во ядер CPU>` укажите количество ядер.):

```console
make -j <кол-во ядер CPU>
```

5) После выполнения всех действий, запустите QSO Logger:

```console
./QSOSU-desktop-app
```
