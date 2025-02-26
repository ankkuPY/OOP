#**Проект ...**

##**Описание**

В данном проекте на данный момент созданы классы для отоброажения информации о продуктах и о категориях продуктов. Так же есть функционал чтения данных из json файла.
В модуле Products параметр self.__price и в модуле Category параметр self.__products установили как приватные. Добавлены сеттеры и геттеры. Добавлена возможность перебора товаров в категории по циклу. Добавлены отображения строк в нужном формате с помощью магических методов. Добавлены новые тесты.

##**Установка**

1. Клонируйте репозиторий:
```
git clone https://github.com/lAntonKuznetsovl/OOP.git
```
2. Установите зависимости:
```
pip install -r requirements.txt
```

##**Использование**

1. Импортируйте необходимые функции:
        ```
        from your_module import Category, Product or reading_json, create_object_from_json
        ```
2. Используйте функции в своем коде:
    Отдельно для каждого продукта:
    ```
        product = Product("Имя продукта", "Описание продукта", цена, количество)

        print(product.name)
        print(product.description)
        print(product.price)
        print(product.quantity)
   ```
   или для данных в json файле:
   ```
        data_list = reading_json(path_to_file) # получение данных из json файла
        classes_objects = create_object_from_json(data_list) # получение объектов класса на основе данных полученных из json файла.
    ```
4. Запуск тестов.
      Чтобы запустить тесты - перейдите в интересующий ваш модуль и запустите тест набрав в терминале команду `pytest`.
      Чтобы посмотртеь на сколько тесты покрывают тот или иной модуль:
          1. Выберите файл с тестами интересующего модуля.
          2. Посмотрите покрытие модуля набрав команду `pytest --cov` в терминале.
          3. Так же можно посмотреть покрытие тестами в HTML-формате, выполните в терминале команду `pytest --cov=src --cov-report=html`.
          4. После, в окне структуры проекта появится дирректория htmlcov. Нажмите правой клавишей мыши на файл index.html. в папке htmlcov, выберите вкладку Open in --> Browser --> "Нужный браузер"

          
