# Продолжаем проект по Django REST framework (DRF) добавляем Docker Compose

    Django REST framework (DRF) — это библиотека, которая работает со стандартными моделями Django для создания гибкого и
    мощного API для проекта.

    Docker Compose — это инструмент для определения и запуска многоконтейнерных приложений. Он позволяет определить все
    компоненты вашего приложения, их настройки и взаимодействия в одном файле конфигурации, а затем легко запустить их все
    одной командой.

# ТРЕКЕР ПОЛЕЗНЫХ ПРИВЫЧЕК
________________________________________________________________________________________________________________________

## ОПИСАНИЕ
Проект представляет собой бэкенд-часть SPA (Single Page Application) веб-приложения. Это мощный инструмент, который
поможет пользователям приобретать новые полезные привычки и избавляться от старых плохих. Проект разработан с учетом
концепций, представленных в книге "Атомные привычки" Джеймса Клира и предоставляет удобные инструменты для
самосовершенствования и улучшения качества жизни.
________________________________________________________________________________________________________________________

## ОСОБЕННОСТИ ПРОЕКТА
1. Тщательно разработанная модель привычки: Центральный элемент в проекте "Трекер полезных привычек". Она представляет
   собой описание конкретной привычки пользователя, включая информацию о времени, месте и действии, связанным с этой
   привычкой. Модель также учитывает ее характеристики, такие как приятность, вознаграждение и связанные привычки. Это
   позволяет пользователям эффективно отслеживать и улучшать свои привычки, создавать целенаправленные напоминания и
   получать мотивацию для выполнения заданных действий.
2. Интеграция с Telegram: Приложение интегрировано с Telegram, что позволяет отправлять уведомления и напоминания
   пользователям через собственного бота. Это полезное средство для обеспечения постоянной мотивации и контроля за
   полезными привычками.
3. CORS: В проекте имеется настройка CORS, что позволяет клиентской части приложения безопасно общаться с бэкенд-частью.
   Это гарантирует, что веб-приложение может работать в разных браузерах и с разных доменов, обеспечивая гибкость в
   использовании.
4. Отложенные задачи с помощью Celery: Используется Celery для выполнения отложенных задач и фоновой обработки данных.
   Это
   обеспечивает эффективное управление задачами и оптимизацию производительности приложения.

________________________________________________________________________________________________________________________

## Требование к настройке и запуску
1. Создание файла .env: Создайте файл с именем .env в корневой директории вашего проекта. В файле .env заполните

        SECRET_KEY=
        DEBUG=
        POSTGRES_DB=
        POSTGRES_USER=
        POSTGRES_PASSWORD=
        POSTGRES_HOST=
        POSTGRES_PORT=
        CELERY_BROKER_URL=
        CELERY_RESULT_BACKEND=
        EMAIL_BACKEND=
        EMAIL_HOST=
        EMAIL_PORT=
        EMAIL_USE_TLS=
        EMAIL_USE_SSL=
        EMAIL_HOST_USER=
        EMAIL_HOST_PASSWORD=
        API_TELEGRAM_TOKEN=
        TELEGRAM_ID=

2. Сборка контейнеров: Теперь выполните следующую команду для сборки контейнеров:

       docker-compose build

________________________________________________________________________________________________________________________

## ЗАПУСК ПРОЕКТА
1. Запуск проекта: Для запуска проекта, после успешной сборки контейнеров, введите следующую комманду:

        docker-compose up

2. Использование проекта: Откройте веб-браузер и перейдите по адресу, указанному в консоли (
   обычно http://127.0.0.1:8000/).
   Проведите тестирование различных функциональностей вашего проекта, чтобы удостовериться, что они работают как
   ожидалось.

________________________________________________________________________________________________________________________

## ТЕХНОЛОГИИ
1. Python 3.10: Проект основан на языке программирования Python, что обеспечивает чистоту и читаемость кода, а также
   широкие
   возможности для расширения.
2. Django: В качестве фреймворка для разработки веб-приложения используется Django, что обеспечивает структурированный и
   масштабируемый подход к веб-разработке.
3. Django Rest Framework (DRF): DRF применяется для построения API проекта, обеспечивая простоту и гибкость
   взаимодействия
   с данными.
4. Telegram API: Интеграция с Telegram обеспечивает надежное и мгновенное взаимодействие с пользователями, делая
   приложение
   отличным выбором для напоминания о привычках.
5. Celery: Для выполнения асинхронных задач и улучшения производительности проекта активируется Celery Worker. Это
   позволяет обрабатывать фоновые задачи, такие как отправка уведомлений и обработка длительных операций.
6. Swagger(OpenAPI): Документация API предоставляется с использованием интерфейса Swagger, что упрощает понимание и
   использование API для разработчиков.
7. Docker: Для упрощения развертывания и управления приложением в среде контейнеров используется Docker. Docker
   обеспечивает изоляцию и переносимость приложения, что делает процесс развертывания более удобным и надежным.
________________________________________________________________________________________________________________________

## СВЯЗЬ
Если у вас возникли вопросы, предложения или потребность в поддержке, не стесняйтесь связаться со мной. Я готов помочь
Вам с вашим проектом и ответить на все Ваши вопросы. Вы можете связаться со мной по следующим контактам:

Электронная почта: gubingm@list.ru
Telegram: @CompasSpace