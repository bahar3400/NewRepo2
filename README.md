using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // ortaöğretim çalışma sitesi yap mesala matamatik bölümünde kullanıcı iki sayı aktar toplamını iste sonucu doğru ise 5 puan kazansın değilse  2 puan insin
            // sözel kısım string kelimler birleştirme veya harflar bu puan kısmı burada da geçerli olsun kullanıcı  harflar atansın ve o harflerle kelieme yapsın 


            Console.WriteLine("Oyunumuza Hoşgeldiniz....");
            Console.WriteLine("--------------------------------------------------------------------------------------------------------------------------");

            int seçim = 1;
            int seçim2 = 2;

            Console.WriteLine("Matamatik mi çalışmak isterseniz=1\nTürkçe çalışmak isterseniz=2 Basabilirsiniz ");
            int giriş1 = Convert.ToInt32(Console.ReadLine());


            if (giriş1 == seçim)
            {
                int toplama = 1;
                int çıkarma = 2;
                int çarpma = 3;
                int bölme = 4;

                Console.WriteLine("Toplama yapmak istersiniz 1\nÇıkarma yapmak istersiniz 2\nÇarpma yapmak isterseniz 3\nBölme yapmak isterseniz 4 basınız....  ");
                int giriş2 = Convert.ToInt32(Console.ReadLine());


                if (giriş2 == 1)
                {

                    Random rastgele1 = new Random();
                    int sayi1 = rastgele1.Next(0, 501);
                    int sayi2 = rastgele1.Next(0, 501);

                    Console.WriteLine("Sayıları topla:  " + sayi1 + " + " + sayi2);
                    Console.WriteLine("Sonucu giriniz: ");
                    int sonuc = Convert.ToInt32(Console.ReadLine());
                    int işlem1 = sayi1 + sayi2;
                    if (işlem1 == sonuc)
                    {
                        Console.WriteLine("Doğru Tebrikler");
                    }
                    else
                    {
                        Console.WriteLine("Üzgünüm Yanlış Girdiniz....");
                    }

                }
                else if (giriş2 == 2)
                {

                    Random rastgele2 = new Random();
                    int sayi3 = rastgele2.Next(0, 501);
                    int sayi4 = rastgele2.Next(0, 501);

                    Console.WriteLine("Sayıları çıkar :  " + sayi3 + " - " + sayi4);
                    Console.WriteLine("Sonucu giriniz: ");
                    int sonuc2 = Convert.ToInt32(Console.ReadLine());
                    int işlem2 = sayi3 - sayi4;
                    if (işlem2 == sonuc2)
                    {
                        Console.WriteLine("Doğru Tebrikler");
                    }
                    else
                    {
                        Console.WriteLine("Üzgünüm Yanlış Girdiniz....");
                    }

                }
                else if (giriş2 == 3)
                {
                    Random rastgele1 = new Random();
                    int sayi1 = rastgele1.Next(0, 501);
                    int sayi2 = rastgele1.Next(0, 501);

                    Console.WriteLine("Sayıları Çarp:  " + sayi1 + " * " + sayi2);
                    Console.WriteLine("Sonucu giriniz: ");
                    int sonuc = Convert.ToInt32(Console.ReadLine());
                    int işlem1 = sayi1 * sayi2;
                    if (işlem1 == sonuc)
                    {
                        Console.WriteLine("Doğru Tebrikler");
                    }
                    else
                    {
                        Console.WriteLine("Üzgünüm Yanlış Girdiniz....");
                    }

                }

                else if (giriş2 == 4)
                {
                    Random rastgele1 = new Random();
                    int sayi1 = rastgele1.Next(0, 501);
                    int sayi2 = rastgele1.Next(0, 501);

                    Console.WriteLine("Sayıları Bölme :  " + sayi1 + " / " + sayi2);
                    Console.WriteLine("Sonucu giriniz: ");
                    int sonuc = Convert.ToInt32(Console.ReadLine());
                    int işlem1 = sayi1 / sayi2;
                    if (işlem1 == sonuc)
                    {
                        Console.WriteLine("Doğru Tebrikler");
                    }
                    else
                    {
                        Console.WriteLine("Üzgünüm Yanlış Girdiniz....");
                    }
                }
                else
                {
                    Console.WriteLine("Yanlış sayı girdiniz çıkış yapıldı");
                    Environment.Exit(0);
                }

            }
            else if (giriş1 == seçim2)
            {

                Random rastgele = new Random();
                char harf = (char)rastgele.Next('a', 'z' + 1);
                char harf1 = (char)rastgele.Next('a', 'z' + 1);
                char harf2 = (char)rastgele.Next('a', 'z' + 1);
                char harf3 = (char)rastgele.Next('a', 'z' + 1);
                char harf4 = (char)rastgele.Next('a', 'z' + 1);
                char harf5 = (char)rastgele.Next('a', 'z' + 1);
                char harf6 = (char)rastgele.Next('a', 'z' + 1);


                Console.WriteLine("Karşınıza çıkan harflerle bir kelime oluşturunuz = " + harf+" "+ harf1+ " "+harf2+" "+ harf3+" "+harf4+" "+harf5+" "+harf6 );
                String kelime = Console.ReadLine();

            }
            else
            {
                Console.WriteLine("Yanlış sayı girdiniz çıkış yapıldı");
                Environment.Exit(0);

            }




















        }
    }
}
