# DS // Тестовое задание для стажировки

Необходимо реализовать веб-приложение momentum, аналог [расширения](https://chromewebstore.google.com/detail/momentum/laookkfknpbbblfpciffpaejjkokdgca?hl=ru&pli=1).
В приложении есть часы, дата, слайдер изображений, виджеты погоды, список задач.

## Блок погоды
- Состоит из города
- Отображения температуры
- Отображения текущей погоды (дождь/солнечная/снег/пасмурно)

**Функционал:**
- Для определения текущего города использовать geolocation api, город по умолчанию Краснодар
- Для хранения населённого пункта используется локальное хранилище - local storage.
- Для получения погоды использовать [список api](https://github.com/public-api-lists/public-api-lists?tab=readme-ov-file#weather)
  
## Блок слайдер изображений на фоне
- Динамичная смена обоев в зависимости от текущего времени
  
**Функционал:**
- Для динамической смены обоев дано 4 картинки и каждая картинка соответствует определенному промежутку времени, например если сейчас 15:00, то показываем картинку из промежутка 12:00 - 18:00
- Каждому промежутку соответсвтует свое изображение:
`00:00 - 06:00` - `https://github.com/digitalSector47/traineeship-test-task/images/01.jpg`
`06:00 - 12:00` - `https://github.com/digitalSector47/traineeship-test-task/images/02.jpg`
`12:00 - 18:00` - `https://github.com/digitalSector47/traineeship-test-task/images/03.jpg`
`18:00 - 00:00` - `https://github.com/digitalSector47/traineeship-test-task/images/04.jpg`

## Блок времени и даты
- Отображение времени в формате `hh:mm:ss`
- Отображение даты в формате текущий день и текущий день недели, пример: `09 сентября, понедельник`
  
**Функционал:**
- Время изменяется каждую секунду
- Для работы приложения используем текущий часовой пояс

## Блок задач
- Поле для ввода новой задачи
- Чекбокс показать только выполненные задачи
- Список всех задач (состоит из чекбокса, названия задачи и кнопки удалить задачу)
- Кнопка удалить выполненные задачи
  
**Функционал:**
- Добавление новых задач осуществляется при нажатии на "Enter"
- Если поля для ввода новой задачи пустое - появляется ошибка
- Функционал фильтрации задач по выполненным
- Функционал удаления задачи из списка, у каждой задачи, должа быть кнопка удалить
- Функционал перевода задачи в статус выполнено, осуществляется при нажатии на чекбокс в списке задач
- Функционал удаления выполненных задач

