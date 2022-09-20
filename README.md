 ## Условие задачи
1. Задача: Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых
меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте
выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись
исключительно массивами.
2. ### Нарисовать блок-схему алгоритма решения задачи
![Блок-схема](https://github.com/Igor8814/Git_Test/blob/main/Screenshot_30.png)

## Код решения задачи :
~~~
void FillArray(string[] args)

{  
    Console.WriteLine("Введите   элементы массива: "); 
    for (int i = 0; i < args.Length; i++)
    {
        args[i] = new String(Console.ReadLine());
    }
}
void PrintArr(string[] args)
{
    Console.WriteLine("Первоначальный массив:");
    for (int i = 0; i < args.Length; i++)
    {
        Console.Write($"{args[i]} ");
    }
}
void NewStringArr(string[] array)
{
    Console.WriteLine("Новый массив:");
    for (int i = 0; i < array.Length; i++)
    {
        if (array[i].Length <= 3)
        {
            Console.Write($"{array[i]} ");
        }
    }
}
string[] stringArray = new string[4];
FillArray(stringArray);
PrintArr(stringArray);
Console.WriteLine();
NewStringArr(stringArray);
~~~