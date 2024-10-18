# PorcentAumentoSal.
Crie um programa que peça ao usuario para inserir seu salario (tipo decimal), e uma porcentagem de aumento (tipo decimal). O programa deve calcular o novo salario, com o aumento aplicado.
Se o novo salario for maior que R$ 5000, exiba uma mensagem de congratulações.
Caso o salario esteja entre R$ 3000 e R$ 5000, use o switch case para determinar o imposto de renda: Se o salario for entre R$ 3000 e R$ 3999, aplique uma aliquota de 15%;
Se o salario for entre R$ 4000 e R$ 4999, aplique uma aliquota de 20%; Exiba o valor do imposto e o salario liquido, após o imposto. Caso contrario, exiba uma mensagem dizendo que o 
salario não será tributado.

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
                Console.WriteLine("Aplique aliquota de 20%");
            }

                Console.ReadKey();
            }
        }
    }
}
