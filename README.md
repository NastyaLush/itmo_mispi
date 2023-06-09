# itmo_mispi

<!-- TABLE OF CONTENTS -->
<details>
  <summary>task_lab1</summary>
  <ol>
    Вариант №2005: Халабалу.Ру - Скидки, акции, распродажи и дисконт в Петербурге. Зачем ходить в поисках скидок и акций по городу, если можно зайти на наш сайт и узнать обо всем из первых рук - http://www.hullabaloo.ru/
    
Составить список требований, предъявляемых к разрабатываемому веб-сайту (в соответствии с вариантом). Требования должны делиться на следующие категории:
- Функциональные.
   * Требования пользователей сайта.
   * Требования владельцев сайта.
- Нефункциональные.
    
    
Требования необходимо оформить в соответствии с шаблонами RUP (документ SRS - Software Requirements Specification). Для каждого из требований нужно указать его атрибуты (в соответствии с методологией RUP), а также оценить и аргументировать приблизительное количество часов, требующихся на реализацию этого требования.

Для функциональных требований нужно составить UML UseCase-диаграммы, описывающие реализующие их прецеденты использования.

Вопросы к защите лабораторной работы:

- Методологии разработки ПО. Унифицированный процесс.
- Требования и их категоризация. Атрибуты требований.
- Язык UML.
- Прецеденты использования. UseCase-диаграммы - состав, виды связей.
  </ol>
</details>


<details>
  <summary>task_lab2</summary>
  <ol>
    PS: лабораторная работа выполнена не совсем по тз
    
    
![image](https://github.com/NastyaLush/itmo_mispi/assets/95052885/416c8330-c56d-43f5-b1a9-fe39e8935052)

Сконфигурировать в своём домашнем каталоге репозитории svn и git и загрузить в них начальную ревизию файлов с исходными кодами (в соответствии с выданным вариантом).

Воспроизвести последовательность команд для систем контроля версий svn и git, осуществляющих операции над исходным кодом, приведённые на блок-схеме.

При составлении последовательности команд необходимо учитывать следующие условия:

- Цвет элементов схемы указывает на пользователя, совершившего действие (красный - первый, синий - второй).
- Цифры над узлами - номер ревизии. Ревизии создаются последовательно.
- Необходимо разрешать конфликты между версиями, если они возникают.

Вопросы к защите лабораторной работы:
- Системы контроля версий - назначение, примеры решений.
- Ревизии и ветки.
- Основные операции над данными в системах контроля версий. Основные команды svn и git.
  </ol>
</details>

<details>
  <summary>task_lab3</summary>
  <ol>
    <a href="https://github.com/NastyaLush/itmo_web_jsf_3lab/tree/mispi3">Ссылка на реп</a>
    
    
Написать сценарий для утилиты Apache Ant, реализующий компиляцию, тестирование и упаковку в jar-архив кода проекта из лабораторной работы №3 по дисциплине "Веб-программирование".

Каждый этап должен быть выделен в отдельный блок сценария; все переменные и константы, используемые в сценарии, должны быть вынесены в отдельный файл параметров; MANIFEST.MF должен содержать информацию о версии и о запускаемом классе.

Cценарий должен реализовывать следующие цели (targets):

- **compile** -- компиляция исходных кодов проекта.
- **build** -- компиляция исходных кодов проекта и их упаковка в исполняемый jar-архив. Компиляцию исходных кодов реализовать посредством вызова цели compile.
- **clean** -- удаление скомпилированных классов проекта и всех временных файлов (если они есть).
- **test** -- запуск junit-тестов проекта. Перед запуском тестов необходимо осуществить сборку проекта (цель build).
- **xml** - валидация всех xml-файлов в проекте.
- **env** - осуществляет сборку и запуск программы в альтернативных окружениях; окружение задается версией java и набором аргументов виртуальной машины в файле параметров.


Вопросы к защите лабораторной работы:

- Тестирование ПО. Цель тестирования, виды тестирования.
- Модульное тестирование, основные принципы и используемые подходы.
- Пакет JUnit, основные API.
- Системы автоматической сборки. Назначение, принципы работы, примеры систем.
- Утилита make. Make-файлы, цели и правила.
- Утилита Ant. Сценарии сборки, цели и команды.

  </ol>
</details>

<details>
  <summary>task_lab4</summary>
  <ol>
    <a href="https://github.com/NastyaLush/itmo_web_jsf_3lab/tree/mispi4":>Ссылка на реп</a>
    
    
1. Для своей программы из лабораторной работы #3(смотри главную ветку) по дисциплине "Веб-программирование" реализовать:

+ MBean, считающий общее число установленных пользователем точек, а также число точек, попадающих в область. В случае, если координаты установленной пользователем точки вышли за пределы отображаемой области координатной плоскости, разработанный MBean должен отправлять оповещение об этом событии.
+ MBean, определяющий площадь получившейся фигуры.


2. С помощью утилиты JConsole провести мониторинг программы:

+ Снять показания MBean-классов, разработанных в ходе выполнения задания 1.
+ Определить версию Java Language Specification, реализуемую данной средой исполнения.


3. С помощью утилиты VisualVM провести мониторинг и профилирование программы:

+ Снять график изменения показаний MBean-классов, разработанных в ходе выполнения задания 1, с течением времени.
+ Определить имя потока, потребляющего наибольший процент времени CPU.


4. С помощью утилиты VisualVM и профилировщика IDE NetBeans, Eclipse или Idea локализовать и устранить проблемы с производительностью в программе. По результатам локализации и устранения проблемы необходимо составить отчёт, в котором должна содержаться следующая информация:

+ Описание выявленной проблемы.
+ Описание путей устранения выявленной проблемы.
+ Подробное (со скриншотами) описание алгоритма действий, который позволил выявить и локализовать проблему.
+ Студент должен обеспечить возможность воспроизведения процесса поиска и локализации проблемы по требованию преподавателя.


Вопросы к защите лабораторной работы:

+ Мониторинг и профилирование. Основные понятия. Отличия мониторинга от профилирования.
+ Инфраструктура для организации мониторинга и профилирования в составе JDK. JMX.
+ MBeans. Основные понятия. Архитектура фреймворка.
+ Утилита JConsole. Возможности, область применения.
+ Утилита Visual VM. Возможности, область применения.
+ Удалённый мониторинг и профилирование приложений на платформе Java.

  </ol>
</details>
