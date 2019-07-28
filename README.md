# integer137_microservices
integer137 microservices repository

##"ДЗ Kubernetes-4"

"Провели установку helm. Установили tiller."

"Установили и шаблонизировали Chart."

"Установили несколько релизов ui-компоненты приложения."

"Кастомизировали установку своими переменными."

"Проделали аналогичную операцию с остальными компонентами приложения."

"Дополнительно создали в директорях templates файлы _helpers.tpl, в которых описали функцию {{ .Release.Name }}-{{ .Chart.Name }} для каждой компоненты приложения."

"Создали Chart'ы для каждой компоненты приложения."

"Создали Chart в папке /reddit и настроили зависимости к компонентам приложения."

"Обновили зависимости Chart'а reddit. Обновили релиз, установленный в папке reddit."

"Начали установку Gitlab."

"Подготовили GKE-кластер для Gitlab."

"Добавили репозиторий Gitlab."

"Скачали Chart gitlab-omnibus."

"Внесли изменения в файлы values.yaml и gitlab-svc.yaml."

"Внесли изменения в файлы gitlab-config.yaml и gitlab-ingress.yaml."

"Установили Gitlab командой ````helm install --name gitlab . -f values.yaml````."

"Добавили запись в файл /etc/hosts."

"Залогинились в Gitlab. Создали группу, переменные, проекты."

"Создали pipeline для каждой компоненты приложения."

"Создали staging и production среды для работы приложения, задеплоили."

##"ДЗ Kubernetes-3"

"Разобрали типы сервисов kubernetes."

"Разобрали плагин kube-dns."

"Разобрали тип сервиса LoadBalancer, перенастроили ui-сервис."

"Включили встроенный ingress на кластере GKE."

"Перенастроили ingress."

"Защитили сервис с помощью TLS."

"Разобрали и добавили Network Policy в GKE."

"Добавили хранилище для базы данных."

"Использовали типы хранилища Volume и PersistentVolume."

"Использовали динамическое выделение Volume-ов."

##"ДЗ Kubernetes-2"

"Провели установку kubectl."

"Провели установку Minicube."

"Осуществили запуск Minicube-кластера."

"Запустили в Minikube компоненты приложения."

"Осуществили проверку."

"Создали сервисы для компонентов приложения. Осуществили проверку."

"Создали окружение dev. Запустили в нем сервисы. Осуществили проверку."

"Развернули Kubernetes Engine в GCP."

"Создадали dev namespace в GKE."

"Задеплоили все компоненты приложения в namespace dev в GKE."

"Ссылка на приложение http://34.90.50.214:32091"

##"ДЗ Kubernetes-1"

"Создали файлы с Deployment манифестами в директории kubernetes/reddit."

"Kubernetes The Hard Way."

"Инициализировали gcloud. Установили tmux."

"Установили cfssl, cfssljson и kubectl."

"Проделали провиженинг сети."

"Создали 3 контроллера и 3 воркера для kubernetes."

"Создали сертификаты."

"Создаем конфигурационные файлы kubernetes."

"Настроили ключи."

"Произвели запуск контроллеров kubernetes."

"Произвели запуск воркеров kubernetes."

"Настроили удаленный доступ."

"Настроили сетевые маршруты для подов."

"Развернули DNS-addon."

"Провели пробный запуск подов из папки reddit."

##"ДЗ Logging-1"

"Произвели подготовку. Выполнили пересборку образов."

"Создадали Docker хост в GCE."

"Создали отдельный compose-файл для системы логирования."

"Собрали docker image для fluentd."

"Запустили сервисы. Посмотрели логи приложения командой ````docker-compose logs -f post````."

"Собрали образы elasticsearch и kibana."

"Провели настройку kibana."

"Просмотрели лог-сообщения через kibana."

"Пересоздали образ fluentd для фильтрации json-логов."

"Выполнили поиск в kibana по событию создания нового поста."

"Настроили логирование UI сервиса."

"Произвели парсинг логов, используя grok-шаблон."

"Добавили в compose-файл для сервисов логирования сервис распределенного трейсинга Zipkin."

"Изучили Zipkin WEB UI."

##"ДЗ Monitoring-2"

"Произвели подготовку окружения в GCP."

"Разделили файлы Docker-compose (сервисы и мониторинг)."

"Добавили cadvisor в конфигурацию Prometheus."

"Пересобираем образ Prometheus. Запускаем сервисы. Открыли страницу cAdvisor UI ````http://34.76.73.88:8080/docker/````."

"Использовали инструмент Grafana для визуализации данных из Prometheus."

"Добавили новый источник данных grafana. Скачали с сайта grafana дашборд."

"Произвели импорт дашборда."

"Добавили в конфигурацию Prometheus информацию о post-сервисе."

"Создали и сохранили новый дашборд UI_Service_Monitoring. Создали графики."

"Добавили график 95 процентиля времени ответа на запрос."

"Добавили дашборд метрик бизнес логики."

"Добавили Alertmanager для системы мониторинга Prometheus. Пересобрали образ Prometheus."

"Проверили интеграцию Alertmanager-Slack."

"Запушили собранные образы на DockerHub."

##"ДЗ Monitoring-1"

"Создали правило фаервола для Prometheus и Puma."

"Создали Docker хост в GCE."

"Запустили систему мониторинга Prometheus."

"Выбрали метрику prometheus_build_info."

"Просмотрели информацию о метриках Prometheus http://34.76.73.88:9090/metrics."

"Переупорядочили структуру директорий."

"Создаем Docker образ. Определяем конфигурацию Prometheus в файле prometheus.yml."

"Проводим сборку образов при помощи скриптов docker_build.sh."

"Подняли сервисы, определенные в docker/docker-compose.yml."

"Посмотрели список endpoint-ов."

"Остановили post сервис. Наблюдаем за графиком. Восстанавливаем работу приложения."

"Определили Node exporter сервис в docker/docker-compose.yml файле."

"Добавили новый Job в prometheus.yml. Пересоздали Docker-образ Prometheus."

"Пересоздали сервисы командой ````docker-compose up -d````."

"Получим информацию об использовании CPU с помощью метрики node_load1."

"Запушили собранные образы на DockerHub."

"Ссылка на Докерхаб ````https://hub.docker.com/u/integer137````."

##"ДЗ Gitlab-ci-1"

"Создали новую виртуальную машину с заданными параметрами в GCP."

"Устанавили Docker на виртуальную машину."

"Подготовили окружение. Внесли правки в docker-compose.yml."

"Проверили доступ к Gitlab по http://35.198.81.51. Указали пароль для root, вошли в систему."

"Создали группу homework. Создали проект example."

"Добавили remote в integer137_microservices. Добавили в репозиторий файл .gitlab-ci.yml."

"Подготовили пайплайн. Запустили раннер. Зарегистрировали его в интерактивном режиме."

"Проверили статус раннера."

"Добавляем тестирование приложения reddit в pipeline. Внесли правки в .gitlab-ci.yml."

"Создали файл simpletest.rb в папке reddit."

"Добавили библиотеку для тестирования в reddit/Gemfile приложения."

"Провели описание DEV-окружения."

"Создаем stage и prod окружения."

"Добавили директиву only. Проверяем с тэгом."

"Добавляем job, который определяет динамическое окружение для каждой ветки в репозитории."

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
