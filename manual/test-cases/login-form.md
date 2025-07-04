# 🔐 Тест-кейсы — Форма авторизации

## 📘 Описание
Форма логина состоит из двух полей (Email и Password) и кнопки "Login".  
Протестируем базовые сценарии — как позитивные, так и негативные.

---

## ✅ TC-001. Успешный вход с валидными данными

**Предусловия:** Пользователь зарегистрирован

- **Шаги:**
  1. Открыть страницу логина
  2. Ввести корректный Email
  3. Ввести корректный пароль
  4. Нажать кнопку "Login"

- **Ожидаемый результат:**  
  Пользователь авторизован, происходит переход в личный кабинет

---

## ❌ TC-002. Вход с неверным паролем

- **Шаги:**
  1. Ввести корректный Email
  2. Ввести неправильный пароль
  3. Нажать "Login"

- **Ожидаемый результат:**  
  Ошибка "Неверный логин или пароль", авторизация не происходит

---

## ⚠️ TC-003. Попытка входа с пустыми полями

- **Шаги:**
  1. Оставить оба поля пустыми
  2. Нажать "Login"

- **Ожидаемый результат:**  
  Ошибка валидации: поля подсвечены, сообщение "Заполните все поля"

---

## 🧪 TC-004. Ввод email без "@" (невалидный формат)

- **Шаги:**
  1. Ввести "userexample.com" в поле Email
  2. Ввести любой пароль
  3. Нажать "Login"

- **Ожидаемый результат:**  
  Ошибка валидации: "Введите корректный email"
