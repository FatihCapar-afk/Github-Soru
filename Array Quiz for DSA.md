Soru 1 (Bilgisayar mimarisinde diziler bellekte blok halinde tutulduğu için işlemci önbelleğine (CPU cache) kolayca alınır ve indeks numarasıyla istenen elemana anında, yani O(1) hızında erişilebilir.)
Dizilerin (arrays) avantajlarını hangi seçenek doğru tanımlar?

Cevap: Bellekte ardışık (contiguous) yer ayrıldığı için rastgele erişime (random access) ve önbellek (cache) dostu bir yapıya izin vermesidir.
----------------------------------------------------------------------------------------
Soru 2 (İlk eleman bellek bloğunun tam başlangıç adresindedir (offset = 0))
Bir dizinin ilk indeksi (indekslemesi) genellikle hangisinden başlar?

Cevap: 0
----------------------------------------------------------------------------------------
Soru 3 ("Rastgele erişim", dizideki herhangi bir elemana, önceki elemanları tek tek taramak zorunda kalmadan, doğrudan matematiksel adresi üzerinden anında ulaşabilme yeteneğidir.)
Bir dizideki elemanlara erişmek için hangi yöntem kullanılır?

Cevap: Rastgele Erişim (Random Access)
----------------------------------------------------------------------------------------
Soru 4 (Dizinin donanımsal temel özelliği budur. RAM üzerinde elemanlar yan yana dizilir; böylece işletim sistemi bir sonraki veriyi nerede bulacağını kolayca hesaplar.)
Diziler bellekte nasıl saklanır?

Cevap: Tüm elemanlar bellekte ardışık (bitişik) bir blokta saklanır.
----------------------------------------------------------------------------------------
Soru 5 (Statik dizilerin boyutu kod yazılırken veya derlenirken belirlenir (Örn: 100 elemanlık dizi). Sadece 10 eleman kullanırsan, kalan 90 elemanlık yer bellekte boşuna kilitlenmiş olur.)
Statik dizilerin dezavantajı nedir?

Cevap: Diziye eklenen eleman sayısı, ayrılan kapasiteden azsa bellek (RAM) alanının israf edilme ihtimali vardır.
----------------------------------------------------------------------------------------
Soru 6 (Dinamik diziler büyüyebilme özelliğine sahip olsalar da arka planda standart diziler kullanırlar. Yer bittiğinde, bellekte daha büyük, yeni bir "bitişik" alan bulup verileri oraya taşırlar.)
Dinamik bir dizinin elemanları bellekte nasıl saklanır?

Cevap: Her bir eleman bellekte yine ardışık (bitişik) konumlarda saklanır.
----------------------------------------------------------------------------------------
Soru 7 (Bilgisayar bilimlerinde "declare", işletim sisteminden "bana şu kadar yer ayır" demektir. "Initialize" ise ayrılan o boş alana ilk gerçek verileri yerleştirmektir.)
Bir diziyi bildirmek (declare) ile başlatmak (initialize) arasındaki fark nedir?

Cevap: Bildirim (declaration) dizinin boyutunu ve veri tipini belirler; başlatma (initialization) ise diziye ilk değerlerini atar.
----------------------------------------------------------------------------------------
Soru 8 (Matematikteki matris yapısının kodlamadaki karşılığıdır. Veriler excel tablosu gibi dikey ve yatay düzlemde organize edilir.)
İki boyutlu (2D) dizi nedir?

Cevap: Satır ve sütunlardan oluşan bir matris veya dizilerin dizisidir (array of arrays).
Soru 9 (Standart programlama notasyonunda ilk köşeli parantez [i] satır indeksini (yatay eksen), ikinci köşeli parantez [j] ise sütun indeksini (dikey eksen) temsil eder.)
İki boyutlu (2D) bir dizideki elemanlara nasıl erişilir?

Cevap: dizi[i][j]
----------------------------------------------------------------------------------------
Soru 10 (Dizinin 0. indeksine yeni bir eleman koyduğunda, sağdaki diğer tüm elemanların birer sıra sağa kaydırılması (shift) gerekir. N adet eleman varsa N adet kaydırma işlemi yapılır.)
Bir dizinin en başına eleman eklemenin veya silmenin zaman karmaşıklığı nedir?

Cevap: O(N)
----------------------------------------------------------------------------------------
Soru 11 (Sadece 51 ile 100 arasındaki notlarla ilgilendiğimiz için (yaklaşık 50 farklı not türü), koca bir dizi açmak yerine, sadece bu notların sayısını tutacak spesifik boyutta küçük bir dizi açmak bellek optimizasyonudur.)
Bir P programı, [0..100] aralığında notlar alan 500 öğrencinin notlarını okuyor ve 50'den büyük notların frekansını (kaç kere alındığını) yazdırıyor. P'nin bu frekansları saklaması için en iyi yol nedir?

Cevap: 50 sayılık (veya duruma göre 51) bir dizi kullanmak.
----------------------------------------------------------------------------------------
Soru 12 (Alt diziler orijinal dizide yan yana duran (ardışık) elemanlardan oluşmak zorundadır. Matematiksel olarak ardışık kombinasyonların toplamı n + (n-1) + ... + 1 formülünden n(n+1)/2 çıkar.)
n elemanlı bir dizi için kaç farklı alt dizi (subarray) oluşturulabilir?

Cevap: n(n+1)/2
----------------------------------------------------------------------------------------
Soru 13 (Alt dizilimlerde (subsequence) elemanların yan yana olma zorunluluğu yoktur. Dizideki her eleman ya bu dizilime katılır (1) ya da katılmaz (0). Toplam n eleman için 2 * 2 * ... = 2^n ihtimal vardır.)
n elemanlı bir dizi için oluşturulabilecek olası alt dizilim (subsequence) sayısı nedir?

Cevap: 2^n
----------------------------------------------------------------------------------------
Soru 14 ("Subarray" (alt dizi) kuralına göre elemanlar kesintisiz ve sırasıyla alınmalıdır. Örneğin {1, 3} bir alt dizi olamaz çünkü arada 2 atlanmıştır.)
arr[] = {1, 2, 3} dizisinden oluşturulabilecek tüm alt diziler (subarrays) hangileridir?

Cevap: {1}, {2}, {3}, {1, 2}, {2, 3}, {1, 2, 3}
----------------------------------------------------------------------------------------
Soru 15 (Dizilerin ilk elemanı 0. indeksten başladığı için, 10 elemanlı bir dizinin son elemanı 9. indekstedir. Bu yüzden döngü hep "uzunluk - 1" noktasına kadar çalışmalıdır, aksi halde kod çökebilir (Out of Bounds hatası).)
Bir dizideki tüm elemanları sırayla gezmek (iterate) için hangi döngü yapısını kullanırsınız?

Cevap: for i = 0 to (dizinin uzunluğu - 1)
----------------------------------------------------------------------------------------
Soru 16 (0. indeks 5'tir, 1. indeks 8'dir. Kod bu ikisini çarpıyor (5 * 8 = 40) ve sonucu 2. indeksteki elemanın (orijinali 3 olan sayının) yerine yazıyor.)
Aşağıdaki kod çalıştıktan sonra arr[2]'nin son değeri ne olur?
arr[] = {5, 8, 3, 7};
arr[2] = arr[1] * arr[0];

Cevap: 40
----------------------------------------------------------------------------------------
Soru 17 (Dizi halihazırda 5 elemanlıdır. İkinci satırda yapılan işlem sadece 3. indekste bulunan veriyi (4'ü) silip yerine 10 yazmaktır. Diziye yeni bir kapasite veya alan eklenmemiştir.)
Bu işlemden sonra arr dizisinin uzunluğu (eleman sayısı) nedir?
arr[] = {1, 2, 3, 4, 5};
arr[3] = 10;

Cevap: 5
----------------------------------------------------------------------------------------
Soru 18 (Dışarıdaki i döngüsü satırları (0 ve 1. satır), içerideki j döngüsü sütunları (0, 1, 2. sütun) gezer. Bu iç içe döngü mantığı matrisi tıpkı bir kitabı okur gibi soldan sağa, yukarıdan aşağıya yazar.)
Aşağıdaki iki boyutlu dizi kod parçasının (yazım hataları giderilmiş halinin) çıktısı nedir?
arr[2][3] = {{1, 2, 3}, {4, 5, 6}};
for (i = 0 To 1) {
for (j = 0 To 2) { print(arr[i][j]); }
}

Cevap: 1 2 3 4 5 6
----------------------------------------------------------------------------------------
Soru 19 (Programlamada klasik veri değiştirme (swap) yöntemidir. "temp" (geçici) değişkeni sayesinde dizinin ilk elemanı olan 1 ile son elemanı olan 4 kendi aralarında yer değiştirilmiştir.)
Aşağıdaki kod çalıştıktan sonra dizinin elemanları nasıl olur?
arr[] = {1, 2, 3, 4};
temp = arr[0];
arr[0] = arr[3];
arr[3] = temp;

Cevap: {4, 2, 3, 1}
----------------------------------------------------------------------------------------
Soru 20 ("İki Gösterici" (Two-pointer) tekniğiyle, bir işaretçi dizinin başından, diğeri sonundan başlayarak ortada buluşana kadar elemanları yer değiştirir. Dizinin üzerinden sadece bir kere tam olarak geçileceği için işlem O(N) lineer sürede biter.)
Negatif ve pozitif sayılardan oluşan bir diziyi, tüm pozitifler bir tarafta ve negatifler diğer tarafta olacak şekilde ayırmak için (örneğin sol tarafa pozitifler, sağ tarafa negatifler) en kötü durumda (worst-case) zaman karmaşıklığı nedir?

Cevap: O(N)