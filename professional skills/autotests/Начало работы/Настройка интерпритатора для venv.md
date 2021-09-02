При использовании [[venv]] важно использовать интерпритатор питона также из виртуального окружения. В pycharm для этого нужно перейти в  interpriteter settings и указать путь к venv для данного проекта.

Увидеть, что используется нужный интерпритатор, можно в первой строке вывода скрипта в консоли, например:
```
C:\autotests\example_repo_1\venv\Scripts\python.exe C:/autotests/example_repo_1/example.py
Hello, world!

Process finished with exit code 0
```
В данном случае 
```
C:\autotests\example_repo_1\venv\Scripts\python.exe
```
нужный нам интерпритатор из venv

#python #автоматизация 