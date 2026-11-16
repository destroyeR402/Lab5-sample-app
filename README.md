# Лабораторная работа №5. Заполнение макета

Учебное приложение sample app по книге *Ruby on Rails Tutorial* (глава 5).
Проект продолжает лабораторную работу №4.

Выполнил: Мифтахов Р. Н., группа 4411.

## Что сделано

- подключён Bootstrap 3 и собственные стили на Sass (`app/assets/stylesheets/application.scss`, гем `dartsass-rails`);
- макет разбит на частичные шаблоны `_header.html.erb` и `_footer.html.erb`;
- именованные маршруты: `root`, `/help`, `/about`, `/contact`, `/signup`;
- контроллер `Users` с действием `new` — заготовка страницы регистрации;
- интеграционный тест ссылок макета `test/integration/site_layout_test.rb` и тест хелпера `full_title`.

## Запуск

```sh
bundle install
bin/rails dartsass:build   # собрать CSS из Sass
bin/rails test             # тесты
bin/dev                    # сервер + слежение за Sass, http://localhost:3000
```

Отчёт по работе: `Отчет_ЛР5_Мифтахов.docx`.
