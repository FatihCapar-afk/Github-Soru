Question 1 (Heap Sort, verileri bir yığın (heap) veri yapısına dönüştürerek sıralar; Quick Sort veya Merge Sort gibi problemi alt parçalara bölüp birleştirme mantığıyla çalışmaz.)
Soru: Aşağıdaki algoritmalardan hangisi doğası gereği bir "Böl ve Yönet" (Divide & Conquer) algoritması DEĞİLDİR?

Cevap: B) Heap Sort
----------------------------------------------------------------------------------------
Question 2 ("Horner Metodu" kullanılarak polinom a_0 + x(a_1 + x(a_2 + x(a_3))) şeklinde yazılabilir. Bu sayede sadece 3 çarpma işlemiyle sonuç hesaplanır.)
oru: Tüm a_i =\ 0 olmak üzere p(x) = a_0 + a_1x + a_2x^2 + a_3x^3   polinomu veriliyor. Bu polinomu bir x girdisi için değerlendirmek için gereken minimum çarpma sayısı kaçtır?

Cevap: A) 3
----------------------------------------------------------------------------------------
Question 3 ("Üs almayı kareleyerek yapma" (Exponentiation by squaring) tekniği sayesinde, her adımda üssü yarıya indirerek işlemi logaritmik zamanda tamamlayabilirsiniz.)
Soru: Elinizde pow() fonksiyonu olmadığını varsayalım. x^n değerini (n pozitif tam sayı) hesaplamak için yazacağınız fonksiyonun mümkün olan en iyi zaman karmaşıklığı ne olur?

Cevap: D) O(Logn)
----------------------------------------------------------------------------------------
Question 4 (İkili arama (Binary Search) mantığı, dizi sıralı olduğu sürece (döndürülmüş olsa bile) O(\log n) sürede çalışabilir; ancak tamamen sırasız bir dizide arama her zaman doğrusal zaman (O(n)) gerektirir.)
Soru: n boyutlu bir dizide bir x elemanını arama problemi, hangi durumlarda O(\log n) sürede çözülebilir?Dizi sıralıysaDizi sıralıysa ve k kadar döndürülmüşse (k biliniyor)Dizi sıralıysa ve $k$ kadar döndürülmüşse (k bilinmiyor)Dizi sıralı değilse

Cevap: C) 1, 2 and 3 only
----------------------------------------------------------------------------------------
Question 5 (Sekant yöntemi, fonksiyonun köküne yaklaşmak için iki nokta arasındaki doğrusal interpolasyonu kullanır; bu formül yeni tahmin noktasını hesaplar.)
Soru: Sekant yöntemi (Secant method) ile kök bulma algoritmasındaki eksik ifade (xt = ?) aşağıdakilerden hangisidir?

Cevap: D) x_a - (x_b - x_a) f(x_a) / (f(x_b) - f(x_a))
----------------------------------------------------------------------------------------
Question 6 (Böl ve yönet kullanılsın ya da kullanılmasın, sırasız bir dizide hem min hem max değerini bulmak için gereken karşılaştırma sayısı en kötü durumda her zaman aynı mertebededir.)
Soru: Sırasız bir dizide minimum ve maksimum elemanları bulma problemini düşünün. A1 algoritması böl ve yönet kullanmadan, A2 ise diziyi doğrusal tarayarak (linear scan) bu işlemi yapıyor. En kötü durumda karşılaştırma sayıları (a_1 ve a_2) arasındaki ilişki nedir?

Cevap: C) a1 = a2
----------------------------------------------------------------------------------------
Question 7 (Insertion Sort, dizi zaten sıralıysa (best case) her elemanı sadece bir kez kontrol eder ve O(n) sürede biter; bu durumda diğer algoritmalardan daha az karşılaştırma yapar.)
Soru: Verilen sıralı diziyi (23, 32, 45, 69, 72, 73, 89, 97) tekrar artan sırada sıralamak için hangi algoritma en az sayıda karşılaştırma yapar?

Cevap: C) Insertion sort
----------------------------------------------------------------------------------------
Question 8 (Ağacın kök düğümü (root), eğer sağ çocuğu varsa maksimum eleman olamaz; değilse bile kökün sol çocuğu her zaman maksimumdan küçüktür. Bu seçimi yapmak için ağacı taramaya gerek yoktur.)
Soru: n elemanlı bir ikili arama ağacında (BST), maksimum elemandan daha küçük olan herhangi bir elemanı seçmenin zaman karmaşıklığı nedir?

Cevap: D) Θ(1)
----------------------------------------------------------------------------------------
Question 9 (Eğer aranan eleman pivotun solundaysa sadece sol parçaya bakılır; sağındaysa sağ parçaya bakılır ve aranan sıra (k) çıkarılan eleman sayısı kadar kaydırılır.)
Soru: Verilen kth_smallest fonksiyonunda boş bırakılan yerlere sırasıyla hangi argüman listeleri gelmelidir?

Cevap: A) (a, left_end, k) ve (a+left_end+1, n–left_end–1, k–left_end–1)
----------------------------------------------------------------------------------------
Question 10 (Elemanları çiftler halinde karşılaştırarak (böl ve yönet mantığıyla) min ve max bulmak için en verimli algoritma yaklaşık 1.5n karşılaştırma yapar.v)
Soru: n elemanlı bir dizide minimum ve maksimum değerleri bulmak için gereken karşılaştırma sayısı t için hangisi doğrudur?

Cevap: C) t > n ve t ≤ 3⌈n/2⌉
----------------------------------------------------------------------------------------
Question 11 (Bu, Öklid algoritmasının çıkarma işlemi kullanarak uygulanan halidir ve iki sayının en büyük ortak bölenini (EBOB/GCD) bulur.)
Soru: Verilen C programı neyi hesaplar? (Sayılar eşitlenene kadar büyükten küçüğü çıkarıyor).

Cevap: C) the greatest common divisor of x and y
----------------------------------------------------------------------------------------
Question 12 (Dizi ikiye bölünür, her iki yarının kendi içindeki ve merkezi kesen alt dizilerin toplamı hesaplanır; bu rekürans yapısı Merge Sort ile aynı karmaşıklığı (O(n \log n)) verir.)
Soru: Maksimum Alt Dizi Toplamı (Maximum Subarray Sum) problemi böl ve yönet yöntemiyle çözüldüğünde en kötü durum zaman karmaşıklığı ne olur?

Cevap: B) O(nLogn)
----------------------------------------------------------------------------------------
Question 13 (Min-heap yapısında en küçük eleman köktedir, ancak maksimum eleman herhangi bir yaprak düğümde (leaf node) olabilir. Yapraklar toplam elemanların yarısı (n/2) olduğu için tümünü taramak doğrusal zaman (O(n)) gerektirir.)
Soru: n elemanlı bir ikili min-heap (binary min-heap) yapısında maksimum elemanı bulmak için en iyi algoritmanın en kötü durum zaman karmaşıklığı nedir?

Cevap: C) Θ(n)