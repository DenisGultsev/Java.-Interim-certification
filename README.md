# PhoneBook

Пояснение к коду
Предоставленный код - это программа на языке Java, которая реализует простое приложение телефонной книги. Она позволяет пользователям добавлять, удалять и искать номера телефонов по фамилии. Данные телефонной книги хранятся в HashMap, а программа читает и записывает данные в файл "phonebook.txt".

Давайте разобьем код на разные блоки:

Импорт инструкций
Код начинается с нескольких инструкций импорта, которые импортируют необходимые классы из пакетов java.io и java.util. Эти классы используются для операций ввода/вывода файлов, хранения данных и ввода пользовательских данных.

Определение класса
Код определяет публичный класс с именем Phonebook. Этот класс содержит метод main, который служит точкой входа в программу.

Метод main
Метод main - это место, где начинается выполнение программы. Он выполняет следующие шаги:

Создает новый HashMap с именем phoneBook для хранения данных телефонной книги.
Создает новый объект Scanner для чтения пользовательского ввода с консоли.
Входит в цикл while, который продолжается, пока пользователь не введет команду "exit".
Внутри цикла while программа читает данные телефонной книги из файла "phonebook.txt" и заполняет HashMap phoneBook.
Печатает данные телефонной книги в порядке убывания количества номеров телефонов, связанных с каждой фамилией.
Предлагает пользователю ввести команду и выполняет соответствующее действие на основе введенных пользователем данных.
Если пользователь вводит "add", программа запрашивает фамилию и номер телефона, добавляет запись в HashMap phoneBook и выводит сообщение об успешном добавлении.
Если пользователь вводит "del", программа запрашивает фамилию, удаляет соответствующую запись из HashMap phoneBook, если она существует, и выводит сообщение об успешном или неудачном удалении.
Если пользователь вводит "num", программа запрашивает фамилию, извлекает соответствующий номер телефона из HashMap phoneBook, если он существует, и выводит его.
Если пользователь вводит "sur", программа запрашивает номер телефона, ищет соответствующую фамилию в HashMap phoneBook, если она существует, и выводит ее.
Если пользователь вводит "save", программа записывает данные телефонной книги из HashMap phoneBook в файл "phonebook.txt" и выводит сообщение об успешном сохранении.
Если пользователь вводит "exit", программа выходит из цикла while и выводит сообщение о выходе.
Если пользователь вводит недопустимую команду, программа выводит сообщение об ошибке.
После цикла while программа снова читает данные телефонной книги из файла "phonebook.txt" и выводит их на консоль.
Вспомогательные методы
Код также включает вспомогательный метод с именем printPhoneBookDescending, который принимает входные данные в виде HashMap phoneBook и выводит его содержимое в порядке убывания количества номеров телефонов, связанных с каждой фамилией. Этот метод вызывается в методе main для отображения данных телефонной книги.

В целом, код предоставляет базовую реализацию приложения телефонной книги с использованием HashMap для хранения данных и файлового ввода/вывода для сохранения данных.
