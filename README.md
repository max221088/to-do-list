# to-do-list
Требования:

1. Используйте Vue.js для создания компонентов и управления состоянием приложения.
2. Интерфейс должен содержать следующие элементы:
  - Поле ввода для добавления новой задачи.
  - Кнопка "Добавить", чтобы добавить новую задачу в список.
  - Список добавленных задач с возможностью отметить         выполненные или удалить задачу.
  - Опционально: добавьте кнопку "Редактировать", чтобы пользователи могли изменить текст задачи после добавления.
3. Задачи должны сохраняться в состоянии приложения и не должны исчезать после перезагрузки страницы.
4. Верстка и дизайн могут быть простыми, но должны быть читабельными и эстетичными.


Выполнено:

1. Приложение написано с использованием фреймворка Vue.js 3. Используеться Vuex для управления состоянием,
  также для сохранение пользовательских данных используеться LocalStorage.
2. Интерфейс разделен на два условных блока:
    - болк меню содержит:
        1. Кнопку добавление заданий процесс добавления задания вынесен в модальное окно для удобства     использования
        2. Поле писка заметки по ее содержанию (процесс поиска происходит во времмя ввода запроса)
        3. Выпадающий список сортировки по дате добавления заметки от более раннией до более поздней
        4. Выпадающий список фильтра заметок по криерию отметки о выполнеии.
    - рабочая область с заданиями содержит :
        1. Плитки с заданиями в которых отображаеться индикатор о выполенеии, текст задания, дата добавления, дата выполнения или статус "в работе", кнопки управления заданием такие как редактирование и удаление заметки, так же отредактиовать задание можно по двойному клику на содержание задания.
        2. Чтобы отметить задачу как "выполнена" достаточно нажать на пиктограмку ввиде "галочки" также после этого появиться всплывающее сообщение, статус измениться на "выполнено",  появиться дата и время выполнения.
        3. Удаление заметки осуществляеться нажатием на пиктограму "удалить" после подтверждения в всплывающем окне заметка будет удалена безвозвратно.
        4. При таких действиях как "удаление", "редактирование", "добавление" появляеться соответствующее всплывающее сообщение в нижнем правом углу рабочей области.
3. При обновлении страницы список дел будет восстановлен из LocalStorage.
4. Для запуска приложения установить  Vue CLI дальше процесс установки стандартный и соответствует инструкции ниже


## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
