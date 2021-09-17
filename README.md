using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;  

class Program {
  public static void Main (string[] args) {
    int num1, num2, opcion, i, j;
    double valor, potencia, cont;
    do{
    Console. Clear();
    Console.WriteLine("Menu de opciones");
    Console.WriteLine("1. Suma");
    Console.WriteLine("2. Resta");
    Console.WriteLine("3. Multiplicacion");
    Console.WriteLine("4. Division");
    Console.WriteLine("5. Potenciacion");
    Console.WriteLine("6. Raiz");
    Console.WriteLine("7. Logaritmo");
    Console.WriteLine("8. Salir");
    Console.WriteLine("Introduzca opcion (1-7): ");
    opcion = int.Parse(Console.ReadLine());

     switch ( opcion )
        {
            case 1: Console.WriteLine("SUMA:");
                    Console.WriteLine("Digite primer numero:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite segundo numero:");
                    num2 = int.Parse(Console.ReadLine());
                    valor = num1 + num2;
                    Console.WriteLine("La respuesta es: " + valor);
                    System.Console.ReadKey();
                    break;

            case 2: Console.WriteLine("RESTA:");
                    Console.WriteLine("Digite primer numero:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite segundo numero:");
                    num2 = int.Parse(Console.ReadLine());
                    valor = num1 - num2;
                    Console.WriteLine("La respuesta es: " + valor);
                    System.Console.ReadKey();
                    break;


            case 3: Console.WriteLine("MULTIPLICACION:");
                    Console.WriteLine("Digite primer numero:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite segundo numero:");
                    num2 = int.Parse(Console.ReadLine());
                    valor = num1 * num2;
                    Console.WriteLine("La respuesta es: " + valor);
                    System.Console.ReadKey();
                    break;

            case 4: Console.WriteLine("DIVISION:");
                    Console.WriteLine("Digite primer numero:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite segundo numero:");
                    num2 = int.Parse(Console.ReadLine());
                    valor = num1 / num2;
                    Console.WriteLine("La respuesta es: " + valor);
                    System.Console.ReadKey();
                    break;

            case 5: Console.WriteLine("POTENCIACION:");
                    Console.WriteLine("Digite base:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite exponente:");
                    num2 = int.Parse(Console.ReadLine());
                    i = 1;
                    valor = num1;
                    do{
                      valor = valor * num1;
                      i = i + 1;
                    }while (i < num2);
                    Console.WriteLine("La respuesta es: " + valor);
                    System.Console.ReadKey();
                    break;

            case 6: Console.WriteLine("RAIZ:");
                    Console.WriteLine("Digite radicando:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite indice:");
                    num2 = int.Parse(Console.ReadLine());
                    i = 1;
                    j = 1;
                    potencia = 1;
                    do{
                      j=1;
                      do{
                        potencia = potencia * i;
                        j = j + 1;
                      }while (j < num2);
                      i = i +1;
                      valor = potencia;
                      potencia = i;
                    } while(valor != num1);
                    i = i-1;
                    Console.WriteLine("La respuesta es: " + i);
                    System.Console.ReadKey();
                    break;
            
            case 7: Console.WriteLine("LOGARITMO:");
                    Console.WriteLine("Digite base:");
                    num1 = int.Parse(Console.ReadLine());
                    Console.WriteLine("Digite antilogaritmo:");
                    num2 = int.Parse(Console.ReadLine());
                    i = 1;
                    valor = num2;
                    do{
                      valor = valor / num1;
                      i = i + 1;
                    }while (valor != num1);
                    Console.WriteLine("La respuesta es: " + i);
                    System.Console.ReadKey();
                    break;

            case 8: Console.WriteLine("Adios vuelva pronto!");
            System.Console.ReadKey();
                    break;  
             
            default:
                    Console.WriteLine("OPCION INVALIDA!");
                    System.Console.ReadKey();
                    break;
         }
          

    } while ( opcion != 8 );
   
  }
}
