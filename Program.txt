using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Diagnostics;

namespace T05_Jaramillo_Regino_Hector_Armando
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Programa Hecho para realizar la suma del 1 al 1,000,000 \nPresione Entrar para empezar");
            Console.ReadKey(true);
            Stopwatch t = new Stopwatch();
            t.Start();
            Console.WriteLine("El valor de la suma de numeros del 1 al 1,000,000 es igual a: {0}", Suma());
            Console.WriteLine("Proceso Realizado en un tiempo de:  {0}", t.Elapsed.ToString());
            t.Stop();
            Console.ReadKey(true);
        }
        public static Decimal Suma()
        {
            decimal suma = 0;
            for (decimal i = 1; i < 1000001; i++) { suma += i; }
            return suma;
        }
    }
}
