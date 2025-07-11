# Чек-лист проверки поля e-mail

| №  | Проверка                                                               | Ожидаемый результат               | Комментарий |
|----|------------------------------------------------------------------------|-----------------------------------|-------------|
| 1  | Валидный email, содержащий строчные и заглавные буквы                  | Поле принимает значение           |             |
| 2  | Email начинается с цифры в локальной части                             | Поле принимает значение           |             |
| 3  | Email начинается с цифры в доменной части                              | Поле принимает значение           |             |
| 4  | Email с несколькими точками в локальной и доменной частях              | Поле принимает значение           |             |
| 5  | Email с дефисом в локальной части                                      | Поле принимает значение           |             |
| 6  | Email с дефисом в доменной части                                       | Поле принимает значение           |             |
| 7  | Email с нижним подчёркиванием в локальной части                        | Поле принимает значение           |             |
| 8  | Длинный email: локальная часть = 64 символа, доменная = 64 символа     | Поле принимает значение           |             |
| 9  | Пустое поле                                                            | Появляется ошибка                 |             |
| 10 | Превышение длины локальной части (максимум 64 символа)                 | Появляется ошибка                 |             |
| 11 | Превышение длины доменного имени (максимум 63 символа, без точки)      | Появляется ошибка                 | Длина имени каждого домена (между разделительными точками) не может превышать 63 знака, общая же длина имени (включая имена субдоменов, разделительные точки и имя зоны) ограничена 255 знаками.Но на практике чаще всего проверяют только длину доменного имени в 63 символа, не включая точку. |
| 12 | Отсутствие символа `@` в email                                         | Появляется ошибка                 |             |
| 13 | Отсутствие локальной части                                             | Появляется ошибка                 |             |
| 14 | Отсутствие доменной части                                              | Появляется ошибка                 |             |
| 15 | Email содержит две точки подряд                                        | Появляется ошибка                 |             |
| 16 | Локальная часть начинается или заканчивается на `.`                    | Появляется ошибка                 |             |
| 17 | Доменная часть начинается или заканчивается на `.`                     | Появляется ошибка                 |             |
| 18 | Email содержит два дефиса подряд                                       | Появляется ошибка                 |             |
| 19 | Локальная часть начинается или заканчивается на `-`                    | Появляется ошибка                 |             |
| 20 | Доменная часть начинается или заканчивается на `-`                     | Появляется ошибка                 |             |

---

## Полезные ссылки
- Сервис для проверки e-mail: [validate.smtp.bz](https://validate.smtp.bz/)
- Проверка сложности паролей: [Haystack](https://www.grc.com/haystack.htm), [Passcheck](https://exploit.in/passcheck/)
