# BR-027 — Пустой пароль при авторизации

## Описание
Если в форме авторизации оставить поле Пароль пустым, система всё равно пускает в личный кабинет.

## Шаги воспроизведения
1. Перейти по ссылке https://lm.skillbox.cc/qa_tester/module06/auth/index.html
2. Ввести в поле E-mail: `skillbox@test.ru`
3. Поле Пароль оставить пустым
4. Нажать кнопку "Войти"

## Фактический результат
- Пользователь попадает в личный кабинет.
- Под полем Пароль выводится сообщение: `Пароль не относится к почте`

## Ожидаемый результат
- Авторизация не должна проходить, если поле Пароль пустое.
- Должно появиться сообщение о необходимости ввести пароль.
