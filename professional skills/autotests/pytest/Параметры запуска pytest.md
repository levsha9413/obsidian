В pytest можно запускать с параметрами и создавать свои параметры для запуска. Например чтобы указывать тестовый стенд при запуске или браузер.

Ссылка на доку https://docs.pytest.org/en/6.2.x/example/simple.html

Шаблон куска кода который добавляет параметр, можно сразу прописать несколько параметров: 
//обязательно лежит в conftest.py обычно в корневом
import pytest

def pytest_addoption(parser):
    parser.addoption(
        "--cmdopt", action="store", default="type1", help="my option: type1 or type2", choises=['type1','param1','param2']
    )

Шаблон куска кода который будет парсить введенные значения параметра и вставлять уже в тест:
@pytest.fixture
def cmdopt(request):
    return request.config.getoption("--cmdopt")
	

В отдельном файле лежит тест который использует параметр из фикстуры:
def test_answer(cmdopt):
    if cmdopt == "type1":
        print("first")
    elif cmdopt == "type2":
        print("second")
    assert 0
	
	
Важно: 
не переопределять дефолтные параметры pytest
посмотреть параметры pytest -h

#автоматизация 