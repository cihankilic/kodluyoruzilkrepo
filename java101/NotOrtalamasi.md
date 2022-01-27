# Not Ortalaması Hesaplayan Program
``` java
import java.util.Scanner;

public class NotOrtalamasi {

    public static void main(String[] args) {
	/* Bu projede kullanıcının not girişini yaptığı 6 dersin
	   not ortalaması bulunduktan sonra kullanıcının geçme
	   durumu terminale yazdırılmaktadır.
	 */
        int mat, fizik,kimya, turkce, tarih, muzik;

        Scanner imp = new Scanner(System.in);

        System.out.print("Matematik ders notu: ");
        mat = imp.nextInt();

        System.out.print("Fizik ders notu: ");
        fizik = imp.nextInt();

        System.out.print("Kimya ders notu: ");
        kimya = imp.nextInt();

        System.out.print("Türkçe ders notu: ");
        turkce = imp.nextInt();

        System.out.print("Tarih ders notu: ");
        tarih = imp.nextInt();
        
        System.out.print("Müzik ders notu: ");
        muzik = imp.nextInt();

        int toplam = mat + fizik + kimya + turkce + tarih + muzik;

        double sonuc = toplam / 6.0;

        System.out.println("Ortalama Sonucu : "+ sonuc);

        int gecti = (sonuc < 60)  ? 0:1;

        switch (gecti){
            case 0:
                System.out.println("Sınıfta Kaldı");
                return;

            case 1:
                System.out.println("Sınıfı Geçti");
                return;
        }

    }
}
```
