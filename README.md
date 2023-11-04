# Ответы 
1)Сложность  https://github.com/PolinaSnigir/labs_aisd/blob/main/Aisd1laba/Aisd1laba.cpp#L155 в худшем случае O(n), потому что при позиции pos <= Count / 2, метод будет выполнять цикл while, что потребует примерно n / 2 итераций.
При позиции pos > Count / 2, метод будет выполнять цикл while, в этом случае количество итераций будет равно n - pos + 1.
Таким образом, в худшем случае, количество итераций составит n, что приводит к алгоритмической сложности O(n).

2)Сложность https://github.com/PolinaSnigir/labs_aisd/blob/main/Aisd1laba/Aisd1laba.cpp#L326 в худшем случае O(1), потому что данный метод проверяет, находится ли индекс в допустимом диапазоне, и возвращает значение элемента массива по этому индексу. Такая операция выполняется независимо от размера массива.

3)Сложность https://github.com/PolinaSnigir/labs_aisd/blob/main/Aisd1laba/Aisd1laba.cpp#L498 в худшем случае O(n), потому что

 Условие isOperand(token):  операцию isOperand(token) можно рассматривать как операцию константного времени, поскольку она зависит от реализации проверки операнда.

 Условие isFunction(token):  можно рассматривать как операцию константного времени.

 Условие isOperator(token):  каждая итерация цикла занимает временную сложность O(1), и количество итераций будет пропорционально размеру стека. В наихудшем случае, когда все операторы имеют одинаковую приоритетность, количество итераций будет равно количеству операторов во входной строке, т.е. O(n).

 Условия token == "(" и token == ")":  в худшем случае, когда все токены являются открывающими или закрывающими скобками, каждая итерация цикла будет выполняться за O(1), и размеры стека operatorStack и строкового потока postfixExpression будут пропорциональны длине входной строки O(n).
 
 Цикл while (!operatorStack.isEmpty()):  в худшем случае, когда стек содержит все операторы из входной строки, количество итераций будет равно количеству операторов, т.е. O(n).