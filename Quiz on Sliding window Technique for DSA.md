Soru 1 (Bu teknik, bir dizi üzerinde sürekli en baştan hesaplama yapmak yerine, pencereyi kaydırarak gereksiz tekrarlardan kaçınmamızı ve hızı artırmamızı sağlar.)
Çeviri: Algoritmalar bağlamında "sliding window" tekniğini hangi amaçla kullanabiliriz?
Cevap: B) Bir alt dizideki maksimum veya minimum toplamı bulmanın zaman karmaşıklığını optimize etmek için
----------------------------------------------------------------------------------------
Soru 2 (Pencere dizi üzerinde sadece bir kez baştan sona kaydığı için işlem miktarı dizi boyutuyla doğru orantılıdır (O(n)).)
Çeviri: n boyutundaki bir dizide, k boyutundaki herhangi bir alt dizinin maksimum toplamını bulmak için "sliding window" kullanıldığında zaman karmaşıklığı ne olur?
Cevap: B) O(n)
----------------------------------------------------------------------------------------
Soru 3 (Aranan tüm karakterleri bulana kadar pencereyi genişletip, ardından en küçük boyutu bulmak için daralttığımızdan pencere boyutu sabit kalmaz.)
Çeviri: Belirli tüm karakterleri içeren en küçük alt dizeyi (substring) bulma probleminde hangi tip pencere kullanılır?
Cevap: B) Variable size (Değişken boyutlu)
----------------------------------------------------------------------------------------
Soru 4 (Pencerenin dışına çıkan eski sayıyı toplamdan düşüp, pencereye yeni dahil olan sayıyı eklemek, tüm pencereyi tekrar toplamaktan çok daha hızlıdır.)
Çeviri: k boyutundaki bir kayan pencerede, sağa doğru bir adım ilerlerken pencere toplamını nasıl verimli bir şekilde güncelleriz?
Cevap: B) Subtract outgoing element, add incoming element (Çıkan elemanı çıkarıp, giren elemanı ekleyerek)
----------------------------------------------------------------------------------------
Soru 5 ([1, 2], [2, 1], [1, 2] veya [2, 3] gibi tüm 2'li alt dizilerde en fazla 2 farklı sayı bulunabilir.)
Çeviri: arr = [1, 2, 1, 2, 3] dizisi ve k = 2 verildiğinde, 2 boyutundaki herhangi bir alt dizideki maksimum farklı (distinct) eleman sayısı kaçtır?
Cevap: 2
----------------------------------------------------------------------------------------
Soru 6 (Tüm farklı karakterler {a, b, c, d} kümesidir. "bcdbca" içinde "cdbc" veya "dbca" gibi parçalara bakıldığında, "dbca" (4 karakter) tüm harfleri içeren en kısa dizidir.)
Çeviri: s = "aabcbcdbca" string'inde, içindeki tüm farklı karakterleri (a, b, c, d) içeren en küçük alt dizenin uzunluğu nedir?
Cevap: B) 4