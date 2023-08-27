#                         План тестирования.
#    Возможности записаться на обучение "Профессия Тестировщик"
##       Переходом через "Каталог курсов"
1. Зайти на сайт https://netology.ru/
2. Нажать на меню "Каталог курсов";
3. Выбрать "Программирование";
4. Пролистать до профессии "Профессия Тестировщик";
5. Кликнуть на профессию;
6. Кликнуть кнопку записаться, находящуюся в шапке сайта, справа от меню входа.
##          Переходом через главную страницу 
1. Зайти на сайт https://netology.ru/
2. В меню "Направления обучения" выбрать "Программирование";
3. Выбрать однин из курсов по тестированию (кликнуть на него)
4. Отроется страница с описанием кликнуть по кнопке Записаться или прокрутить 
       страницу в самый низ, до формы записи.

#      Тесты ввода валидных и невалидных данных.

##     Валидные значения для поля "Имя"
     1.  Текст на кириллице;
     2.  Не менее 2ух символов;
     3.  Допустимо использование ё/й;
     4.  Допустимо двойное имя через пробел или "-";
Пример: Пётр.
##   Невалидные данные для поля "Имя"
     1. Текст на латинице;
     2. Меньше 2ух символов;
     3. Максимально возможное кол-во символов;
     4. Иероглифы;
     5. Цифры;
     6. Спецсимволы; 

##   Валидные значения для поля "Телефон"
1. Начинается с +7;
2. Содержит 10 цифр после +7.
3. Пример: "+7 900 100 00 00".


##     Невалидные данные для поля "Телефон"
1.  Не используется +7;
2.  Меньше 10 цифр после +7;
3.  Больше 10 цифр;
4.  Спецсимволы;
5.  Буквы;

##   Валидные значения для поля "Электронная почта"
  
1. Текст на латинице;
2. Используется @;
3. Введен текст до и после @;
4. После @ используется точка.

##    Невалидные значения для поля "Электронная почта"
  
1. Текст на кириллице;
2.  Не используется @;
3.  Отсутствует текст до @;
4.  Отсутствует текст после @;
5.  Нет точки после @;


##    Позитивный сценарий тестирования формы записи на курс
1. Выполнить переход к форме записи
2. Ввести валидное значение в поле "Имя"
3. Ввести валидное значение в поле "Телефон"
4. Ввести валидное значение в поле "Электронная почта"
5. Нажать на кнопку "Записаться"
Ожидаемый результат: Форма заполнена (сообщение об удачной записи)


##    Негативный сценарий тестирование формы записи на курс
1. Выполнить переход к форме записи
2. Ввести невалидное значение в поле "Имя"
3. Ввести валидное значение в поле "Телефон"
4. Ввести валидное значение в поле "Электронная почта"
5. Нажать на кнопку "Записаться"
Ожидаемый результат: Ошибка заполнения поля "Имя" 

#    Перечень используемых инструментов с обоснованием выбора.
1. Язык программирования JAVA. Выбрал, потому что другого языка не знаю;
2. Интегрированная среда разработки IntelliJ IDEA Community Edition 2023.1. Пробовал Visual Studio, IntelliJ показалась удобнее;
3. Система автоматической сборки Gradle. Gradle проще и компактнее, чем Maven;
4. Фреймворк для автоматизированного тестирования веб-приложений Selenide. Понятнее и проще чем Selenium;
5. Библиотека для генерации тестовых данных Faker;
6. Библиотека, позволяющая сократить шаблонный код Lombok;
7. Фреймворк для создания отчетов Allure. Проще в освоении и понятнее аналогов;
8. Паттерны тестирование, как Page objects.

#     Перечень необходимых разрешений, данных и доступов.
1. Разрашение на тестирование от владельца
2. Доступ к тестовой БД(если имеется)
3. Доступ к API(если имеется)

#     Перечень и описание возможных рисков при автоматизации.
* Отсуцтвие тестовых меток.
* Во время тестирование сервис должен работать;
* Во время тестирования разработчики могут обновить приложение

#     Перечень необходимых специалистов для автоматизации.
*     Один Авто-Тестировщик.

#     Интервальная оценка с учётом рисков в часах.
*   2-4 рабочих дня (16-36 ч.) (Если мало опыта)
