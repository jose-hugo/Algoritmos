# Algoritmos

Área triângulo

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int a, b, c, d;
   
   float base, altura, area;
   
   printf ("Digite a base: ");
   scanf ("%f",&base);
   
   printf ("Digite a altura: ");
   scanf ("%f",&altura);
   
   area = (base*altura) / 2;
   
   printf ("Área = %.2f\n\n", area);
  
  
   system("PAUSE");
}

Caso - 7 Opções Menu Sistema

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int op;
   printf ("\nSistema para Controle de Clientes:\n\n ");
   printf ("\n______________________________________\n\n");
   printf ("*   1) Cadastro de clientes       *\n");
   printf ("*   2) Alteração de dados         *\n");
   printf ("*   3) Excluir cadastro           *\n");
   printf ("*   4) Pesquisar cliente          *\n");
   printf ("*   5) Relatório de clientes      *\n");
   printf ("*   6) Configurações              *\n");
   printf ("*   7) Finalizar o sistema        *\n");
   printf ("\n______________________________________\n\n");
   printf ("Digite a opção desejada: ");
   scanf ("%d", &op);
   switch(op)
   {
      case 1: { printf ("\nVocê selecionou a opção Cadastro de clientes\n\n"); break; }   
      case 2: { printf ("\nVocê selecionou a opção Alteração de dados\n\n"); break; } 
      case 3: { printf ("\nVocê selecionou a opção Excluir cadastro\n\n"); break; } 
      case 4: { printf ("\nVocê selecionou a opção Pesquisar cliente\n\n"); break; } 
      case 5: { printf ("\nVocê selecionou a opção Relatório de clientes\n\n"); break; } 
      case 6: { printf ("\nVocê selecionou a opção Configurações\n\n"); break; } 
      case 7: { printf ("\nVocê selecionou a opção Finalizar o sistema\n\n"); break; } 
      default: { printf ("\nOpção inválida!!!\n\n"); }     
   }       
   system("PAUSE");
}

Caso Calculadora

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   float n1, n2, res;
   char op;
   printf ("\nCalculadora simples - Menu de opções\n\n");
   printf ("________________________________\n\n");
   printf ("*    (+) Soma                  *\n");
   printf ("*    (-) Subtração             *\n");
   printf ("*    (*) Multiplicação         *\n");
   printf ("*    (/) Divisão               *\n");
   printf ("*    (p) Potenciação           *\n");
   printf ("*    (r) Raíz quadrada         *\n");
   printf ("*    (s) Sair do sistema       *\n");
   printf ("________________________________\n");
   printf ("\nDigite o primeiro número: ");
   scanf ("%f",&n1);
   printf ("\nDigite o segundo número: ");
   scanf ("%f",&n2);
   printf ("\nEscolha a operação matemática desejada: ");
   op = getche();
   switch(op)
   {
      case '+': { res = n1+n2;
                printf ("\n\nSoma = %.1f\n\n", res); break; }   
      case '-': { res = n1-n2;
                printf ("\n\nSubtração = %.1f\n\n", res); break; }   
      case '/': if (n2 == 0){
                printf("\n\nImpossível dividir por 0\n\n", res);}     
                else {
                res = n1/n2;
                printf ("\n\nDivisão = %.1f\n\n", res);} break;
      case '*': { res = n1*n2;
                printf ("\n\nMultiplicação = %.1f\n\n", res); break; }
      case 'p': { res = pow(n1,n2);
                printf ("\n\nPotenciação = %.1f\n\n", res); break; }
      case 'r': { res = sqrt(n1);
                printf ("\nRaíz quadrada do primeiro número = %.1f\n\n",res); 
                res = sqrt(n2);
                printf ("\nRaíz quadrada do segundo número = %.1f\n\n",res); break; }
      default: { printf ("\nOpção inválida!!!\n\n"); }     
   }       
   system("PAUSE");
}

Caso - Mês do Ano

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int a;
   char op;
   printf ("Digite um número entre 1 a 12 para saber o mês do ano: ");
   scanf ("%d",&a);
   switch(a)
   {
      case 1: { printf ("\nJaneiro\n\n"); break; }   
      case 2: { printf ("\nFevereiro\n\n"); break; } 
      case 3: { printf ("\nMarço\n\n"); break; } 
      case 4: { printf ("\nAbril\n\n"); break; } 
      case 5: { printf ("\nMaio\n\n"); break; } 
      case 6: { printf ("\nJunho\n\n"); break; } 
      case 7: { printf ("\nJulho\n\n"); break; } 
      case 8: { printf ("\nAgosto\n\n"); break; } 
      case 9: { printf ("\nSetembro\n\n"); break; } 
      case 10: { printf ("\nOutubro\n\n"); break; } 
      case 11: { printf ("\nNovembro\n\n"); break; } 
      case 12: { printf ("\nDezembro\n\n"); break; } 
      default: { printf ("\nMês do ano inválido!!!\n\n"); }     
   }       
   system("PAUSE");
}

Desconto Compra

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int pagamento;
   float valorproduto, valortotal;
   char avistadinheiro, avistacartao, duasparcelas, tresparcelas;
   
     printf ("Qual o valor do produto: ");
   scanf("%f",&valorproduto);
   
     printf ("\nSelecione a forma de pagamento:\n\n1 - À vista no dinheiro\n2 - À vista no cartão\n3 - 2 Parcelas\n4 - 3 Parcelas\n\nOpção: ");
     scanf ("%d",&pagamento);  
   
   if (pagamento == 1){
   valortotal = valorproduto - (valorproduto * 0.10);   
   
   }else if (pagamento == 2){
   valortotal = valorproduto - (valorproduto * 0.05);
   
   }else if (pagamento == 3){
   valortotal = valorproduto; 
   
   }else if (pagamento == 4){
   valortotal = valorproduto + (valorproduto * 0.10); }  
   
   printf ("\n--------------------------------------\n");
   printf ("Valor Total com desconto: %.2f\n\n", valortotal);
   
   
   system("PAUSE");
}

Dobro Número 5x - While

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int dobro=0,i=1,num;
      while(i <= 5 )
      {    
          printf("Digite um numero: ");  
          scanf("%d",&num);
          dobro = num * 2;
          printf("Dobro = %d\n",dobro); 
          i = i + 1; 
      }  
      system("PAUSE");
} 

Dobro número

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()

{       
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int n, dobro, i ;
   for (i = 1 ; i <= 5 ; i = i+1)
   {
       printf ("Digite um número: ");
       scanf ("%d", &n);
       dobro = n+n;    
       printf ("Dobro: %d\n\n", dobro);
       _sleep(100);
   }    
   system("PAUSE");
}

exercicio casos semana

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int a;
   printf ("Digite um número entre 1 e 7 para saber o dia da semana: ");
   scanf ("%d",&a);
   switch(a)
   {
      case 1: { printf ("Domingo\n\n"); break; }   
      case 2: { printf ("Segunda-feira\n\n"); break; }   
      case 3: { printf ("Terça-feira\n\n"); break; }
      case 4: { printf ("Quarta-feira\n\n"); break; }
      case 5: { printf ("Quinta-feira\n\n"); break; }
      case 6: { printf ("Sexta-feira\n\n"); break; }
      case 7: { printf ("Sábado\n\n"); break; }   
      default: { printf ("Dia da semana inválido!!!\n\n"); }     
   }       
   system("PAUSE");
}

exercicio laco numero impar 0 a 100.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int num;
   printf ("Números ímpares de 0 à 100\n\n\n");
   for(num = 1 ; num <= 100 ; num = num + 2) 
   {
       printf ("Número ímpar = %d\n", num);  
       _sleep(100);     
   }   
        
   system("PAUSE");
}

funcao while soma salario funcionarios.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()

{       
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   float soma=0, salario;
   printf ("Cálculo de salários, termina com salário = 0\n\n\n");   
   salario = 1;
   while (salario != 0)
      {        
       printf ("Digite o salário do funcionário: ");  
       scanf ("%f", &salario);     
       soma = soma + salario;    
   }        
       
       printf ("\nA soma dos salários é: %.2f\n\n", soma);
       
   system("PAUSE");
}
 
idade nadador.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int idade;
   
   printf ("Idade do nadador: ");
   
   scanf ("%d",&idade);
   
   if (idade >= 5 && idade <=  7)
   printf ("Infantil A\n");
   
   else if (idade >=8 && idade <=10)
   printf ("Infantil B\n");
   
   else if (idade >=11 && idade <=13)
   printf ("Juvenil A\n");
   
   else if (idade >=14 && idade <=17)
   printf ("Juvenil B\n");
   
   else if (idade >= 18)
   printf ("Adulto\n");
  
   system("PAUSE");
}

imc.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   float peso, altura, imc;
   
   printf ("Digite o peso: ");
   scanf ("%f",&peso);
   
   printf ("Digite a altura: ");
   scanf ("%f",&altura);
   
   imc = peso / (altura*altura);
   printf ("IMC = %.1f \n",imc);
   
   if (imc < 18.5)
      printf ("Abaixo do peso ideal\n");
   
   else if (imc >= 18.5 && imc <= 24.9)
      printf ("Peso normal\n");
   
   else if (imc >= 25 && imc <= 29.9)
      printf ("Acima de seu peso\n");
   
   else if (imc >= 30 && imc <= 34.9)
      printf ("Obesidade grau I\n");
   
   else if (imc >= 35 && imc <= 39.9)
      printf ("Obesidade grau II\n");
   
   else if (imc >= 40)
      printf ("Obesidade grau III\n");
   
   system("PAUSE");
}

numero a b maior menor.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int a, b, maior, menor;   

   printf ("Digite o primeiro número: ");
   scanf ("%d", &a);
   
   printf ("Digite o segundo número: ");
   scanf ("%d", &b);  
   
   // Se A for igual a B
   if (a == b) {
      printf ("Números iguais\n");   
   } else
   // Se A > B
   if (a > b){
      printf ("Maior = %d e Menor = %d\n", a, b);
    // Se A < B  
   } else {
     printf ("Maior = %d e Menor = %d\n", b, a);     
   }      
 
   system("PAUSE");
}

numero impar 0 a 100 while.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int num=1;
      printf("\nNumeros impares de 0 ate 100\n\n\n");
      while(num <= 100)
      {    
          printf("Numero impar = %d\n",num);  
          _sleep(30);
          num = num + 2;  
      }  
      system("PAUSE");
} 

numero maior entre 2 continuar ou parar while.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int n1, n2;
      char op = 's';
      
      while (op == 's')
      {
      printf("\n\nInfome o 1 numero:");
      scanf ("%d",&n1);
      printf("Infome o 2 numero:");
      scanf ("%d",&n2);  
      if (n1==n2)
         printf ("Numeros iguais!!\n");   
      else
          {  
             if (n1 >= n2)
                printf("\nN1 Maior\n\n");
             else 
                printf ("\nN2 Maior\n\n");  
          }   
          printf ("\nDeseja continuar ? (s/n):");
          op = getche();
      }
      system("PAUSE");
} 


numero menor.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int n1, n2;
      char op = 's';
      
      while (op == 's')
      {
      printf("\n\nInfome o 1 numero:");
      scanf ("%d",&n1);
      printf("Infome o 2 numero:");
      scanf ("%d",&n2);  
      if (n1==n2)
         printf ("Numeros iguais!!\n");   
      else
          {  
             if (n1 >= n2)
                printf("\nN1 Maior\n\n");
             else 
                printf ("\nN2 Maior\n\n");  
          }   
          printf ("\nDeseja continuar ? (s/n):");
          op = getche();
      }
      system("PAUSE");
} 

numero par ou impar.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   int a;
   
   printf("Declare o número: ");
   scanf ("%d", &a);
   
   if (a % 2 == 0){
   printf ("O número é par\n");       
   } else {
   printf("O número é ímpar\n");
   }
   
   system("PAUSE");
}

numeros inteiros até numero usuario.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()

{       
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int n, dobro, i ;
   printf ("Digite um número: ");
   scanf ("%d", &n);
   dobro = n+n;
   for (i = 1 ; i <= 5 ; i = i+1) 
   {
       printf ("Dobro do número: %d\n", dobro);
       _sleep(100);
   }    
   system("PAUSE");
}

numeros naturais while.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int i = 1,num;
      printf("Digite um numero maior que 1: ");  
      scanf("%d",&num);
      while( i <= num )
      {    
          printf("Numero = %d\n",i);
          i = i + 1;  
          _sleep(30);
      }  
      system("PAUSE");
} 

preco carro.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   char automovel[30];
   float fabrica, venda, impostos, revendedor; 
   
   printf ("Digite o nome do automóvel: ");
   scanf("%s",&automovel);
   
   printf ("Digite o preço de fábrica: ");
   scanf ("%f",&fabrica);
   
   impostos = fabrica * 0.45;
   revendedor = (fabrica + impostos) *0.28;
   venda = fabrica + impostos + revendedor;
   
   printf ("Automóvel: %s\n\n",automovel);

   printf ("Valor de venda: %.2f\n\n",venda);
   
   
   
  
   system("PAUSE");
}

quadrado 15 a 200.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()

{       
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int n, res ;
   
   for ( n = 15 ; n <= 200 ; n = n+1)
   {
    res = n*n;    
    printf ("\n\nQuadrado: %d", res);
    _sleep(300);
   }    
   system("PAUSE");
}
 
quadrado numeros inteiros 15 a 200 for.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int quad=0, i=15;
      printf("\nQuadrado dos numeros inteiros de 15 a 200\n\n\n");
      while( i <= 200 )
      {  
          quad = i*i;
          printf ("\nQuadrado = %d",quad);
          i = i + 1;      
          _sleep (0);
           
      }  
      
      system("PAUSE");
} 

quadrado numeros inteiros 15 a 200 while.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int quad=0, i=15;
      printf("\nQuadrado dos numeros inteiros de 15 a 200\n\n\n");
      while( i <= 200 )
      {  
          quad = i*i;
          printf ("\nQuadrado = %d",quad);
          i = i + 1;      
          _sleep (0);
           
      }  
      
      system("PAUSE");
} 

real e dollar.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   float real, dollar, taxa; 
   
   printf ("Digite o valor em Reais: ");
   scanf ("%f",&real);
   
   printf ("Digite o valor da taxa de conversão: ");
   scanf ("%f",&taxa);
   
   dollar = real * taxa;
   
   printf ("Valor em Dollar= %.2f\n",dollar);
   
     

 
   system("PAUSE");
}

resultados tabuada.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()

{       
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int n, res, i ;
   printf ("Digite um número: ");
   scanf ("%d", &n);
   for (i = 1 ; i <= 10 ; i = i+1)
   {
       res = n*i;    
       printf ("%3d x %3d = %3d\n", n, i, res);
       _sleep(100);
   }    
   system("PAUSE");
}
 
salario liquido professor.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 8E");
   
   float hraula, naulas, inss, salbruto, salliquido;
   
   printf("Declare o valor da hora aula: ");
   scanf ("%f", &hraula);
   
   printf("Declare a quantidade de aulas mensais: ");
   scanf ("%f", &naulas);
   
   printf("Declare o desconto do INSS: ");
   scanf ("%f", &inss);
   
   salbruto   = hraula * naulas;   
   salliquido = salbruto - inss;
   
   printf ("Salário Líquido: %.2f\n", salliquido);
   
   
   
   system("PAUSE");
}

soma dos numeros pares de 0 a 500.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()

{       
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int s=0, num ;
   printf ("Números pares de 1 até 500: \n\n");
   
   for (num = 0 ;  num <= 500 ; num = num+2)
   {        
       printf ("Número par = %d\n", num);  
       s = s + num;          
   }        
       
       printf ("\nA soma dos números pares é: %d\n\n", s);
       
   system("PAUSE");
}
 
soma numeros pares 0 a 500 while.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int s=0,num=0;
      printf("\nSoma dos numeros pares de 0 ate 500\n\n\n");
      while( num <= 500 )
      {    
          printf("Numero par = %d\n",num);  
          s = s + num;
          num += 2;
          _sleep (0);
           
      }  
      printf("\n\nSoma = %d\n\n\n",s);  
      system("PAUSE");
} 

tabuada while.cpp

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

main()  
{
      int i=1,num,res=0;
      printf("Digite um numero para calcular a tabuada: ");  
      scanf("%d",&num);
      while( i <= 10 )
      {    
          res = i * num;
          printf("%2d x %2d = %2d\n",num,i,res);
          i = i + 1;  
      }  
      system("PAUSE");
} 

vetores 1.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int i,n;
   printf ("\nDigite o tamanho do vetor: ");
   scanf ("%d",&n);
   int vet [n];
   
   printf ("\nEntre com os %d números: ",n);
   for (  i=0 ; i<n ; i++ )
   {
       scanf ("%d",&vet[i]);    
   }   
   printf ("\nOs numeros do vetor sao: \n");
   for (  i=0 ; i<n ; i++ )
   {
       printf("%d\n",vet[i]);
   }
           
   system("PAUSE");
}

vetores 2.cpp

#include<stdio.h>  
#include<stdlib.h> 
#include<locale.h> 
#include<conio.h>
#include<math.h>

main()
{  
      
   setlocale(LC_ALL,"Portuguese");
   system("color 1E");
   
   int i,n, menor, maior;
   printf ("\nDigite o tamanho do vetor: ");
   scanf ("%d",&n);
   int vet [n];
   printf ("\nEntre com os %d números: ",n);
   for (  i=0 ; i<n ; i++ )
   
   {
       scanf ("%d",&vet[i]);
   }
   menor = vet [0];
   maior = vet [0];
   
   for (  i=0 ; i<n ; i++ )
   {
       if (vet[i] < menor)
          menor = vet[i];
       if (vet[i] > maior)
          maior = vet[i];
       
   }   
  
   printf("Maior = %d\n",maior);
   printf("Menor = %d\n",menor);
           
   system("PAUSE");
}


