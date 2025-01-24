using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace bankproje
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("*****************BAHAR BANK*******************");

             Console.WriteLine("///LOGİN PAGE///");


            string name = null, password = null;

            Console.WriteLine("İsim : ");
            name = Console.ReadLine();

            if (name != "")
            {
                Console.WriteLine("Şifre: ");
                password =Console.ReadLine();
            }

            if (name == "Bahar" && password == "ekinci")
            {
                int mainvote = -1;
                do
                {
                    Console.WriteLine("\n:::Ana Menü:::");
                    Console.WriteLine("1-Müşteri");
                    Console.WriteLine("2-Hesap");
                    Console.WriteLine("3-Fon Transferi");
                    Console.WriteLine("4-Fon Transfer Raporu");
                    Console.WriteLine("5-Hesap Raporu ");
                    Console.WriteLine("0-Exit");

                    Console.WriteLine("Seçiniz:  ");
                    mainvote = Convert.ToInt32(Console.ReadLine());

                    switch (mainvote)
                    {
                        case 1:müşteri();
                            break;

                        case 2:hesap();
                            break;

                        case 3:fon();
                            break;

                        case 4:fonrapor();
                            break;

                        case 5:hesaprapor();
                            break;


                    }
                } while (mainvote != 0);


            }
            else
            {
                Console.WriteLine("Kullanıcı ismi ve şifre Yanlış.");
            }

            Console.WriteLine(" Teşekkür ederiz Tekrar bekleriz...");
            Console.ReadKey();
        }


        public static void müşteri() 
        {
            int secim2 = -1;
            do
            {
                Console.WriteLine(":::\nMüşteri Menüsü:::");
                Console.WriteLine("1-Müşteri ekle");
                Console.WriteLine("2-Müşteri sil");
                Console.WriteLine("3-Müşteri güncelle");
                Console.WriteLine("4-Müşteri görüntüle");
                Console.WriteLine("0-Ana menüye geri dön");


                Console.WriteLine("İşleminizi seçiniz: ");
                secim2 = Convert.ToInt32(Console.ReadLine());


            } while (secim2 != 0);


        }


        public static void hesap()
        {
            int secim3 = -1;
            do
            {
                Console.WriteLine(":::\nHesap Menüsü:::");
                Console.WriteLine("1-Hesap ekle");
                Console.WriteLine("2-Hesap sil");
                Console.WriteLine("3-Hesap güncelle");
                Console.WriteLine("4-Hesap görüntüle");
                Console.WriteLine("0-Ana menüye geri dön");


                Console.WriteLine("İşleminizi seçiniz: ");
                secim3 = Convert.ToInt32(Console.ReadLine());


            } while (secim3 != 0);

        }


        public static void fon()
        {
            int secim4 = -1;
            do
            {
                Console.WriteLine(":::\nFon Menüsü:::");
                Console.WriteLine("1-Fon ekle");
                Console.WriteLine("2-Fon sil");
                Console.WriteLine("3-Fon Gönder");
                Console.WriteLine("4-Fon görüntüle");
                Console.WriteLine("0-Ana menüye geri dön");


                Console.WriteLine("İşleminizi seçiniz: ");
                secim4 = Convert.ToInt32(Console.ReadLine());


            } while (secim4 != 0);
        }




            public static void fonrapor()
        {
            int secim5 = -1;
            do
            {
                Console.WriteLine(":::\nFon Raporlama Menüsü:::");//Raporlama dediğim kısım kime gitmiş kimden gitmiş gibisinden işlem yapıcam.
                Console.WriteLine("1-Fonu Raporla");
                Console.WriteLine("0-Ana menüye geri dön");


                Console.WriteLine("İşleminizi seçiniz: ");
                secim5 = Convert.ToInt32(Console.ReadLine());


            } while (secim5 != 0);


        }



        public static void hesaprapor()
        {
            int secim6 = -1;
            do
            {
                Console.WriteLine(":::\nHesap Raporlama Menüsü:::");
                Console.WriteLine("1-Hesap Raporla");
                Console.WriteLine("0-Ana menüye geri dön");


                Console.WriteLine("İşleminizi seçiniz: ");
                secim6= Convert.ToInt32(Console.ReadLine());


            } while (secim6 != 0);


        }
