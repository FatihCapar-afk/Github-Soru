Soru 1 (Her bir indeks, o ana kadar gelen tüm sayıların toplamını içinde barındırır.)
Çeviri: Prefix sum dizisi nedir?
Cevap: C) An array that stores the sum of elements from the start to the current index. (Başlangıçtan mevcut indekse kadar olan elemanların toplamını saklayan dizi.)
----------------------------------------------------------------------------------------
Soru 2 (Bir dizide sürekli farklı aralıkların (range sum) toplamı soruluyorsa, prefix sum bunu her seferinde baştan toplamadan yapmamızı sağlar.)
Çeviri: Prefix sum tekniği hangi senaryolarda özellikle kullanışlıdır?
Cevap: C) When you need to compute the sum of elements in a range frequently (Belirli bir aralıktaki elemanların toplamını sık sık hesaplamanız gerektiğinde.)
----------------------------------------------------------------------------------------
Soru 3 (Adım adım toplama yaparsak: 4, sonra 4+(-1)=3, sonra 3+2=5 ve son olarak 5+1=6 elde edilir.)
Çeviri: Verilen programın çıktısı ne olacaktır? (arr = [4, -1, 2, 1])
Cevap: A) 4 3 5 6
----------------------------------------------------------------------------------------
Soru 4 (Dizinin üzerinden sadece bir kez geçmek yeterli olduğu için doğrusal zaman (O(n)) harcanır.)
Çeviri: n boyutundaki bir dizi için prefix sum dizisi oluşturmanın zaman karmaşıklığı nedir?
Cevap: A) O(n)
----------------------------------------------------------------------------------------
Soru 5 (Toplamı bulmak için sadece çıkarma işlemi yapıldığından (P[R] - P[L-1]), sorgu anında gerçekleşir.)
Çeviri: Prefix sum dizisi oluşturulduktan sonra, bir alt dizinin toplamını sorgulamanın zaman karmaşıklığı nedir?
Cevap: D) O(1)
----------------------------------------------------------------------------------------
Soru 6 (Statik bir yapı olduğu için orijinal veri değişince tüm toplamlar bozulur ve güncellenmesi gerekir.)
Çeviri: Prefix sum dizisi oluşturulduktan sonra orijinal dizideki değerleri değiştirirsek ne olur?
Cevap: D) The prefix sum array becomes invalid and needs to be recalculated (Prefix sum dizisi geçersiz hale gelir ve yeniden hesaplanması gerekir.)
----------------------------------------------------------------------------------------
Soru 7 (2D Prefix Sum mantığında her hücre, kendisinin solundaki ve üstündeki tüm dikdörtgen alanın toplamını tutar. Hesaplama yapılırken çakışan alanlar eklenip çıkarılır.)
Çeviri: Verilen 2D dizi ([[10, 20, 30], [5, 10, 20], [2, 4, 6]]) koda gönderilirse çıktı ne olur?
Cevap: C) [[10, 30, 60], [15, 45, 95], [17, 51, 107]]
----------------------------------------------------------------------------------------
Soru 8 (Aralıktaki toplamı bulmak için en sondaki toplamdan, aralığa dahil olmayan kısmın toplamını atmış oluyoruz.)
Çeviri: Prefix sum dizisi kullanarak bir alt dizinin toplamını nasıl hesaplarsınız?
Cevap: C) By subtracting the prefix sum value of the left boundary index from the prefix sum value of the right boundary index (Sağ sınır indeksindeki prefix sum değerinden, sol sınır indeksinin bir öncesindeki değeri çıkararak.)