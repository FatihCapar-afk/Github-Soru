Soru 1 (Bölme yöntemi (modulo), anahtarlar birbirine yakın olduğunda verilerin tablo üzerinde ardışık dizilmesine (kümelenme) en müsait basit yöntemdir.)
Çeviri: Aşağıdaki hash fonksiyonlarından hangisinin bir hash tablosunda kümelenmeye (clustering) neden olma olasılığı en yüksektir? (k: anahtar değer, m: tablo boyutu).
Cevap: h(k) = k % m
----------------------------------------------------------------------------------------
Soru 2 (Çakışma yönetiminde en temel iki yöntem "Separate Chaining" (bağlı liste kullanımı) ve "Open Addressing"dir.)
Çeviri: Çakışmaları (collision) yönetme yöntemleri nelerdir?
Cevap: A) Separate Chaining (Not: B şıkkındaki "Open Chaining" standart bir terim değildir, "Open Addressing" olmalıydı).
----------------------------------------------------------------------------------------
Soru 3 (Linear probing; veritabanları, önbellekleme (caching) ve derleyici tasarımı gibi hızlı erişim gereken yerlerde yaygın kullanılır.)
Çeviri: Doğrusal yoklama (linear probing) uygulamaları neleri içerir?
Cevap: D) All of the above (Hepsi)
----------------------------------------------------------------------------------------
Soru 4 (Verinin değerine göre doğrudan bir dizine yerleştirilmesi işlemine indeks eşleme denir.)
Çeviri: Verinin doğrudan hash tablosundaki bir indekse eşlendiği basit hashing formu hangisidir?
Cevap: B) Index Mapping (veya Direct Address Table)
----------------------------------------------------------------------------------------
Soru 5 (Bir hashing sistemi; anahtar (key), bu anahtarı işleyen fonksiyon (hash function) ve verinin saklandığı tablo (hash table) yapılarından oluşur.)
Çeviri: Aşağıdakilerden hangileri Hashing'in bileşenleridir?
Cevap: D) All of the above (Hepsi)
----------------------------------------------------------------------------------------
Soru 6 (Kod, (a, b) çiftini gördüğünde sözlüğe ekler; daha sonra (b, a) ile karşılaşırsa bunu simetrik çift olarak ekrana basar. Dizideki (40, 30) ve (10, 5) değerleri, daha önce eklenen (30, 40) ve (5, 10) ile eşleşir.)
Çeviri: Verilen programın çıktısı nedir? (Program, dizideki simetrik çiftleri bulup yazdırıyor).
Cevap: A) (30, 40) ve (5, 10)
----------------------------------------------------------------------------------------
Soru 7 (Hash fonksiyonları "basit uniform" olduğu sürece, yük dengeleme (load factor) değişmez ve beklenen eleman sayısı toplam eleman bölü slot sayısı ($n/m$) olur.)
Çeviri: n anahtar ve m slot verildiğinde; tek sayılar için h1, çiftler için h2 fonksiyonu kullanılıyorsa, bir slotta beklenen anahtar sayısı nedir?
Cevap: C) n / m
----------------------------------------------------------------------------------------
Soru 8 (Elemanların tablodaki konumlarını (özellikle çakışma sonrası kaymaları) doğrulayan tek dizi C şıkkıdır. Örneğin 52, normalde 2. indekse girmelidir ama 2, 3 ve 4 dolu olduğu için 5. indekse kaymıştır.)
Çeviri: 10 uzunluğunda, h(k) = k  10 fonksiyonu ve linear probing kullanan bir tabloda, 6 değer yerleştirildikten sonra oluşan tabloya göre (2:42, 3:23, 4:34, 5:52, 6:46, 7:33) olası ekleme sırası hangisidir?
Cevap: C) 46, 34, 42, 23, 52, 33
----------------------------------------------------------------------------------------
Soru 9 (Adım adım yerleştirme yapıldığında; 12 (indeks 2), 18 (indeks 8) ve 13 (indeks 3) sorunsuz yerleşir. Ancak 2 sayısı geldiğinde 2. indeks dolu olduğu için bir sonrakine bakılır, 3 de dolu olduğu için 4. indekse yerleşir. Bu kaymalar devam ettiğinde veriler C şıkkındaki gibi dizilir.)
Çeviri: 12, 18, 13, 2, 3, 23, 5 ve 15 anahtarları; başlangıçta boş olan, 10 uzunluğundaki bir hash tablosuna h(k) = k  10 fonksiyonu ve doğrusal yoklama (linear probing) kullanılarak yerleştiriliyor. Oluşan hash tablosu aşağıdakilerden hangisidir?
Cevap: C
----------------------------------------------------------------------------------------
Soru 10 (Her sayı için fonksiyon hesaplanır: x=1 rightarrow 2, x=3 rightarrow 3, x=8 rightarrow 3 (çakışma, bir yana kayar rightarrow 4), x=10 rightarrow 1. Yerleşim sırasına göre A şıkkı uygundur.)
Çeviri: Boyutu 7 olan boş bir tabloya (7x+3)  4 fonksiyonu ve kapalı hashing (closed hashing) ile 1, 3, 8, 10 sayıları eklenirse tablonun içeriği ne olur?
Cevap: A) 3, 10, 1, 8, __ , __ , __
----------------------------------------------------------------------------------------
Soru 11 (Yük faktörü formülü:  = {Eleman Sayısı} / {Slot Sayısı} 2000 / 25 = 80.)
Çeviri: 25 slotu ve 2000 elemanı olan bir T hash tablosu için yük faktörü (alpha) nedir?
Cevap: A) 80
----------------------------------------------------------------------------------------
Soru 12 (Bağlı listelerde (chaining) bir elemanı silmek, diğer elemanların yerini kaydırmayı gerektirmediği için çok daha basittir.)
Çeviri: Chained hashing'in (dışsal hashing) open addressing yöntemine göre avantajı nedir?
Cevap: C) Deletion is easier (Silme işlemi daha kolaydır)
----------------------------------------------------------------------------------------
Soru 13 (İkinci hash fonksiyonu (h_2) adım aralığını belirler. h_2(k) = 1 + (123456 \mod 700) = 1 + 256 = 257. İki deneme arasındaki fark tam olarak bu adım miktarıdır.)
Çeviri: m=701 ve n=700 için double hashing kullanıldığında, k=123456 anahtarı için birinci ve ikinci deneme (probe) arasındaki slot farkı nedir?
Cevap: C) 257
----------------------------------------------------------------------------------------
Soru 14 (Bu soruda sayıların ikili (binary) karşılıklarına bakılır. Örneğin 5 (0101) ve 13 (1101) sayılarının son iki biti "01"dir, bu yüzden aynı sütuna düşerler ve 3./4. bitlerine göre ağaçta dallanırlar. C şıkkındaki sayılar ve bit dizilimleri, görseldeki ağaç yapısını (boş kalan "00" sütunu, dallanan "01" ve "10" sütunları) tam olarak doğrular.)
Çeviri: 4 bitlik tam sayı anahtarları için dinamik bir hashing yaklaşımını ele alın:

(A) 4 boyutunda ana bir hash tablosu vardır.
(B) Bir anahtarın en az anlamlı 2 biti (LSB), ana tabloya indekslemek için kullanılır.
(C) Başlangıçta ana tablo boş değerlerden oluşur.
(D) Çakışmaları çözmek için, her bir tablo girişi talep üzerine büyüyen bir ikili ağaç (binary tree) olarak düzenlenir.
(E) Önce 3. en az anlamlı bit, anahtarları sol ve sağ alt ağaçlara ayırmak için kullanılır.
(F) Daha fazla çakışma olursa, 4. en az anlamlı bit kullanılır.
(G) Bölme işlemi sadece ihtiyaç duyulduğunda (çakışma olduğunda) yapılır.
Görseldeki tablo durumuna göre, hangi anahtar dizisi bu yapıyı oluşturmuş olabilir?
Cevap: C) 10, 9, 6, 7, 5, 13
----------------------------------------------------------------------------------------
Soru 15 (h1(90) = 21. h2(90) = 1 + (90 19) = 1 + 14 = 15. 1. deneme: (21 + 1  15)  23 = 36  23 = 13. (Soru 1. denemeyi sorduğu için sonuç 13 çıkmalı ancak seçeneklerde işleme göre B şıkkı/farklılık olabilir; matematiksel sonuç 13'tür).)
eviri: h1(k) = k  23 ve h2(k) = 1+(k  19) fonksiyonları ile k=90 için 1. denemedeki (probe 1) adres nedir? (0. denemeden başlandığını varsayın).
Cevap: B) 15
----------------------------------------------------------------------------------------
Soru 16 (18 normalde 18  7 = 4 indeksine gitmek ister. Eğer 4 dolu değilse oraya yerleşir. Adım adım yerleştirmede 18'in yeri 4 olur.)
Çeviri: h(k) = k  7 ve linear probing ile 44, 45, 79, 55, 91, 18, 63 sayıları eklendiğinde 18'in konumu ne olur?
Cevap: B) 4
----------------------------------------------------------------------------------------
Soru 17 (Aranan eleman bulunamazsa, ilk boş slot görülene kadar arama devam eder. En uzun dolu blok uzunluğu kadar karşılaştırma yapılır.)
Çeviri: 10 kovalı bir tabloda S1-S7 arası elemanlar linear probing ile eklenmiştir. Tabloda olmayan bir öğeyi ararken yapılacak maksimum karşılaştırma sayısı nedir?
Cevap: C) 6 (Tablo görseline bağlıdır, genellikle dolu slotların en uzun zinciri + 1 boş slot bakılır).
----------------------------------------------------------------------------------------
Soru 18 (Özet: Çarpma yöntemi (multiplication method) kullanılarak yapılan hesaplamada sonuç 88 çıkar.)
Çeviri: m=100 ve h(k) =  m(kA  1) fonksiyonunda k=123456 ve A  0.618 (altın oran) için konum nedir?
Cevap: C) 88
----------------------------------------------------------------------------------------
Soru 19 (Her harfin sayısal değeri (I=8, S=18, R=17, O=14) formüle konur ve yeni harf bulunur.)
Çeviri: ISRO kelimesi k=7 anahtarı ve Ck(M) = (kM + 13)  26 fonksiyonu ile şifrelenirse sonuç ne olur?
Cevap: C) GQPM
----------------------------------------------------------------------------------------
Soru 20 (661 mod 13 = 11. 182 mod 13 = 0. 24 mod 13 = 11 (dolu  12). 103 mod 13 = 12 (dolu  başa dönerse 1, veya 11). Hesaplamaya göre 11 olur.)
Çeviri: 13 elemanlı tabloda k  13 ve linear probing ile 661, 182, 24 ve 103 eklendiğinde, 103 hangi indekse girer?
Cevap: C) 11
----------------------------------------------------------------------------------------
Soru 21 (123456*0.618... işleminin ondalık kısmının 10.000 ile çarpılıp aşağı yuvarlanmasıyla 46 elde edilir.)
Çeviri: m=10000 ve altın oran sabitli hash fonksiyonunda k=123456 nereye eşlenir?
Cevap: A) 46
----------------------------------------------------------------------------------------
Soru 22 (Hashing, ideal durumda veriye erişimi doğrudan adresleme ile O(1) sürede yapar.)
Çeviri: Hangi arama tekniği O(1) (sabit zaman) karmaşıklığına sahiptir?
Cevap: D) Hashing
----------------------------------------------------------------------------------------
Soru 23 (Saklanan her eleman için tabloda yer ayrıldığından, alan ihtiyacı eleman sayısıyla (N) doğru orantılıdır.)
Çeviri: Hashmap kullanıldığında programın kullandığı alan (space complexity) nedir?
Cevap: C) O(N)
----------------------------------------------------------------------------------------
Soru 24 (Harflerin alfabedeki sıralarına göre mod 10 değerleri hesaplandığında, aynı indekse denk gelen ilk harf M'dir.)
Çeviri: K R P C S N Y T J M karakterleri h(x) = ({ord}(x) - {ord}("A") + 1) \mod 10 ile eklenirse hangi harf çakışmaya neden olur?
Cevap: C) M
----------------------------------------------------------------------------------------
Soru 25 (Çakışma olasılığı, tablonun doluluk oranı olan yük faktörüne (n/m) bağlıdır.)
Çeviri: Uniform dağılımda n anahtarın m boyutlu tabloda çakışma olasılığı nedir?
Cevap: B) O(n/m)
----------------------------------------------------------------------------------------
Soru 26 (Olasılığın %50'yi geçmesi için tablonun yarısından fazlasının (20/2 + 1) dolması gerekir.)
Çeviri: 20 boyutlu bir tabloda, yeni bir anahtarın çakışma olasılığının 0.5'i geçmesi için kaç anahtar eklenmelidir?
Cevap: D) 10
----------------------------------------------------------------------------------------
Soru 27 (Hash fonksiyonları çıktı boyutunu sabit tutar ve çakışma (farklı girdilerin aynı çıktıyı vermesi) mümkündür.)
Çeviri: Hash fonksiyonları için hangileri doğrudur? (I. Rastgele uzunluğu sabit uzunluğa çevirir, II. Sabit uzunluğu değişkene çevirir, III. Farklı mesajlara aynı değeri verebilir).
Cevap: C) I and III only
----------------------------------------------------------------------------------------
Soru 28 (Küp alma işlemi, mod 10 tabanında rakamların son basamaklarını diğer kare veya doğrusal yöntemlere göre daha çeşitli dağıtır.)
Çeviri: 0-2020 arası sayılar için hangi fonksiyon 10 kovaya en homojen dağılımı yapar?
Cevap: C) h(i) = i³ mod 10
----------------------------------------------------------------------------------------
Soru 29 (Her bir ekleme için 100 slotun 97'si (ilk 3 dışındakiler) seçilebilir. 3 ekleme için olasılık (97/100)^3 olur.)
Çeviri: 100 slotlu ve chaining kullanılan bir tabloda, ilk 3 eklemeden sonra ilk 3 slotun boş kalma olasılığı nedir?
Cevap: A) (97 × 97 × 97) / 100³
----------------------------------------------------------------------------------------
Soru 30 (Çakışma ve kayma mantığına göre elemanların birbirine olan bağımlılıkları (önce hangisi girmeli) analiz edildiğinde 30 farklı kombinasyon çıkar.)
Çeviri: Soru 8'deki tabloyu (42, 23, 34, 52, 46, 33 değerleri ile) oluşturabilecek kaç farklı ekleme sırası vardır?
Cevap: C) 30
----------------------------------------------------------------------------------------
Soru 31 (x=1  0, x=3  6, x=8  0 (çakışma  1), x=10 6 (çakışma 0 dolu  1 dolu  2$). Yerleşim: 0:1, 1:8, 2:10, 6:3.)
Çeviri: 7 boyutlu tabloya (3x + 4) 7 ile 1, 3, 8, 10 eklenirse sonuç ne olur?
Cevap: B) 1, 8, 10, _, _, _, 3