# BR-017 Точка в начале доменной части

**Описание:**  
Форма принимает email с точкой в начале доменной части и выполняет регистрацию.  
Под полем E-mail отображается сообщение "Email не удовлетворяет условиям".

**Шаги воспроизведения:**  
1. Перейти по ссылке https://lm.skillbox.cc/qa_tester/module05/homework1/  
2. Ввести телефон: `89112223344`  
3. Ввести email: `test@.ru`  
4. Ввести пароль и подтверждение: `Qwer123!`  
5. Согласиться с обработкой персональных данных.  
6. Нажать кнопку **Зарегистрироваться**.

**Фактический результат:**  
Регистрация проходит успешно, несмотря на точку в начале доменной части.

**Ожидаемый результат:**  
Форма должна отклонить email с точкой в начале доменной части и выдать ошибку валидации.
