Question 1 (Dizinin mevcut durumu, dizinin sonundaki büyük elemanların (27 ve 28) yerlerine yerleştiğini ve kök elemanının tekrar yığın yapısına uygun hale getirilmesi için iki ana aşamanın tamamlandığını gösterir.)
Soru: Sekiz tam sayıdan oluşan bir diziyi heapsort kullanarak sıraladığımızı ve bazı heapify (max veya min) işlemlerini henüz bitirdiğimizi varsayalım. Dizi şu an şu şekildedir: 16 14 15 10 12 27 28. Yığının kökünde (root) kaç tane heapify işlemi yapılmıştır?

Cevap: B) 2
----------------------------------------------------------------------------------------
Question 2 (Dinamik veri yapıları (bağlı listeler, ağaçlar vb.) çalışma anında boyutu değişebilen veriler olduğu için, bu verilerin saklanması için yönetilebilir bir alan olan "heap" belleği zorunludur.)
Soru: Çalışma zamanı ortamında (runtime environment) hangi dillerin mutlaka "heap" bellek tahsisine ihtiyacı vardır?

Cevap: D) Those that allow dynamic data structures
----------------------------------------------------------------------------------------
Question 3 (Min-heap yapısında en küçük eleman köktedir, ancak en büyük eleman herhangi bir yaprak düğümde (leaf node) olabilir. Yaprak sayısı yaklaşık n/2 olduğu için tüm yaprakları taramak doğrusal zaman (O(n)) gerektirir.)
Soru: Bir dizi olarak uygulanan n elemanlı bir ikili min-heap (binary min-heap) H olsun. H içindeki maksimum elemanı bulmak için en iyi (optimal) algoritmanın en kötü durum (worst case) zaman karmaşıklığı nedir?

Cevap: C) O(n)
----------------------------------------------------------------------------------------
Question 4 (100 değeri dizinin en sonundadır ve max-heap kuralını bozmaktadır. 100'ü yukarı taşımak (bubble-up) için 50 ve ardından 89 ile yer değiştirmesi gerekir, bu da toplam 2 işlem yapar.)
Soru: Aşağıdaki eleman dizisini düşünün: <89, 19, 50, 17, 12, 15, 2, 5, 7, 11, 6, 9, 100>. Bu diziyi bir max-heap'e dönüştürmek için gereken minimum yer değiştirme (interchange) sayısı kaçtır?

Cevap: C) 2
----------------------------------------------------------------------------------------
Question 5 (Heap yapısının temel özelliği, en büyük (max-heap) veya en küçük (min-heap) elemanın her zaman kök dizininde (genelde 0 veya 1. indeks) bulunmasıdır, bu yüzden erişim sabittir.)
Soru: Bir heap yapısında Min/Max (kök) değerini bulmak ne kadar zaman alır?

Cevap: C) O(1)
----------------------------------------------------------------------------------------
Question 6 (Heap yapıları; öncelikli kuyruklar (hastane/medikal), Huffman kodlaması (dosya sıkıştırma) ve sıralı işlem takibi (borsa/stok) gibi birçok alanda temel olarak kullanılır.)
Soru: Heap veri yapısının uygulamaları nelerdir?

Cevap: D) All of these
----------------------------------------------------------------------------------------
Question 7 (1023 elemanlı tam bir ağaçta 512 yaprak düğüm vardır. Maksimum eleman bu yapraklar arasındadır. 512 eleman arasından en büyüğünü bulmak için $n-1$ yani 511 karşılaştırma yapılır.)
Soru: 1023 eleman içeren bir ikili min-heap dizi gösterimini düşünün. Heap içindeki maksimum elemanı bulmak için gereken minimum karşılaştırma sayısı kaçtır?

Cevap: B) 511
----------------------------------------------------------------------------------------
Question 8 (İlk silmede 25 çıkar ve yerine 12 gelir, sonra heapify yapılır. İkinci silmede yeni kök (16) çıkar ve yerine 8 gelir, tekrar heapify yapıldığında en büyükler yukarı çıkar.)
Soru: Bir binary-max heap verildiğinde, elemanlar dizide 25, 14, 16, 13, 10, 8, 12 şeklinde saklanmaktadır. İki silme (delete) işleminden sonra dizinin içeriği ne olur?

Cevap: D) 14, 13, 12, 10, 8
----------------------------------------------------------------------------------------
Question 9 (Bu, ikili yığınların matematiksel bir özelliğidir; yapraklardan yukarı doğru çıktıkça düğüm sayısı her seviyede yaklaşık yarıya iner.)
Soru: n elemanlı herhangi bir heap yapısında h yüksekliğindeki düğüm sayısı kaçtır?

Cevap: D) ceil(n/2^{h+1})
----------------------------------------------------------------------------------------
Question 10 (Bir max-heap'te her ebeveyn, çocuklarından büyük olmalıdır. C şıkkında 26 > (15, 17), 15 > (14, 11) ve 17 > (9, 13) kuralı eksiksiz sağlanır.)
Soru: Aşağıdaki dizilerden hangisi bir binary max-heap temsil eder?

Cevap: C) [26, 15, 17, 14, 11, 9, 13]
----------------------------------------------------------------------------------------
Question 11 (B seçeneğinde tüm ebeveyn düğümler çocuklarından büyüktür. Diğer şıklarda (örneğin A'da 2'nin altında 8 olması gibi) heap kuralını bozan durumlar vardır.)
Soru: Aşağıdakilerden hangisi geçerli (valid) bir heap'tir?

Cevap: B) 16 14 10 8 7 9 3 2 4 1
----------------------------------------------------------------------------------------
Question 12 (70 değeri yanlış yerdedir. Önce ebeveyni olan 10 ile, sonra yeni ebeveyni olan 40 ile yer değiştirerek max-heap kuralını sağlar.)
Soru: 89, 19, 40, 17, 12, 10, 2, 5, 7, 11, 6, 9, 70 dizisini maksimum elemanın kökte olduğu bir heap'e dönüştürmek için gereken minimum yer değiştirme sayısı kaçtır?

Cevap: C) 2
----------------------------------------------------------------------------------------
Question 13 (A şıkkında her eleman, altındaki çocuk düğümlerden büyüktür (örneğin 17 > 6 ve 13; 6 > 12 ve 7 gibi - burada dizilim tam bir ağaç yapısına uygundur).)
Soru: Aşağıdaki dizi dizilerinden hangisi bir heap oluşturur?

Cevap: A) {23, 17, 14, 6, 13, 10, 1, 12, 7, 5}
----------------------------------------------------------------------------------------
Question 14 (Min-heap'te daha küçük sayılar daha yukarıda olmalıdır ancak 9 sayısı, kendisinden küçük 8 tane sayı (1, 2, ..., 8) tarafından üst seviyelerde tutularak 8. derinliğe kadar itilebilir.)
Soru: [1, 1023] aralığındaki her tam sayının birer kez kullanılmasıyla bir binary min-heap oluşturuluyor. 9 tam sayısının görünebileceği maksimum derinlik nedir?

Cevap: C) 8
----------------------------------------------------------------------------------------
Question 15 (Bir düğüm silindiğinde yerine son eleman konur ve bu eleman ağaç boyunca yukarı veya aşağı taşınır. Bu işlem en fazla ağacın yüksekliği (d veya \log n) kadar sürer.)
Soru: i. indeksteki düğümü silmek için bir delete(i) operatörü tasarlanacaktır. Heap ağacının derinliği d ise, eleman silindikten sonra heap yapısını tekrar düzenlemenin zaman karmaşıklığı nedir?

Cevap: B) O(d) but not O(1)
----------------------------------------------------------------------------------------
Question 16 (Tekil eklemeler O(n \log n) gibi görünse de, aşağıdan yukarıya doğru yapılan Build Heap işlemi matematiksel olarak doğrusal zamanda, yani O(n) sürede tamamlanır.)
Soru: "Build Heap" işleminin zaman karmaşıklığı nedir?

Cevap: C) O(n)
----------------------------------------------------------------------------------------
Question 17 (35 en sona eklenir. Ebeveyni olan 15'ten büyük olduğu için onunla yer değiştirir. Sonraki ebeveyni 30'dan da büyük olduğu için onunla da yer değiştirir ve 40'ın altına yerleşir.)
Soru: 40, 30, 20, 10, 15, 16, 17, 8, 4 dizisiyle temsil edilen bir max-heap'e 35 değeri eklenirse, yeni heap ne olur?

Cevap: D) 40, 35, 20, 10, 15, 16, 17, 8, 4, 30
----------------------------------------------------------------------------------------
Question 18 (1-tabanlı dizi gösteriminde, herhangi bir düğümün ebeveyni her zaman bulunduğu indeksin yarısının tam sayı kısmıdır.)
Soru: 1'den n'e kadar olan bir dizide, i indeksindeki elemanın ebeveyninin indeksi nedir?

Cevap: B) floor(i/2)
----------------------------------------------------------------------------------------
Question 19 (1 sona eklenir (değişiklik olmaz). 7 sona eklenir, ebeveyni olan 5 ile yer değiştirir ve yeni yapıyı oluşturur.)
Soru: Başlangıçta [10, 8, 5, 3, 2] olan bir max-heap'e sırasıyla 1 ve 7 sayıları eklenirse yeni seviye-sırası ne olur?

Cevap: A) 10, 8, 7, 3, 2, 1, 5
----------------------------------------------------------------------------------------
Question 20 (İki heap'i birleştirmek (merge), özel heap türleri (Fibonacci heap gibi) kullanılmıyorsa genellikle tüm elemanları yeniden düzenlemeyi gerektirir ve en maliyetli işlemdir.)
Soru: Aşağıdaki Binary Min Heap işlemlerinden hangisi en yüksek zaman karmaşıklığına sahiptir?

Cevap: B) Merging with another heap...
----------------------------------------------------------------------------------------
Question 21 (İki diziyi birleştirip (toplam 2n eleman) üzerlerinde Build Heap algoritmasını çalıştırmak doğrusal zamanda (O(n)) sonuç verir.)
Soru: Her biri n boyutunda iki max-heap verildiğinde, bunları tek bir max-heap yapmak için gereken minimum zaman karmaşıklığı nedir?

Cevap: C) O(n)
----------------------------------------------------------------------------------------
Question 22 (Elemanlar eklendikçe "yukarı kaydırma" (bubble-up) işlemi uygulanır. Örneğin 30 eklendiğinde 15 ile yer değiştirir; 25 eklendiğinde 20 ile yer değiştirir. Tüm elemanlar yerleştiğinde, her ebeveynin çocuklarından büyük olduğu ve tam ağaç yapısının korunduğu (a) şıkkındaki heap yapısı oluşur.)
Soru: 32, 15, 20, 30, 12, 25, 16 elemanları verilen sırayla bir Max Heap yapısına tek tek ekleniyor. Oluşan sonuç Max Heap hangisidir?

Cevap: A) a
----------------------------------------------------------------------------------------
Question 23 (Bir yapının heap sayılması için hem şekil şartını (tam ikili ağaç olması) hem de değer şartını (ebeveyn-çocuk ilişkisi) sağlaması gerekir.)
Soru: Bir ağacın "heap" olması için gerekli şart nedir?

Cevap: C) The tree must be complete and Every Root value should be greater or smaller than the children's value.
----------------------------------------------------------------------------------------
Question 24 (7 sabit bir sayıdır. $n$ ne kadar büyük olursa olsun, 7. en küçük eleman ağacın ilk birkaç seviyesi içinde sınırlı bir alandadır, bu yüzden arama süresi sabittir.)
Soru: n elemanlı bir min-heap'te 7. en küçük eleman ne kadar sürede bulunabilir?

Cevap: D) O(1)
----------------------------------------------------------------------------------------
Question 25 (Eğer elemanlar toplu eklenip en son Build Heap yapılırsa işlem doğrusal zamanda (O(n)) biter.)
Soru: n elemanlı bir heap'e n eleman daha eklemek için gereken toplam süre nedir?

Cevap: B) O(n)
----------------------------------------------------------------------------------------
Question 26 (Tanım gereği tüm heap yapıları tam ikili ağaç olmak zorundadır (son seviye hariç tüm seviyeler dolu, son seviye soldan sağa doludur).)
Soru: Bir min-heap her zaman bir tam ikili ağaçtır (complete binary tree).

Cevap: A) True
----------------------------------------------------------------------------------------
Question 27 (Max-heap kuralı (Ebeveyn >= Çocuk) bu üç dizide de ağaç yapısı boyunca korunmaktadır.)
Soru: Aşağıdaki dizilerden hangileri bir binary max-heap temsil eder?

Cevap: (1), (3) ve (4). seçenekler.
----------------------------------------------------------------------------------------
Question 28-29 (3-ary heap yapısında her düğümün 3 çocuğu vardır. Elemanlar dizide 3i+1, 3i+2, 3i+3 formülüyle yerleşir ve max-heap kuralı yine geçerlidir.)
Soru: 3-ary (üçlü) max-heap yapısı ile ilgili sorular.

Cevap 28: A) 10, 7, 9, 8, 3, 1, 5, 2, 6, 4

Cevap 29: D) 9, 5, 6, 8, 3, 1
----------------------------------------------------------------------------------------
Question 30 (Bir yapının max-heap olması için iki şartı sağlaması gerekir:

Şekil Şartı: Tam bir ikili ağaç olmalı (A şıkkı eksik düğüm nedeniyle elenir).

Değer Şartı: Her ebeveyn düğüm, çocuklarından büyük veya eşit olmalıdır (C ve D şıkları bu kuralı ihlal eder). (B) şıkkı her iki şartı da sağlar.)
Soru: Aşağıdakilerden hangisi bir max-heap yapısıdır?

Cevap: B) (B)