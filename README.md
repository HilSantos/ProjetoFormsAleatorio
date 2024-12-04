# ProjetoFormsAleatorio
CRIE UM PROJETO DE FORMA QUE AO CLICAR EM UM BOTÃO, EXIBA EM UMA LABEL UM NÚMERO INTEIRO ALEATÓRIO, (RESTRINJA A PESQUISA DOS NÚMEROS DE 1 ATÉ 20) - DICA UTILIZE OS CONCEITOS DO RANDOM.

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Reflection.Emit;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace ProjetoFormsAleatorio
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

  private void btnGerarNumero_Click(object sender, EventArgs e)
        {
            Random random = new Random(DateTime.Now.Millisecond);
            int numeroAleatorio = random.Next(1, 21);
            lblResultado.Text = numeroAleatorio.ToString();
        }
    }
}
