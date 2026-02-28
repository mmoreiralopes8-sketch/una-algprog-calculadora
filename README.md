Resposta 
1. dotnet new webapi/dotnet new xunit
2. Criado
3. net10.0

Codigo VisualStudio

// See https://aka.ms/new-console-template for more information
using Microsoft.VisualBasic;

Console.WriteLine("Calculadora");

Console.WriteLine("Digite o primeiro número: ");
double num1 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Digite o segundo número: ");
double num2 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Escolha uma operação:");
Console.WriteLine("1 - Adição");
Console.WriteLine("2 - Subtração");
Console.WriteLine("3 - Multiplicação");
Console.WriteLine("4 - Divisão");
int operacao = Convert.ToInt32(Console.ReadLine());

switch (operacao)
{
case 1:
    Console.WriteLine($"Resultado: {num1 + num2}");
    break;
case 2: 
    Console.WriteLine($"Resultado: {num1 - num2}");
    break;
case 3:
    Console.WriteLine($"Resultado: {num1 * num2}");
    break;
case 4:
    if (num2 !=0)
      Console.WriteLine($"Resultado: {num1 / num2}");
    else
      Console.WriteLine("Erro: Divisão por zero não é permitida");
    break;
default:
    Console.WriteLine("Operação inválida. ");

    break;
}


   
