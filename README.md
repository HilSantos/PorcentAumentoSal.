# PorcentAumentoSal.

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace PorcentAumentoSal
{
    public class Program
    {
        static void Main(string[] args)
        {
            double salario = 0, salAumento = 0;
            int op, total;

            Console.WriteLine("Informe o salario: ");
            salario = Convert.ToDouble(Console.ReadLine());

            Console.WriteLine("Salario inicial:" + salario + "\n");
            salAumento = Convert.ToDouble(Console.ReadLine());

            op = Convert.ToInt32(Console.ReadLine());

            if (salario >= 5000)
            {
                Console.WriteLine("Congratulações");
            }
            else if (salAumento >= 3000 && salAumento <= 5000)
            {
                Console.WriteLine("Aplique aliquota de 15%");
            }
            else (salAumento >= 3000 && salAumento <= 3999)
            {
                Console.WriteLine("");
            }

                Console.ReadKey();
            }
        }
    }
}
