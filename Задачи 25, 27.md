
{
    //Задача 25: Напишите цикл, который принимает на вход два числа (A и B) 
    //и возводит число A в натуральную степень B.
    //3, 5 -> 243 (3⁵)
    //2, 4 -> 16

    Random random = new Random();
    int number = random.Next(2,3);
    int exponent = random.Next(3,5);
    Console.WriteLine($"Число {number} в степени {exponent} равно {Power(number, exponent)}");
}

int Power( int number, int exponent)
{
    int result = 1;

    for (int i = 0; i < exponent; i++)
    {
        result *= number;
    }
    return result;
}
Zadacha25();

{
//Задача 27: Напишите программу, которая принимает на вход число и выдаёт сумму цифр в числе.
//452 -> 11
//82 -> 10
//9012 -> 12

Random random = new Random();
int number = random.Next (100,1000);

int sum = 0;

Console.Write("В числе " + number);
while(number > 0)
{
    sum += number % 10;
    number /=10;
}

Console.WriteLine("Сумма цифр равна: " + sum);
