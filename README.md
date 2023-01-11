# CS101_ForLoops
```cs
// for(ifade1;kosul;ifade2)
// {
//     komut1;
//     komut2;
// }
using System.Text;

Console.Write("bir sayı giriniz");
int sayac=int.Parse(Console.ReadLine());
//ekranda girilen sayıya kadar  olan tek sayıları yazdır.
for (var i = 1; i <= sayac; i++) //döngüyü 0'dan başlat her seferinde 1 artır ve length eşit olana kadar devam ettir

{
    if(i%2==1)
    Console.WriteLine(i); 
    //komutlar
}

//1 ile 1000 arasaındaki tek ve çift sayıların toplamını yazdırın

int tekToplam=0;
int ciftToplam=0;

for (var i = 1; i <=1000; i++)
{
    if(i%2==1)
    tekToplam+=i;
    else
    ciftToplam+=i;

}

Console.WriteLine("tek sayıları toplamı:"+tekToplam); 
Console.WriteLine("çift sayıları toplamı:"+ciftToplam); 


//break ve continue   
//for döngüsünde bir yerde  çıkmak istitorsanız break kullanılır
//continue ise bir şart bağl olarak o kod bloğunu atlamak istiyorsak continue kullannırız

Console.WriteLine("break kulalnıdığında");
for (var i = 1; i <= 10; i++) // for  döndüsünde break ile sayı 4 olduğunda döngü sonlacaktır.
{
    if (i==4)
    break;
    Console.WriteLine(i);
}

Console.WriteLine("continue kulalnıdığında");
for (var i = 1; i <= 10; i++) // for döngüsünde continue ile sayı 4 olduğunda o sayıyı atlayarak döngü devam eder
{
    if (i==4)
    continue;
    Console.WriteLine(i);
}

//Day 5: Loops - HackerRank
int n = Convert.ToInt32(Console.ReadLine().Trim());
for (var i = 1; i <= 10; i++) // for  döndüsünde break ile sayı 4 olduğunda döngü sonlacaktır.
{
    Console.WriteLine(n+" x "+i+" = "+n*i);
}


//Staircase - HackerRank

class Result
{
  static void staircase(int n) {
        for(int i = 1; i <= n; i++)
        {
            StringBuilder a = new StringBuilder(String.Empty);

            a.Append(' ', n - i);
            a.Append('#', i);

            Console.WriteLine(a);
        }
    }
    
        static void Main(string[] args) {
        int n = Convert.ToInt32(Console.ReadLine());

        staircase(n);
    }
}
```
