# Dir_Hide

Как использовать:

    Установите зависимости:

    pip install requests

-------

    Создайте файл wordlist.txt с путями для проверки, например:

    /admin
    /login
    /backup
    /config
    /test
    /secret

    -------

    Запустите инструмент:
    
    python dir_hide.py http://example.com wordlist.txt -t 20 -x .php .html -o results.txt

   -------

Параметры командной строки:

    url: Базовый URL для сканирования.

    wordlist: Путь к файлу со словарем.

    -t, --threads: Количество потоков (по умолчанию 10).

    -x, --extensions: Расширения файлов для проверки (например, .php, .html).

    -o, --output: Файл для сохранения результатов.

    -p, --proxy: Прокси для использования (например, http://127.0.0.1:8080).

    -T, --timeout: Тайм-аут запроса в секундах (по умолчанию 5).

    -u, --user-agent: Пользовательский заголовок User-Agent.


    

Особенности:

    Многопоточность: Использует ThreadPoolExecutor для ускорения перебора.

    Расширения файлов: Поддерживает проверку путей с различными расширениями.

    Логирование: Выводит подробные логи в консоль.

    Сохранение результатов: Сохраняет найденные пути в файл.

    Гибкость: Поддерживает прокси, кастомные заголовки и тайм-ауты.


Этот инструмент является мощным и гибким решением для поиска скрытых ресурсов на веб-серверах. 

------

Используйте его только в законных целях!
