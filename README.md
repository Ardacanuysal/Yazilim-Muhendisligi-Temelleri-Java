# -dev
youtube linki: https://www.youtube.com/watch?v=-0Tcie2iFaU
//Yazilim Muhendisligi dersi final projesi anlatım videosu yukarıdaki youtube linkinde


 kodlar:
 package sayitahmini;

import java.util.Scanner;

public class Sayitahmini {

    public static void main(String[] args) {

        //0-100 arası  sayı tahmini yapar yakınlık uzaklıgına gore yorum yapar
        
        int sayi = (int) (Math.random() * 101);

        Scanner giris = new Scanner(System.in);
        int tahmin = -1;//0 dan başlar

        System.out.println("0-100 arası say giriniz");

        while (tahmin != sayi) {
            System.out.println("tahmin ediniz");
            tahmin=giris.nextInt();
            
            if(tahmin==sayi){
                System.out.println("doğru bildinizz");
            }
            else if(tahmin<sayi){
                System.out.println("tahmininiz dusuk");
            }
            else if (tahmin>sayi){
                System.out.println("tagmininiz yuksek");
            }
        }

    }

}
----------------------------------------------------------------------------
package sayiverigirisi;

import java.util.Scanner;

public class Sayiverigirisi {

    public static void main(String[] args) {

        //girilen sayıların toplamını yapar 0 girilince işlemi sonllandırır
        
        Scanner giris = new Scanner(System.in);

        System.out.println("bir tam sayi giriniz" + "(işlemi sonlandırmak için 0'a basınız.)");
        int veri = giris.nextInt();

        int toplam = 0;
        while (veri != 0) {
            toplam += veri;
            System.out.println("bir tam sayi giriniz" + "(işlemi sonlandırmak için 0'a basınız.)");
            veri = giris.nextInt();
        }
        System.out.println("toplam:"+toplam);
    }

----------------------------------------------------------------------------------
package odev1;

import java.util.Scanner;

public class Odev1 {

    public static void main(String[] args) {

        //bir ucretlının sıcıl numarası calısma saatı ve saatlık ucretı bılgısayara gırıs olarak veriliyor ucretlının bu bılgılerle maasını hesaplayan algorıtmanın java kodu:
        
        Scanner KLAVYE = new Scanner(System.in);

        System.out.println("sicil no gırınız");
        String Scilno = KLAVYE.nextLine();
        System.out.println("calısma saatı gırınız");
        int calismasaati = KLAVYE.nextInt();
        System.out.println("saatlık ucret giriniz");
        int saaatlikucret = KLAVYE.nextInt();
        int maas;
        maas = saaatlikucret * calismasaati;
        System.out.println("maas:" + maas);

    }

}
--------------------------------------------------------------------------------------
package plakka22;
import java.util.Scanner;
public class Plakka22 {

    public static void main(String[] args) {
    
        //8 karakterli girilen plakanın hangi ile ait olduğunu tespit eder
        
    Scanner klavye = new Scanner(System.in);
        System.out.println("Plakanızın Tamamını Arada Hiç Boşluk Bırakmadan Giriniz:");//boluklar bıle karakterdir
        String plaka = klavye.next();
        int alankodu = Integer.parseInt(plaka.substring(0, 2));
        if (plaka.length() == 7) {
            String[] sehir = {"Adana", "Adıyaman", "Afyonkarahisar", "Ağrı", "Amasya", "Ankara", "Antalya", "Artvin", "Aydın", "Balıkesir", "Bilecik", "Bingöl", "Bitlis", "Bolu", "Burdur", "Bursa", "Çanakkale", "Çankırı", "Çorum", "Denizli", "Diyarbakır", "Edirne", "Elazığ", "Erzincan", "Erzurum", "Eskişehir", "Gaziantep", "Giresun", "Gümüşhane", "Hakkari", "Hatay", "Isparta", "Mersin", "İstanbul", "İzmir", "Kars", "Kastamonu", "Kayseri", "Kırklareli", "Kırşehir", "Kocaeli", "Konya", "Kütahya", "Malatya", "Manisa", "Kahramanmaraş", "Mardin", "Muğla", "Muş", "Nevşehir", "Niğde", "Ordu", "Rize", "Sakarya", "Samsun", "Siirt", "Sinop", "Sivas", "Tekirdağ", "Tokat", "Trabzon", "Tunceli", "Şanlıurfa", "Uşak", "Van", "Yozgat", "Zonguldak", "Aksaray", "Bayburt", "Karaman", "Kırıkkale", "Batman", "Şırnak", "Bartın", "Ardahan", "Iğdır", "Yalova", "Karabük", "Kilis", "Osmaniye", "Düzce"};
            System.out.println(sehir[alankodu - 1] + "---> İline Ait Plaka:)");
        } else if (plaka.length() == 8) {
            String[] sehir = {"Adana", "Adıyaman", "çobanla", "Ağrı", "Amasya", "Ankara", "Antalya", "Artvin", "Aydın", "Balıkesir", "Bilecik", "Bingöl", "Bitlis", "Bolu", "Burdur", "Bursa", "Çanakkale", "Çankırı", "Çorum", "Denizli", "Diyarbakır", "Edirne", "Elazığ", "Erzincan", "Erzurum", "Eskişehir", "Gaziantep", "Giresun", "Gümüşhane", "Hakkari", "Hatay", "Isparta", "Mersin", "İstanbul", "İzmir", "Kars", "Kastamonu", "Kayseri", "Kırklareli", "Kırşehir", "Kocaeli", "Konya", "Kütahya", "Malatya", "Manisa", "Kahramanmaraş", "Mardin", "Muğla", "Muş", "Nevşehir", "Niğde", "Ordu", "Rize", "Sakarya", "Samsun", "Siirt", "Sinop", "Sivas", "Tekirdağ", "Tokat", "Trabzon", "Tunceli", "Şanlıurfa", "Uşak", "Van", "Yozgat", "Zonguldak", "Aksaray", "Bayburt", "Karaman", "Kırıkkale", "Batman", "Şırnak", "Bartın", "Ardahan", "Iğdır", "Yalova", "Karabük", "Kilis", "Osmaniye", "Düzce"};
            System.out.println(sehir[alankodu - 1] + "---> İline Ait Plaka:)");
        
        
        } else {
            System.out.println("Yanlış Bir Plaka Tuşladınız Kontrol Edip Tekrar Deneyiniz.");
        }
 

    
    }

}
-----------------------------------------------------------------------------------------------
package isimsoyisimistemeyamanakbulut;

import java.util.Scanner;

public class Isimsoyisimistemeyamanakbulut {

    public static void main(String[] args) {

        int sonuc = (int) (Math.random() * 4);//random işlem attırır

        int sayi1 = (int) (Math.random() * 10);
        int sayi2 = (int) (Math.random() * 10);

        //

        /*
        System.out.println("toplama için1");
        System.out.println("çıkartma için 2");
        System.out.println("çarpma için 3");
        System.out.println("bolme için 4");
        Scanner klavye = new Scanner(System.in);
        int sonuc = klavye.nextInt();
         */
        
        if (sonuc == 1) {
            Scanner giris = new Scanner(System.in);
            System.out.print(sayi1 + "+" + sayi2 + " sonuc nedir?");
            int cevap = giris.nextInt();

            while (sayi1 + sayi2 != cevap) {
                System.out.println("yanlis cevap tekrar deneyiniz");
            }
            cevap = giris.nextInt();
        } 
        else if (sonuc == 2) {
            Scanner giris = new Scanner(System.in);
            System.out.println(sayi1 + "-" + sayi2 + "sonuc nedir?");
            int cevap = giris.nextInt();

            while (sayi1 - sayi2 != cevap) {
                System.out.println("yanlis cevap tekrar deneyiniz");
            }
            System.out.println("bildiniz tebrikler");
        } 
        else if (sonuc == 3) {
            Scanner giris = new Scanner(System.in);
            System.out.println(sayi1 + "x" + sayi2 + "sonucu nedir?");
            int cevap = giris.nextInt();
            while (sayi1 * sayi2 != cevap) {
                System.out.println("yanlis cevap tekrar deneyiniz");
            }
            System.out.println("bildiniz tebrikler");
        } else if (sonuc == 4) {
            Scanner giris = new Scanner(System.in);
            System.out.println(sayi1 + "/" + sayi2 + "sonuc nedir?");
            int cevap = giris.nextInt();
            while (sayi1 / sayi2 != cevap) {
                System.out.println("yanlis cevap tekrar deneyiniz");
            }
            System.out.println("bildiniz tebrikler");
        }
    }

}
---------------------------------------------------------------------------------
package pkg10luktabandan82tabana;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        //disaridan gırıs 10 tabandakı bır  sayı degişkeni için eger girilen deger cift ise 8 tabanına donusturen,cift değilse 2 tabanına donusturen programın java kodu:
       
        Scanner klavye = new Scanner(System.in);
        System.out.println("lütfen bir tamsayı giriniz");

        int sayi = klavye.nextInt();
        if (sayi % 2 == 0) {
            String sonuc = "";
            while (sayi != 0) {
                int kalan = sayi % 8;
                sayi = sayi % 8;
                sonuc = kalan + sonuc;
            }
            System.out.println("gririlen sayının 8 tabanınfakı karsılıgı" + sonuc);
        } else {
            String sonuc = "";
            while (sayi != 0) {
                int kalan = sayi % 2;
                sonuc = kalan + sonuc;
            }
            System.out.println("girlşine sayının 2 tabanındaski karsılığı" + sonuc);
        }
    }

}
---------------------------------------------------------------------------------------------
package arcelikprojemakine;
import java.util.Scanner;
public class Arcelikprojemakine {
    public static void main(String[] args) {
    
        /*Bir fabrikada makinelerin çalışmaya başlama zamanları farklıdır. Fabrikanın çalışmaya başlama saati mevsime göre değişmektedir. Sonbahar ve Kış aylarında fabrika 08:00 de çalışmaya başlamaktadır. İlkbahar ve Yaz aylarında ise fabrikanın çalışmaya başlama saati 09:00 dır.
Fabrikanın paydos saati her mevsim 17:00 dır. Makineler Sonbahar ve Kış aylarında 30 dakika ara ile İlkbahar ve Yaz aylarında ise 45 dakika ara ile çalışmaya başlatılmaktadır.
Programa fabrikadaki makine sayısı ve hangi ayda olduğu (1 ile 12 arasında bir değer) bilgisi giriş olarak veriliyor.
Programın çıktısı olarak makinelerin sırasıyla toplam kaç dakika çalıştığı ekrana yazdırılmaktadır. Programın java kodunu yazınız.
*/
        
        Scanner klavye=new Scanner(System.in);
        System.out.println("Lütfen makina sayısını giriniz");
        int makinesayisi=klavye.nextInt();
        
        System.out.println("Lutfen hangi ayda olduğunu giriniz:");
        int ay=klavye.nextInt();
        int sure,aralık;
        if (ay>2&&ay<9){
            sure=480;
            aralık=45;}
        else {
            sure=540;//yaz ve ilk bahar
            aralık=30;}
        for(int i =makinesayisi;i>0;i--){
            System.out.println(sure+",");
            sure =sure-aralık;
        }
        
        }
                
    }


-----------------------------------------------------------------------------------------------------------------------
package ödev6;
import java.util.Scanner;
public class Ödev6 {

    public static void main(String[] args) {
    

// cınsıyet ve adım sayıasın baglı olarak  kalori hesabı yapmak

    
    Scanner klavye=new Scanner (System.in);
        System.out.println("Cinsiyet giriniz");
         String cinsiyet =klavye.nextLine();
         System.out.println("adım sayısını giriniz");
         int adimSayisi=klavye.nextInt();
         int kalori;
         if(cinsiyet.equals("kadin")){
         kalori=adimSayisi*30/500;
         }
         else{
             kalori=adimSayisi*45/500;
         }
          System.out.println("Yakılan kalori miktarı:"+kalori);


    }

}
------------------------------------------------------------------------------------------------

package faktöryelhesabı;

import java.util.Scanner;

public class FaktöryelHesabı {
  //faktöryel hesabında atanan 1 o sayının başlangıcını belirtmekte i++ 
    public static void main(String[] args) {
        
        Scanner klavye = new Scanner(System.in);
        int faktoryel =1;
        System.out.println("faktöryel hesaplanacak sayıyı giriniz");
        
        int sayi = klavye.nextInt();
        for (int i = 1; i <=sayi; i++){
            faktoryel= faktoryel * i;
        }
        System.out.println("işlemin sonucu---->>"+ faktoryel);
        
    }
    
}
---------------------------------------------------------------------------------------------------
package bamyaöddeviialgooymahyaman;

public class Bamyaöddeviialgooymahyaman {

    public static void main(String[] args) {
        // mesaj uzerinden baMya stringlerini cekiniz
        String mesaj = "Merhaba dünya";

        String mesaj1 = mesaj.substring(5, 7);//ba
        char mesaj2 = mesaj.charAt(0);//M
        String mesaj3 = mesaj.substring(11,13);//ya

        System.out.println(mesaj1 + mesaj2+ mesaj3);

    }

}
-----------------------------------------------------------------------------------------------------





