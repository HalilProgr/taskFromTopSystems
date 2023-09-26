Задание:
Необходимо привести пример программы или библиотеки на C++,
которая выводит на экран различные геометрические фигуры : круг, квадрат, треугольник, прямоугольник и т.п.
Глубина проработки примера(количество фигур, параметры, методы) на Ваше усмотрение.
Программа не обязательно должна запускаться и работать(хотя это будет плюсом).
В задании Вам необходимо продемонстрировать умение использовать ООП.
Просим не пользоваться библиотекой QT при выполнении задания.


Для решения задачи последнего пункта работы проект собран в VS, в данном проекте я предоставлю 2 подхода
к созданию объектов визуализации:
1) Использование TopoDS_Builder, обощенный интерфей для реализации объектов на основе топологии OpenCascade
2) Использование геометрических примитивов в OpenCascade для построение объектов визуализации

Так как в задании не было уточнено требуется построить только контур примитива или поверхность примитива 
(с учетом заполнения внутренней поверхности), то реализую обе части.

системой визуализации будет VTK, что бы не использовать QtOpenGl.
Приложение будет консольным, где аргумент передаваемый будет обозначать тот или иной примитив.

Реализация будет состоять из классов:

    makerTopoPrimitiv - класс реализующий один из выбранных прмиитивов
    makerTopoSurface 

    makerPrimitiv - класс реализующий один из выбранных прмиитивов
    maerSurface

    hh