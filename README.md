query
Легенда
В рамках изучения Java Core и изучения работы протокола HTTP вы использовали библиотеку HttpClient из состава Apache HttpComponents.

В состав данной библиотеки входит утилитный класс URLEncodedUtils, который и позволяет "парсить" Query String, извлекая параметры.

Необходимо добавить в ваш сервер (из предыдущего ДЗ) функциональность обработки параметров запроса так, чтобы можно было из объекта типа Request отдельно получать и путь запроса, и параметры из Query String.

Например, это можно сделать в виде метода getQueryParam(String name) и getQueryParams(). Подумайте, что они должны возвращать, исходя из документации на утилитный класс.

Задача
Подключите к своему проекту HttpClient
Реализуйте функциональность по обработке параметров из Query
При необходимости, доработайте функциональность поиска handler'а так, чтобы учитывался только путь без Query: т.е. handler, зарегистрированный на "/messages", обрабатывал и запросы "/messages?last=10"
Результат
Реализуйте новую функциональность в ветке feature/query вашего репозитория из ДЗ 1 и откройте Pull Request.

Поскольку вы - главный архитектор и проектировщик данного решения (уже более функционального), то все архитектурные решения принимать вам, но будьте готовы к критике со стороны проверяющих.

В качестве результата пришлите ссылку на ваш Pull Request на GitHub в личном кабинете студента на сайте netology.ru.

После того, как ДЗ будет принято, сделайте merge для Pull Request'а.

x-www-form-urlencoded* (задача со звёздочкой)
Важно: выполнение данного ДЗ не влияет на получение зачёта по ДЗ.

Легенда
Необходимо добавить в ваш сервер (из предыдущего ДЗ) функциональность обработки тела, оформленного в виде x-www-form-url-encoded, запроса так, чтобы можно было из объекта типа Request отдельно параметры, переданные в теле запроса.

Например, это можно сделать в виде метода getPostParam(String name) и getPostParams(). Подумайте, что они должны возвращать, исходя из того, что в передаваемой вам форме может быть два параметра с одинаковым именем.

Задача
Реализуйте функциональность по обработке тела запроса, если он представлен в виде x-www-form-urlencoded.

Результат
Реализуйте новую функциональность в ветке feature/form вашего репозитория из предыдущего ДЗ и откройте Pull Request.

Поскольку вы - главный архитектор и проектировщик данного решения (уже более функционального), то все архитектурные решения принимать вам, но будьте готовы к критике со стороны проверяющих.

В качестве результата пришлите ссылку на ваш Pull Request на GitHub в личном кабинете студента на сайте netology.ru.

После того, как ДЗ будет принято, сделайте merge для Pull Request'а.

multipart/form-data* (задача со звёздочкой)
Важно: выполнение данного ДЗ не влияет на получение зачёта по ДЗ.

Легенда
Почему бы не реализовать "полную" функциональность и не добавить поддержку multipart-запросов? Используйте библиотеку FileUpload, чтобы добавить подобную функциональность.

Например, это можно сделать в виде метода getPart(String name) и getParts(). Подумайте, что они должны возвращать, исходя из того, что:

В передаваемой вам форме может быть два параметра с одинаковым именем
Каждый Part может быть как файлом, так и обычным полем
Всё это значит, что нужно как-то уметь отличать обычные поля от файлов.

Задача
Реализуйте функциональность по обработке тела запроса, если от представлен в виде multipart/form-data.

Поскольку вы - главный архитектор и проектировщик данного небольшого класса, то все архитектурные решения принимать вам, но будьте готовы к критике со стороны проверяющих.

Результат
Реализуйте новую функциональность в ветке feature/multipart вашего репозитория из предыдущего ДЗ и откройте Pull Request.

Поскольку вы - главный архитектор и проектировщик данного решения (уже более функционального), то все архитектурные решения принимать вам, но будьте готовы к критике со стороны проверяющих.

В качестве результата пришлите ссылку на ваш Pull Request на GitHub в личном кабинете студента на сайте netology.ru.

После того, как ДЗ будет принято, сделайте merge для Pull Request'а.
