# BR-011 Короткая дата (1–3 цифры)

**Описание:**  
При вводе в поле "Дата" значений длиной от 1 до 3 цифр система возвращает сообщение о некорректной дате.

**Шаги воспроизведения:**
1. Перейти по ссылке https://lm.skillbox.cc/qa_tester/module04/homework1/
2. Ввести в поле даты последовательно: `3`, `21`, `132`.
3. После каждого ввода нажать кнопку «УЗНАТЬ».

**Фактический результат:**  
Система отображает сообщение «Некорректная дата».

**Ожидаемый результат:**  
Система должна требовать ввод даты в формате `DD.MM.YYYY`, показывая конкретную подсказку.
