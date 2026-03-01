Soru 1 (QuickSort'un en kötü senaryosu (O(n^2)), pivot hep en küçük veya en büyük eleman seçildiğinde (yani dizi hep dengesiz bölündüğünde) ortaya çıkar. Eğer medyanı pivot seçersek, dizi her seferinde garanti olarak tam ortadan (n/2, n/2) ikiye bölünür. Bu da zaman karmaşıklığını mükemmel dengeli ağaç yapısı olan O(n log n)'e çeker.)
Bir dizinin ortanca değerini (medyanını) O(n) sürede bulan bir algoritmamız olduğunu varsayalım. Şimdi, QuickSort (Hızlı Sıralama) algoritmasını şöyle değiştirdiğimizi düşünelim: Her adımda önce bu algoritma ile dizinin medyanını buluyoruz ve ardından bu medyanı "pivot" olarak kullanıyoruz. Bu değiştirilmiş QuickSort'un en kötü durumdaki (worst-case) zaman karmaşıklığı ne olur?

Cevap: O(n Logn)
----------------------------------------------------------------------------------------
Soru 2 (En kötü durumda pivot en küçük veya en büyük eleman seçilir. Dizinin bir tarafında 0, diğer tarafında (n-1) eleman kalır. Dizi her adımda sadece 1 eleman küçüldüğü için T(n) = T(n-1) + O(n) denklemi oluşur ve bu denklemin çözümü O(n^2) çıkar.)
QuickSort algoritmasının en kötü durumu (worst-case) için özyineleme (recurrence) denklemi ve zaman karmaşıklığı nedir?

Cevap: Recurrence is T(n) = T(n-1) + O(n) and time complexity is O(n^2)
----------------------------------------------------------------------------------------
Soru 3 İlk elemanı pivot seçen klasik QuickSort için, dizinin tamamen artan (sorted) veya tamamen azalan (reverse sorted) olması fark etmez. Her iki senaryo da algoritmanın en kötü durumu (worst-case) olduğu için tamamen aynı sayıda karşılaştırma yapılır (O(n^2)).
QuickSort, "ilk elemanı" pivot alacak şekilde aşağıdaki iki farklı giriş dizisi üzerinde çalıştırılıyor:
(i) 1, 2, 3,......., n (Artan şekilde sıralı)
(ii) n, n-1, n-2,......, 2, 1 (Azalan şekilde sıralı)
Bu diziler için yapılan karşılaştırma sayıları sırasıyla C1 ve C2 olsun. Hangisi doğrudur?

Cevap: C1 = C2
----------------------------------------------------------------------------------------
Soru 4 (Radix Sort'un zaman karmaşıklığı $O(d * (n + b))$ formülüyle hesaplanır. Burada 'd' basamak sayısını temsil eder. Verilen aralık $n^k$ olduğu için, basamak sayısı $k * \log(n)$ gibi davranır (tabana göre). Bu da formülü sadeleştirildiğinde asimptotik olarak Θ(k*n) sonucunu verir.)
K sabiti n'den bağımsız (k>0) olmak üzere, (n^(k/2), n^k] aralığındaki n adet tam sayıyı sıralamak için Radix Sort kullanırsak çalışma süresi ne olur?

Cevap: Θ(kn)
----------------------------------------------------------------------------------------
Soru 5 ("Optimize edilmiş" Bubble Sort, iç döngüde bir "swapped" (yer değiştirme yapıldı mı) bayrağı kullanır. Eğer dizi zaten sıralı gelirse (en iyi durum), iç döngü diziyi bir tur (N kere) gezer, hiçbir yer değiştirme yapmaz, bayrak "false" kalır ve algoritma O(N) sürede döngüden çıkıp biter.)
Optimize edilmiş Bubble Sort (Kabarcık Sıralaması) algoritmasının en iyi durum (best-case) zaman karmaşıklığı nedir?

Cevap: O(N)
----------------------------------------------------------------------------------------
Soru 6 (Merge Sort'un ağaç derinliği, diziyi böldüğümüz orana bağlıdır. Dizi N/3 ve 2N/3 parçalarına bölündüğünde, en derin dalı 2N/3 olan parça oluşturur. Derinliği belirleyen denklem N * (2/3)^k = 1 olur. Bu da k = \log_{3/2}(N) demektir. Her seviyede N işlem yapıldığı için sonuç N \log_{3/2} N çıkar.)
Değiştirilmiş bir Merge Sort (Birleştirme Sıralaması) algoritmasında, giriş dizisi her adımda uzunluğunun (N) "üçte biri" (1/3) konumundan bölünüyor. (Yani N/3 ve 2N/3 şeklinde iki parçaya). Bu değiştirilmiş Merge Sort için en sıkı üst sınır (tightest upper bound) zaman karmaşıklığı nedir?

Cevap: N(logN taban 3/2) veya O(N log(3/2) N)
----------------------------------------------------------------------------------------
Soru 7 (Seçeneklerdeki Quick, Bubble ve Selection Sort algoritmalarının en kötü durumu O(n^2)'dir. Merge Sort ise her zaman, her durumda (en iyi, ortalama, en kötü) veriyi yarıya bölerek işlem yaptığı için en kötü durumu garantili olarak O(n log n)'dir.)
Aşağıdaki sıralama algoritmalarından hangisinin en kötü durum (worst-case) karmaşıklığı en düşüktür?

Cevap: Merge Sort
----------------------------------------------------------------------------------------
Soru 8 (Heap Sort kesinlikle karşılaştırma tabanlıdır (sayıları birbiriyle büyüklük-küçüklük olarak kıyaslar). Counting Sort ve Radix Sort ise karşılaştırma tabanlı değildir, doğrudan sayıların frekanslarına veya basamaklarına bakarlar.)
Karşılaştırma tabanlı (comparison-based) sıralama algoritmaları hakkında aşağıdakilerden hangisi yanlıştır?

Cevap: Heap Sort karşılaştırma tabanlı bir sıralama algoritması değildir. (Heap Sort is not a comparison based sorting algorithm.)
----------------------------------------------------------------------------------------
Soru 9 (Insertion Sort'un zaman karmaşıklığı O(n + I) olarak ifade edilir, buradaki 'I' tersinme (inversion) sayısıdır. Soruda I'nin en fazla 'n' olabileceği belirtilmiş. Bu durumda O(n + n) = O(2n) olur, asimptotik olarak (sabitleri attığımızda) Θ(n) yani lineer zaman elde edilir.)
Bir Insertion Sort (Araya Ekleme Sıralaması) algoritmasının en kötü durum çalışma süresi nedir (Eğer girdiler en fazla 'n' adet tersinme/inversion içerecek şekilde kısıtlanmışsa)?

Cevap: Θ (n)
----------------------------------------------------------------------------------------
Soru 10 (Pivotu dizinin ortasından seçmek, ortadaki sayının her zaman medyan (değerce ortanca) olduğu anlamına gelmez. Eğer veriler özel olarak ayarlanmışsa (örn: en büyük eleman hep ortadaysa), algoritma yine diziyi 1 ve n-1 şeklinde dengesiz bölecek ve en kötü duruma (O(n^2)) düşecektir.)
n elemanlı bir diziniz var. Quick Sort algoritmasını uygularken pivot olarak her zaman dizinin (fiziksel olarak) tam ortasındaki elemanı (index olarak N/2) seçtiğinizi varsayalım. Bu durumda en kötü senaryonun (worst case) zaman karmaşıklığı ne olur?

Cevap: O(n^2)
----------------------------------------------------------------------------------------
Soru 11 (Çok büyük veri setlerinde (bellek/RAM yettiği sürece) QuickSort, sabit çarpanının çok küçük olması ve önbellek dostu (cache-friendly) olması sebebiyle pratikte Merge Sort veya Heap Sort'tan daha hızlı çalışır.)
Genel olarak 1 milyondan fazla elemanı olan bir diziyi sıralamak için kullanılacak en iyi algoritma hangisidir?

Cevap: Quick sort.
----------------------------------------------------------------------------------------
Soru 12 (Selection Sort (Seçmeli Sıralama), dizinin içindeki en küçük/en büyük elemanı ararken sadece tarama yapar ve her döngüde "sadece 1 kere" swap işlemi gerçekleştirir. Toplam swap sayısı en fazla O(N)'dir. Diğerlerinde ise swap işlemi O(N^2) veya O(N log N) kere yapılabilir.)
Takas (swap) işleminin sistem açısından çok maliyetli (yavaş) olduğu bir durumu düşünün. Takas işlemi sayısını genel olarak en aza indirmek için hangi sıralama algoritması tercih edilmelidir?

Cevap: Selection Sort
----------------------------------------------------------------------------------------
Soru 13 (Örneğin, elimizde Ahmet(50) ve Ayşe(50) puanlı iki kişi olsun. Eğer sıralamadan önce Ahmet dizide Ayşe'den önce geliyorsa, "kararlı" bir algoritma ile sıralandıktan sonra da Ahmet, Ayşe'den önce gelmeye devam eder.)
Bir sıralama tekniğine "kararlı" (stable) denmesinin sebebi nedir?

Cevap: Birbirinin aynısı olan (non-distinct) elemanların orijinal dizideki göreceli sırasını korumasıdır.
----------------------------------------------------------------------------------------
Soru 14 (En kötü durumda Quicksort O(n^2) zaman alır. Heapsort ve Mergesort ise her türlü senaryoda dengeli yapıları sayesinde maksimum O(n log n) zamanda bitirir. Dolayısıyla en kötü durum senaryosunda bu ikisi Quicksort'u geçer.)
Şu sıralama algoritmalarını düşünün: I. Quicksort, II. Heapsort, III. Mergesort. Bunlardan hangisi veya hangileri en kötü durumda (worst case) en az zamanda (en hızlı) çalışır?

Cevap: II and III only (Sadece Heapsort ve Mergesort)
----------------------------------------------------------------------------------------
Soru 15 (12. Soruda açıkladığımız gibi, Selection Sort her ana geçişte sadece tek bir swap yapar.)
Aşağıdaki "yerinde" (in-place) sıralama algoritmalarından hangisi en az sayıda takas (swap) işlemine ihtiyaç duyar?

Cevap: Selection sort
----------------------------------------------------------------------------------------
Soru 16 (Sayıların üst sınırı n^2 - 1$ olarak verildiğinde, sayıları n tabanında (base n) ifade edebiliriz. Bu durumda en büyük sayı maksimum 2 basamaklı olur. Radix sort 2 basamak için O(2 * n) çalışır, sabit silindiğinde O(n) sonucuna ulaşılır.)
Aşağıdaki algoritmalarından hangisi, 0 ile (n^2 - 1) aralığındaki n adet tam sayıyı artan sırada O(n) lineer zamanda sıralayabilir?

Cevap: Radix sort
----------------------------------------------------------------------------------------
Soru 17 (Merge Sort büyük problemi alır (dizi), sürekli yarıya bölerek (Divide) en küçük (tek elemanlı) ve kolay çözülebilir alt problemlere ayırır. Sonra bunları sıralayarak tekrar birleştirir (Conquer).)
Merge Sort (Birleştirme Sıralaması) algoritmasında hangi algoritma tasarım tekniği kullanılır?

Cevap: Divide and Conquer (Parçala ve Fethet)
----------------------------------------------------------------------------------------
Soru 18 (3. sorunun aynısı. Standart Quicksort için hem tamamen sıralı hem de tamamen ters sıralı diziler en kötü senaryoyu oluşturur ve tam olarak aynı sayıda işlemi gerektirir (O(n^2)).)
Quick Sort aşağıdaki 2 farklı dizi üzerinde çalıştırılıyor: A: 1, 2, 3……n (Artan) ve B: n, n – 1, n – 2 …… 1 (Azalan). Sırasıyla C1 ve C2 yapılan karşılaştırma sayıları ise hangisi doğrudur?

Cevap: C1 = C2
----------------------------------------------------------------------------------------
Soru 19 (5. soruda da değindiğimiz gibi, eğer dizi zaten sıralıysa ve kod optimize edilmişse, algoritma baştan sona bir kere tarar, hiçbir takas yapmadığını görür ve hemen kapanır.)
Bubble Sort'un (Kabarcık Sıralaması) en iyi durumu (best case) ne zaman ortaya çıkar?

Cevap: Elemanlar zaten artan sırada sıralanmış olduğunda (When elements are sorted in ascending order)
----------------------------------------------------------------------------------------
Soru 20 (Insertion sort çalışırken veriler dışarıdan tek tek akıyorsa (streaming/online) gelen veriyi anında doğru yere yerleştirebilir. Aynı değere sahip verilerin sırasını bozmadığı için de kararlıdır. Ancak 10.000 eleman vb. gibi büyük yapılarda felaket yavaşlar.)
Insertion Sort (Araya Ekleme Sıralaması) için "Online" (veriler geldikçe sıralayabilme) ve "Stable" (kararlı) özellikleri hakkında hangi ifade doğrudur?

Cevap: Araya Ekleme Sıralaması kararlıdır (stable), çevrimiçidir (online) ancak çok sayıda eleman içeren diziler için (O(n^2) olduğu için) uygun değildir.
----------------------------------------------------------------------------------------
Soru 21 
(En iyi durumda:
Merge Sort her halükarda veriyi böler ve birleştirir: O(n log n)
Selection Sort her halükarda tüm diziyi tarar: O(n^2) (Hata uyarısı: Bazı kaynaklarda Selection sort daima O(n^2) olduğu için Merge sorttan yavaştır, bu seçenek sorunun orijinalinde hatalı formüle edilmiş olabilir. Genel kabul gören Best Case'ler: Selection(n^2) > Merge(n log n) = Quick(n log n) > Insertion(n)'dir).
Insertion Sort dizi sıralıysa anında biter: O(n).)

Algoritmaların en iyi durum (best case) zaman karmaşıklıklarına göre sıralanışı (Büyükten Küçüğe - yani Yavaş olandan Hızlı olana) hangisidir?

Cevap: Merge sort > selection sort > quick sort > insertion sort (Yavaştan -> Hızlıya doğru)
----------------------------------------------------------------------------------------
Soru 22 (İlk adımda 4'ü alır, solundaki 5 ile kıyaslar ve öne atar. İkinci adımda 3'ü alır, 4 ve 5'in önüne taşır. Bu şekilde her adımda sağdan bir eleman alıp sol taraftaki "sıralanmış alt dizinin" içine doğru noktaya gömer.)
arr[5] = {5,4,3,2,1} elemanlarından oluşan bir dizi düşünün. Bu diziye Insertion Sort (Araya Ekleme) uygulandığında yapılan ekleme/kaydırma adımları nasıldır?

Cevap:
4 5 3 2 1
3 4 5 2 1
2 3 4 5 1
1 2 3 4 5
----------------------------------------------------------------------------------------
Soru 23 (Pratikte pivotu rastgele (randomized) seçmek kötü durumu neredeyse imkansız kılar. Dizi boyutu çok küçüldüğünde (örn. 10 eleman) fonksiyon çağırma maliyetinden kurtulmak için hızlı olan Insertion Sort kullanılır. Tail recursion belleği korur. 4 numara ise teoride O(n log n) yapsa da o medyan algoritmasının kendi sabitleri çok büyük olduğu için pratikte sistemi yavaşlatır, bu yüzden kullanılmaz.)
Aşağıdaki değişikliklerden hangisi tipik bir QuickSort'un performansını ortalamada iyileştirir ve pratikte sıkça yapılır?

Kötü durumu azaltmak için pivotu rastgele seçmek.

Özyinelemeli çağrıları azaltmak için küçük boyutlu dizilerde Insertion Sort çağırmak.

Kuyruk çağırma optimizasyonları (tail recursion) yapmak.

Lineer medyan arama algoritmasıyla pivotu bulup worst-case'i engellemek.

Cevap: 1, 2 and 3
----------------------------------------------------------------------------------------
Soru 24 (16. sorudaki mantıkla aynıdır. Aralığın üst sınırı polinomik bir ifade (n^c) olduğu sürece, Radix Sort sayıyı n tabanında yazarak c basamaklı bir işlem haline getirir. Bu da O(c*n) yani asimptotik olarak O(n) lineer zaman verir.)
Sayıların 1 ile n^6 aralığında olduğu bir dizi verilmiştir. Bu sayıları lineer zamanda (O(n)) sıralamak için hangi algoritma kullanılabilir?

Cevap: Radix Sort
----------------------------------------------------------------------------------------
Soru 25 (Merge Sort RAM'de değil de diskte okuma yaparken (slow sequential memory) blok blok işlem yaptığı için mükemmeldir. Doğası gereği kararlıdır (stable). Heap Sort'a kıyasla önbellek (cache) ve dallanma tahmini (branch prediction) açısından genelde daha iyi çalışır.)
Merge Sort hakkında hangisi doğrudur?

Cevap: Hepsi doğru (All of the above).
----------------------------------------------------------------------------------------
Soru 26 (Tüm elemanlar aynı olduğunda (örn: 5, 5, 5, 5), dizi zaten "sıralı" olarak kabul edilir. Insertion sort zaten sıralı bir dizi ile karşılaştığında hiçbir elemanı kaydırmadan sadece O(n) sürede tarayıp işlemi bitirir.)
Girdi dizisindeki tüm elemanlar birbirinin tamamen aynısı (identical) olduğunda, tipik bir sıralama algoritması olarak hangisi en az zamanı (en hızlı süreyi) alır?

Cevap: Insertion Sort
----------------------------------------------------------------------------------------
Soru 27 (Buna "External Sorting" (Harici Sıralama) denir. 1 GB veriyi tek seferde 100 MB'lık RAM'e sığdıramazsın. Merge Sort dosyayı 100'er MB'lık parçalara böler, RAM'de sıralayıp diske yazar, sonra bu küçük dosyaları yavaş yavaş, disk üzerinden birleştirir (merge).)
Elindeki 100 MB'lık ana bellekle (RAM) 1 GB'lık devasa bir veriyi sıralaman gerekiyor. Hangi sıralama tekniği en uygundur?

Cevap: Merge sort
----------------------------------------------------------------------------------------
Soru 28 (Heapsort önce veriyi ağaca (Max-Heap) çevirir. Kök olan en büyük elemanı en sona (28) atar. Sonra 2. en büyük elemanı bulur ve onu sondan bir öncekine (27) atar. Dizinin sonunda 27 ve 28 sabitlendiğine göre, kökten sona alma ve yeniden heapify işlemi 2 kez yapılmıştır.)
Sekiz tamsayılık bir diziyi Heapsort kullanarak sıralıyoruz ve bazı heapify (yığınlaştırma) işlemlerini yeni bitirdik. Dizi şu an şöyle görünüyor: 16 14 15 10 12 27 28. Ağacın kökünde (root) kaç adet heapify işlemi gerçekleştirilmiştir?

Cevap: 2
----------------------------------------------------------------------------------------
Soru 29 (Quicksort'ta bir eleman pivot seçilip işlem bittiğinde, pivot kesinlikle dizideki nihai doğru konumuna yerleşmiş olmalıdır. Ayrıca pivotun solundakiler ondan küçük, sağındakiler büyük olmalıdır.
7'ye bakıyoruz: Nihai yerinde mi? (Küçükler solda 2,5,1 / Büyükler sağda 9,12,11,10). Evet olabilir.
9'a bakıyoruz: Solundakiler küçük (2,5,1,7), sağındakiler büyük (12,11,10). O da olabilir.)
Sekiz tamsayılık bir diziyi quicksort kullanarak sıralıyoruz ve ilk bölme işlemini (partitioning) bitirdiğimizde dizi şöyle görünüyor: 2 5 1 7 9 12 11 10. Hangi ifade doğrudur?

Cevap: Pivot 7 de olabilir, 9 da olabilir. (The pivot could be either the 7 or the 9.)
----------------------------------------------------------------------------------------
Soru 30 (Dizi büyük oranda sıralıysa Insertion Sort kaydırma (shift) işlemi yapmaz, sadece doğru yeri teyit edip hemen yanındakine geçer. Karmaşıklığı neredeyse O(n)'e yaklaşarak diğer tüm algoritmalardan daha hızlı sonuç verir.)
Sıralanmış veya neredeyse tamamen sıralanmış (sadece 1-2 eleman yanlış yerde) bir diziye uygulandığında, tipik uygulamalar arasında en iyi performansı veren sıralama algoritması hangisidir?

Cevap: Insertion Sort
----------------------------------------------------------------------------------------
Soru 31 (Quicksort, pivot'a göre elemanları rastgele sağa ve sola fırlattığı (swap yaptığı) için aynı değere sahip elemanların orijinal sırası çok yüksek ihtimalle bozulur. (Insertion, Merge ve Bubble sort kararlı algoritmaların başını çeker).)
Aşağıdakilerden hangisi kendi tipik uygulamasında "kararlı" (stable) BİR SIRALAMA ALGORİTMASI DEĞİLDİR?

Cevap: Quick Sort