# 🧮 Сортировочные алгоритмы

Данный проект содержит реализацию различных сортировочных алгоритмов на C++. Все алгоритмы организованы в соответствующих заголовочных и исходных файлах.

<h2 align="left" id="tech-stack">🔥 Технический стэк</h2>

> Общее

<table width='100%'>
  <tr>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://github.com/devicons/devicon/blob/master/icons/cplusplus/cplusplus-original.svg' width='36' height='36' alt='C++'>
      </a>
      <br>C++
    </td>
  </tr>
</table>

> Системы сборки и управления зависимостями

<table width='100%'>
  <tr>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://www.svgrepo.com/show/373819/makefile.svg' width='36' height='36' alt='Makefile'>
      </a>
      <br>Make
    </td>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://github.com/devicons/devicon/blob/master/icons/nixos/nixos-original.svg' width='36' height='36' alt='Nix'>
      </a>
      <br>Nix
    </td>
  </tr>
</table>

> Контейнеризация

<table width='100%'>
  <tr>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://github.com/devicons/devicon/blob/master/icons/docker/docker-original.svg' width='36' height='36' alt='Docker'>
      </a>
      <br>Docker
    </td>
  </tr>
</table>

> Скрипты

<table width='100%'>
  <tr>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://github.com/devicons/devicon/blob/master/icons/bash/bash-original.svg' width='36' height='36' alt='Bash'>
      </a>
      <br>Bash
    </td>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://github.com/devicons/devicon/blob/master/icons/perl/perl-original.svg' width='36' height='36' alt='Perl'>
      </a>
      <br>Perl
    </td>
  </tr>
</table>

> Тестирование

<table width='100%'>
  <tr>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Google_%22G%22_logo.svg/768px-Google_%22G%22_logo.svg.png' width='36' height='36' alt='Google Benchmark'>
      </a>
      <br>Google Benchmark
    </td>
    <td align='center' width='110' height='90'>
      <a href='#tech-stack'>
        <img src='https://images.vexels.com/content/156537/preview/baseball-glove-icon-baseball-icon-8aebf5.png' width='36' height='36' alt='Catch2'>
      </a>
      <br>Catch2
    </td>
  </tr>
</table>

## 📚 Список реализованных алгоритмов

1. **Bubble Sort** - Простая сортировка с повторяющимся проходом по массиву.
2. **Optimized Bubble Sort** - Улучшенная версия пузырьковой сортировки, которая останавливается, если массив уже отсортирован.
3. **Insertion Sort** - Сортировка вставками, которая строит отсортированный массив, вставляя элементы по одному.
4. **Shell Sort** - Сортировка Шелла, использующая изменяющийся шаг для сортировки элементов на большом расстоянии, что делает её быстрее стандартной сортировки вставками.
5. **Exchange Sort** - Сортировка, основанная на обменах соседних элементов.
6. **Bogo Sort** - Неэффективный алгоритм, который случайно переставляет элементы массива до его сортировки. Средняя сложность O((n+1)!).
7. **Quick Sort** - Быстрая сортировка, использующая метод разбиения массива и рекурсивную сортировку подмассивов.
8. **Selection Sort** - Сортировка выбором, которая последовательно находит минимальный элемент и помещает его на место.
9. **Shaker Sort** - Двунаправленная сортировка, которая проходит по массиву в обе стороны.
10. **Binary Insertion Sort** - Сортировка вставками с использованием бинарного поиска для нахождения позиции вставки.

## 🚀 Начало работы

Для работы с проектом вам потребуется компилятор C++. Вы можете использовать такие инструменты, как `g++`, `clang++` или любой другой, поддерживающий стандарт C++11 и выше.

1. Клонируйте репозиторий:

   ```bash
   git clone git@github.com:Ogorod-corp/sorting.git
   cd sorting
   ```

2. Скомпилируйте исходные файлы:

   ```bash
   g++ -o sort main.cpp src/*.cpp
   ```

3. Запустите программу:

   ```bash
   ./sort
   ```

## 📂 Структура

Вот структура проекта с описанием основных компонентов:

```bash
├── .github                     # CI/CD конфигурации
├── .vscode                     # Настройки Visual Studio Code
├── benchmarks                  # Папка с файлами для бенчмаркинга алгоритмов
├── bin                         # Скомпилированные исполняемые файлы
│   ├── benchmark
│   └── test
├── docs                        # Документация по каждому алгоритму
├── include                     # Заголовочные файлы
├── libs                        # Библиотеки
│   ├── catch2
│   └── benchmark
├── src                         # Исходные файлы с реализацией алгоритмов сортировок
│   ├── bogo.sort.cpp
│   ├── quick.sort.cpp
│   └── ...
├── tests                       # Папка с тестами
│   ├── bogo.sort.test.cpp
│   ├── quick.sort.test.cpp
│   └── ...
├── config.env                  # Конфигурационный файл окружения
├── Dockerfile                  # Dockerfile для контейнеризации
├── Makefile                    # Makefile для сборки проекта
└── shell.nix                   # Конфигурации для Nix
```

## 🔍 Использование

Вы можете использовать любую из реализованных функций сортировки, подключив соответствующий заголовочный файл и вызвав нужную функцию в вашем коде. Например:

```cpp
#include "include/bubble.sort.h"

int main() {
    int arr[] = {64, 34, 25, 12, 22, 11, 90};
    int n = sizeof(arr) / sizeof(arr[0]);

    bubbleSort(arr, n, true); // Сортировка по возрастанию

    // Вывод отсортированного массива
    for (int i = 0; i < n; i++)
        std::cout << arr[i] << " ";

    return 0;
}
```

## 📖 Документация

Документация для каждого из алгоритмов представлена в формате Markdown в папке ./docs. В ней вы найдете описание функций, параметры и примеры использования.

## 📄 Лицензия

Этот проект лицензирован под MIT License. Смотрите файл [LICENSE](LICENSE) для получения дополнительной информации.

## 🤝 Вклад в проект

Если вы хотите внести свой вклад в проект, пожалуйста, создайте новый pull request или откройте issue для обсуждения изменений.
