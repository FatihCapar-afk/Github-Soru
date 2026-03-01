Soru 1 (Döngü, left (0) ve right (4) değerleri merkezde buluşana kadar devam eder. arr[2] < arr[2] (3 < 3) koşulu sağlanmadığı an döngü durur ve her iki işaretçi de 2. indekste kalır.)
Çeviri: Yukarıdaki kod çalıştırıldıktan sonra left ve right işaretçilerinin konumu ne olur?
Cevap: A) 2, 2
----------------------------------------------------------------------------------------
Soru 2 (İç içe döngüler O(N^2) zaman alırken, iki işaretçi diziyi tek bir geçişte (O(N)) tarar.)
Çeviri: Sıralı dizilerde toplam çifti bulmak için "iki işaretçi" yöntemi neden iç içe döngülerden daha verimlidir?
Cevap: B) Each element is processed at most once (Her eleman en fazla bir kez işlenir)
----------------------------------------------------------------------------------------
Soru 3 (Baştaki ve sondaki karakterleri karşılıklı kontrol ederek merkeze ilerlemek en hızlı yoldur.)
Çeviri: "racecar" kelimesinin palindrom olup olmadığını verimli kontrol etmek için hangi teknik kullanılır?
Cevap: B) İki işaretçi kullanarak: Biri en soldan diğeri en sağdan başlayarak içeri doğru eşitlik kontrolü yapmak.
----------------------------------------------------------------------------------------
Soru 4 (Toplamı büyütmek için dizinin küçük tarafındaki (sol) işaretçiyi sağa, yani daha büyük değerlere doğru kaydırmalıyız.)
Çeviri: Sıralı bir dizide hedef toplam 12 ise ve mevcut iki işaretçinin toplamı 12'den küçükse ne yapılmalıdır?
Cevap: B) Move the left pointer rightward (Sol işaretçiyi sağa kaydır)
----------------------------------------------------------------------------------------
Soru 5 (Her iki dizinin en küçük elemanlarını kıyaslayarak adım adım ilerlemek verimli bir birleştirme sağlar.)
Çeviri: İki sıralı diziyi tek bir sıralı dizi olarak birleştirmek (merge) için iki işaretçi nasıl kullanılır?
Cevap: B) İki işaretçiyi de dizilerin başında başlat, elemanları karşılaştır, küçük olanı sonuca ekle ve ilgili işaretçiyi ilerlet.
----------------------------------------------------------------------------------------
Soru 6 (Bu "hızlı ve yavaş işaretçi" (Floyd’s Cycle-Finding varyasyonu) yöntemidir; hızlı olan iki adım atarken yavaş olan bir adım atar.)
Çeviri: Tekli bağlı listede (singly linked list) orta elemanı bulmak için iki işaretçi nasıl uygulanır?
Cevap: D) İkinci işaretçiyi birinciden iki kat hızlı hareket ettir. Hızlı olan sona ulaştığında, yavaş olan ortadadır.
----------------------------------------------------------------------------------------
Soru 7 (Karşılıklı karakterleri takas ederek kelimenin sonunu başına getiririz.)
Çeviri: "Pointer" kelimesini ters çevirmek için iki işaretçi nasıl kullanılır?
Cevap: A) Biri başta diğeri sonda iki işaretçi kullan ve merkezde buluşana kadar karakterlerin yerini değiştir (swap).
----------------------------------------------------------------------------------------
Soru 8 (Diziyi tek bir sefer tarayarak sayıları gruplayabildiğimiz için doğrusal zaman (O(N)) yeterlidir.)
Çeviri: Pozitif ve negatif sayıların olduğu bir dizide, aynı işaretli sayıları (bir tarafa + diğer tarafa -) ayırmak için iki işaretçi kullanıldığında en kötü durum zaman karmaşıklığı nedir?
Cevap: B) O(N)
----------------------------------------------------------------------------------------
Soru 9 (Bir elemanı sabitleyip kalan ikisini iki işaretçiyle aradığımız için O(N)*O(N) = O(N^2) olur.)
Çeviri: Toplamı sıfır olan üçlüleri (triplet) bulmak için iki işaretçi kullanan algoritmanın zaman karmaşıklığı nedir?
Cevap: D) O(n^2)
----------------------------------------------------------------------------------------
Soru 10 (Son iki eleman olan [4, 3] toplamda 7 eder ve uzunluğu 2'dir.)
Çeviri: Toplamı >= 7 olan en küçük alt dizinin uzunluğu nedir? (Dizi: [2, 3, 1, 2, 4, 3])
Cevap: A) 2
----------------------------------------------------------------------------------------
Soru 11 (Hangi işaretçiyi ne yöne kaydıracağımızı bilmemiz için verinin bir düzende olması şarttır.)
Çeviri: İki işaretçi tekniğini etkili uygulamak için hangi koşul gereklidir?
Cevap: A) Array must be sorted or have monotonic property (Dizi sıralı veya monotonik olmalı)
----------------------------------------------------------------------------------------
Soru 12 (Negatif toplam, o ana kadarki serinin bir sonraki elemana fayda sağlamayacağını gösterir, bu yüzden yeni bir başlangıç yapılır.)
Çeviri: Maksimum toplamlı alt diziyi bulan kodda, mevcut toplam negatif olursa ne yapılır?
Cevap: C) Sol işaretçiyi sağ işaretçiyle aynı indekse getirir ve toplamı 0 yapar.
----------------------------------------------------------------------------------------
Soru 13 (Kod, dizideki her elemanı birbiriyle kıyaslayıp aralarındaki mutlak farkın minimum olduğu değeri bulur.)
Çeviri: Verilen iç içe döngülü kod (abs(arr[i] - arr[j])) neyi hesaplar?
Cevap: A) Dizideki en küçük farka sahip çifti (The pair with the smallest difference).