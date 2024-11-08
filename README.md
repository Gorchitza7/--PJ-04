
# Проект "СКАН" (Фин экзамен) (HW) - Поиск публикаций о компаниях

## Описание
Кейс от компании «СКАН». Клиентская часть сервиса для поиска публикаций о компаниях (юридических лицах) в СМИ по ИНН. Серверная часть уже разработана компанией "СКАН".

## Функциональные требования
- Главная страница
- Форма авторизации
- Форма для ввода параметров поиска (ИНН компании, количество документов)
- Страница с результатами поиска (список публикаций)

## Дополнительные требования
- Безопасная авторизация с сохранением токена в локальном хранилище
- Разделение доступа для авторизованных и неавторизованных пользователей
- Обязательные поля в формах, валидация, невозможность отправки незаполненной формы
- Ленивая подгрузка данных (lazy loading) для оптимизации UX
- Использование Redux или React Context для управления состоянием

## Установка
1. Клонировать репозиторий
2. Перейти в директорию проекта
3. Установить зависимости: `npm install`
4. Запустить проект: `npm start`

## Сборка
`npm run build` - создает оптимизированную сборку в директории build/

## Ограничения
- Макс. кол-во документов в выборке 1000, но API работает только до 45
- Нет фото и имени пользователя (используются заглушки)
- Не обновляются данные об использованных компаниях
- Нет обложек для статей (используется заглушка)

Ссылка на макет Figma: https://www.figma.com/file/u3MOjzYnTnirz712GrLbFv/
- Все советы укаазанные в макете учтены при работе над проектом!

## Страница результатов поиска
Результаты поиска отображаются в виде карточек со следующими элементами:
- Дата публикации и название источника (ссылка на оригинал)
- Заголовок публикации
- Теги в зависимости от свойств объекта (технические новости, анонсы, сводки новостей)
- Содержимое публикации с картинками (если есть)
- Кнопка "Читать в источнике" (открывает оригинал в новой вкладке)
- Количество слов в публикации

Реализовать ленивую подгрузку (lazy loading) результатов:
- Изначально загружать только первые 10 результатов
- Добавить кнопку "Показать больше" для подгрузки следующих 10 результатов
- После загрузки всех результатов скрыть кнопку.

На время загрузки результатов показывать лоадер
Если результатов не найдено - отобразить соответствующее сообщение.

## Общие требования
1. Соответствие вёрстки макету (цвета, шрифты, размеры, отступы)
2. Корректное отображение на мобильных устройствах 
3. Семантическая вёрстка (header, main, footer, h1 и т.д.)
4. Визуальные эффекты на ссылках и кнопках при наведении 
5. Грамотное подключение стилей (CSS, CSS-модули, Styled Components и т.п.)
6. Использовать классы, а не ID и теги для стилизации 
7. SVG изображения из Figma для качественного отображения

## Требования к коду
1. Реализация на React 
2. Разумное разделение на компоненты 
3. Использование продвинутых инструментов управления состоянием (useReducer, Context, Redux)
4. Следование принципам KISS и DRY 
5. Разумное использование сторонних библиотек 
6. Аккуратное форматирование и осмысленные названия 
7. Использование современного JS/React синтаксиса 
8. Игнорирование node_modules в .gitignore

## Работу выполнил Маслов Андрей
