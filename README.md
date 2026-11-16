# Лабораторная работа №4. Rails-приправленный Ruby

Учебное приложение sample app по книге *Ruby on Rails Tutorial* (глава 4).
Проект продолжает лабораторную работу №3 (статические страницы).

Выполнил: Мифтахов Р. Н., группа 4411.

## Что сделано

- хелпер `full_title` в `app/helpers/application_helper.rb` — формирует заголовок страницы;
- макет `app/views/layouts/application.html.erb` использует `full_title(yield(:title))`;
- на странице Home убран `provide(:title, ...)`, тест ждёт базовый заголовок;
- класс `User` в `example_user.rb` (`attr_accessor`, `initialize`, `formatted_email`, `alphabetical_name`);
- упражнения главы 4 — по одному файлу в каталоге `exercises/`.

## Запуск

```sh
bundle install
bin/rails test          # тесты
bin/rails server        # http://localhost:3000
ruby exercises/exercise_5_palindrome_check.rb
bin/rails runner exercises/exercise_8_array_access.rb
```

Отчёт по работе: `Отчет_ЛР4_Мифтахов.docx`.
