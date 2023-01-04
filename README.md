# Unit_25.5

Написать тест, который проверяет, что на странице https://petfriends.skillfactory.ru/my_pets со списком питомцев пользователя:

1) Присутствуют все питомцы.
2) Хотя бы у половины питомцев есть фото.
3) У всех питомцев есть имя, возраст и порода.
4) У всех питомцев разные имена.
5) В списке нет повторяющихся питомцев

- В написанном тесте (проверка карточек питомцев) надо добавить неявные ожидания всех элементов (фото, имя питомца, его возраст).
- В написанном тесте (проверка таблицы питомцев) надо добавить явные ожидания элементов страницы

Файл settings.py - валидные email и пароль

файл conftest.py - фикстура, которая выполняется 1 раз перед тестами, осуществляет переход на страницу Мои питомцы (учитываются варианты как с узким окном браузера, так и с широким, от которых зависит видимость кнопки "Мои питомцы").
Т.к. тестирование входа на страницу "Мои питомцы" не входит в список проверок, считаю данные действия предусловием для тестов. Поэтому действия по переходу на страницу "Мои питомцы" вынесла в фикстуру.

файл test_my_pets.py - пять тестов по указанным выше проверкам. В проверке №1 используется явное ожидание. В остальных проверках - неявные
