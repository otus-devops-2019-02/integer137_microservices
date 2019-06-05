# integer137_microservices
integer137 microservices repository

##"ДЗ Docker-4"

"Запустили контейнер с использованием none-драйвера."

"Сравнили вывод команд ````docker run -ti --rm --network host joffotron/docker-net-tools -c ifconfig```` и ````docker-machine ssh docker-host ifconfig````."

"Запустили несколько раз ````docker run --network host -d nginx````."

"Просмотрели существующие в данный момент net-namespaces."

"Создаем bridge-сеть в docker."

"Запускаем проект внутри bridge-сети."

"Запускаем проект внутри 2-х bridge-сетях."

"Проводим установку docker-compose."

"Создаем файл docker-compose.yml."

"Запускаем проект, используя docker-compose."

"Изменяем docker-compose под кейс с множеством сетей. Параметризируем docker-compose.yml."

"Базовое имя проекта docker-compose можно задать. Задается с помощью параметра --project-name. По умолчанию задается по имени директории."

##"ДЗ Docker-3"

"Создали новую ветку в репозитории с названием docker-3."

"Установили линтер hadolint."

"Подключились к Docker-хосту в GCP."

"Распаковали архив reddit-microservices в репозитории. Переименовали каталог в src."

"Создали Dockerfile внутри сервисов post-py, comment, ui."

"Скачали пследний образ MongoDB командой ````docker pull mongo:latest````."

"Собрали образы с сервисами post-py, comment, ui. В процессе сборки вносим правки в Dockerfile сервисов."

"Создадали специальную сеть reddit для приложения."

"Произвели запуск контейнеров."

"Осуществили проверку работоспособности."

"Улучшили сервис ui."

"Перезапустили приложение. Пост не сохранился. Создали Docker volume."

"Подключили volume к контейнеру с MongoDB."

"Перезапустили приложение. Пост сохранился."


##"ДЗ Docker-2"

"Создали новый проект в GCP и разрешили доступ приложению."

"Провели установку Docker machine."

"Создали Docker-хост в GCP."

"Сравнили вывод команд docker run."

"Создали образ с приложением. Создали файлы Dockerfile, mongod.conf, db_config, start.sh."

"Наполнили файл Dockerfile командами."

"Создали образ командой ````docker build -t reddit:latest .````."

"Запустили Docker контейнер."

"Зареристрировались на Docker hub."

"Загрузили образ на Docker hub."

"Запустили Docker образ локально."

"Осуществили всевозможные проверки."

##"ДЗ Docker-1"

"Провели установку Docker."

"Осуществили проверку версии Docker командами:"

````docker version````

````docker info````

"Запустили первый контейнер Docker командой ````docker run hello-world````."

"Создали и запустили новый контейнер из image ````docker run -it ubuntu:16.04 /bin/bash````."

"Осознали разницу между командами docker run и docker start."

"Создали image docker-контейнера командой ````docker commit d120403fe10e yourname/ubuntu-tmp-file````."

"Сохранили вывод команды docker images в файл docker-1.log."
