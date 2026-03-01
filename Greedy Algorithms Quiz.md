Question 1 (Huffman kodlamasında, minimum frekansa sahip iki düğümü sürekli olarak bulup birleştirmek için bir min-heap (öncelikli kuyruk) kullanılır. N eleman için yığından eleman çıkarma ve ekleme işlemleri O(\log N) sürdüğünden toplam zaman karmaşıklığı O(N \log N) olur.)
Soru: Huffman Kodlamasının zaman karmaşıklığı nedir?

Cevap: B) O(NlogN)
----------------------------------------------------------------------------------------
Question 2 (0/1 Sırt Çantası (Knapsack) problemi öğelerin bölünmesine izin vermediği için Dinamik Programlama (Dynamic Programming) kullanır. Kesirli (Fractional) versiyonu ise Greedy ile çözülür.)
Soru: Aşağıdakilerden hangisi Açgözlü (Greedy) yaklaşımı kullanmaz?

Cevap: B) 0/1 Knapsack
----------------------------------------------------------------------------------------
Question 3 (Açgözlü para üstü algoritmasında madeni paralar önce büyükten küçüğe doğru sıralanır. Bu sıralama işlemi O(n \log n) zaman alır ve algoritmanın en maliyetli adımı olduğu için genel karmaşıklığı belirler.)
Soru: Para üstü verme (coin change) problemi için açgözlü (greedy) algoritmanın zaman karmaşıklığı nedir?

Cevap: B) O(nlogn)
----------------------------------------------------------------------------------------
Question 4 (Bellman-Ford algoritması en kısa yolu bulmak için grafın tüm kenarlarını döngüler halinde tekrar tekrar hesaplar; bu Dinamik Programlama mantığıdır. Diğerleri ise o anki en iyi seçimi yapan Greedy algoritmalardır.)
Soru: Aşağıdaki standart algoritmalardan hangisi bir Açgözlü (Greedy) algoritma değildir?

Cevap: D) Bellmen Ford Shortest path algorithm
----------------------------------------------------------------------------------------
Question 5 (Olasılıklar tam olarak 2'nin negatif kuvvetleri şeklinde (mükemmel bir asimetri) dağıldığında, oluşturulan Huffman ağacı bir tarafa doğru tamamen eğik (skewed) olur ve en sık geçen harf 1 bit, en az geçenler en uzun bit dizisini alır.)
Soru: a, b, c, d, e, f harflerinin sırasıyla 1/2, 1/4, 1/8, 1/16, 1/32, 1/32 olasılıklara sahip olduğunu varsayalım. a, b, c, d, e, f harfleri için Huffman kodu aşağıdakilerden hangisidir?

Cevap: A) 0, 10, 110, 1110, 11110, 11111
----------------------------------------------------------------------------------------
Question 6 (Ortalama uzunluk, her harfin olasılığının o harfe atanan bit sayısıyla çarpılıp toplanmasıyla bulunur: 1*(1/2) + 2 *(1/4) + 3*(1/8) + 4*(1/16) + 5*1/32) + 5*(1/32) = 1.9375.)
Soru: a, b, c, d, e, f harflerinin sırasıyla 1/2, 1/4, 1/8, 1/16, 1/32, 1/32 olasılıklara sahip olduğunu varsayalım. Huffman kodlarının ortalama uzunluğu nedir?

Cevap: D) 1.9375
----------------------------------------------------------------------------------------
Question 7 (Greedy algoritması değer/ağırlık oranına göre 4, 1 ve 3. öğeleri seçer (Toplam değer: 104). Ancak optimal çözüm 1. ve 4. öğeleri seçmektir (Toplam değer: 112). Aradaki fark 112 - 104 = 8 olur.)
Soru: Toplam ağırlığı 11 kg'ı geçmeyecek ve toplam değeri maksimize edecek bir alt küme seçilmelidir (öğeler bölünemez). Optimal çözüm V_{opt} ve oran bazlı açgözlü (greedy) çözüm V_{greedy} arasındaki fark (V_{opt} - V_{greedy}) nedir?
Cevap: B) 8
----------------------------------------------------------------------------------------
Question 8 (J2 işinin son bitiş süresi 2. zaman birimidir. B şıkkındaki sıralamada J2 3. sıraya konmuştur, yani 3. zaman biriminde çalıştırılacaktır ki bu, işin teslim süresinin ihlal edilmesi (gecikmesi) demektir.)
Soru: J1, J2, J3, J4 şeklinde 4 işi ve bunlara karşılık gelen bitiş süreleri (deadline) (d1, d2, d3, d4) = (4, 2, 4, 2) olan bir iş çizelgeleme problemini düşünün. Aşağıdakilerden hangisi herhangi bir iş programını ihlal etmeyen uygun (feasible) bir çizelge değildir?

Cevap: B) J4, J1, J2, J3
----------------------------------------------------------------------------------------
Question 9 (Bütün ardışık düğümler (v1-v2, v2-v3 vb.) arasındaki fark her zaman 1'dir. 100 düğümlü bir grafı birleştirmek için 99 kenar gereklidir ve hepsi 1 ağırlıklı seçilirse toplam ağırlık 99 olur.)
Soru: V = {v_1, v_2,..., v_{100}} köşe kümesine ve $1 =< > i < j =<  > 100 olmak üzere E={(v_i, v_j)} kenar kümesine sahip bir G=(V, E) grafı düşünün. (v_i, v_j) kenarının ağırlığı |i - j|'dir. G'nin minimum yayılan ağacının (minimum spanning tree) ağırlığı nedir?

Cevap: A) 99
----------------------------------------------------------------------------------------
Question 10 (Karakterlerin frekansları a:1, b:2, c:2, d:2, e:3'tür. Bunlar için optimal bir Huffman ağacı çizildiğinde karakterlere atanan bit uzunlukları ile kendi frekansları çarpılıp toplandığında ulaşılabilecek en küçük boyut 23 bit olur.)
Soru: abbccddeee dizgisini düşünün. Dizgideki her harfe, bazı özellikleri (hiçbir kod diğerinin öneki olamaz vb.) sağlayan ikili kodlar atanacaktır. Tüm şartları sağlayan atamalara göre, kodlanmış dizginin minimum uzunluğu nedir?

Cevap: B) 23
----------------------------------------------------------------------------------------
Question 11 (7 metrelik çubuk hiç kesilmeden direkt satıldığında fiyatı 18'dir. Başka türlü kesimler (örn. 6 metrelik parça 17 ve 1 metrelik parça 1) de maksimum 18'i verir; yani elde edilebilecek en büyük kazanç 18'dir.)
Soru: Çubuk kesme problemi (Rod cutting) ile ilgili verilen p[1]=1, p[2]=5, p[3]=8, p[4]=9, p[5]=10, p[6]=17, p[7]=18 fiyat dizisine göre, 7 metrelik çubuğun maksimum kazancı R_7 hakkında hangisi doğrudur?R7=18R7=19R7, üç farklı çözümle elde edilirR7, üç parçadan oluşan bir çözümle elde edilemez

Cevap: R7=18
----------------------------------------------------------------------------------------
Question 12 (İçerme-dışlama prensibi kullanılarak aynı harflerin tekrarları çıkarıldığında, harflerin orijinal konumlarına gelmediği tamamen karışık geçerli dizilim (derangement) sayısı 12 olarak hesaplanır.)
Soru: İki L harfinin birbirinden ayırt edilemez olduğu varsayıldığında, LILAC kelimesindeki karakterlerin hiçbirinin orijinal konumunda görünmeyeceği (derangement) permütasyonların sayısı kaçtır?

Cevap: A) 12
----------------------------------------------------------------------------------------
Question 13 (Dosyalara erişim süresini optimize etmek için, Greedy mantığına uygun olarak dosyalar boyutu en küçük olandan en büyük olana doğru artan sırayla dizilmelidir (50, 80, 100, 120, 150, 200).)
Soru: Sırasıyla 100, 200, 50, 80, 120, 150 kayda sahip F1, F2, F3, F4, F5 ve F6 dosyaları vardır. Erişimi optimize etmek için hangi sırayla depolanmalıdırlar?

Cevap: A) F3, F4, F1, F5, F6, F2
----------------------------------------------------------------------------------------
Question 14 (Huffman ağacı oluşturulduğunda b:1, e:2, c:3, a:4, d:4 bitlik kodlar alır. Olasılıklar ile bit sayıları çarpılıp toplandığında ortalama kod uzunluğu (1*0.40) + (2*0.24) + (3*0.16) + (4*0.11) + (4*0.09) = 2.16 çıkar.)
Soru: Olasılıkları sırasıyla 0.11, 0.40, 0.16, 0.09 ve 0.24 olan a, b, c, d, e karakterlerinden oluşan bir metnin, optimal Huffman kodlama tekniğiyle ortalama uzunluğu ne olur?

Cevap: B) 2,16
----------------------------------------------------------------------------------------
Question 15 (Prim algoritması her zaman mevcut ağaca bağlı en düşük ağırlıklı kenarı seçer. A'dan sonra en küçük kenar 7 ile (A,D), sonra 10 ile (A,B), sonra 22 ile (D,F) şeklinde devam eden sıra D şıkkıdır.)
Soru: A düğümünden başlayarak Prim algoritması ile minimum yayılan ağaç oluşturulurken kenarlar hangi sırayla eklenebilir?

Cevap: D) (A, D), (A, B), (D, F), (F, C), (F, G), (G, E)
----------------------------------------------------------------------------------------
Question 16 (Algoritma belirli bir başlangıç (kaynak) noktasından başlayarak diğer tüm düğümlere giden en düşük maliyetli rotaları bulduğu için bu isimle bilinir.)
Soru: Dijkstra algoritmasının diğer adı nedir?

Cevap: A) single-source shortest path problem (Tek kaynaklı en kısa yol problemi)
----------------------------------------------------------------------------------------
Question 17 (Huffman kodları bir "Önek Kodu" (Prefix Code) sistemidir. Atanan hiçbir ikili kod, başka bir kodun başlangıç kısmıyla eşleşmez. Bu, verinin kayıpsız ve hatasız bir şekilde geri çözülmesini garanti eder.)
Soru: Huffman Kodlaması hakkında aşağıdakilerden hangisi doğrudur?

Cevap: C) In Huffman coding, no code is prefix of any other code.
----------------------------------------------------------------------------------------
Question 18 (Belirtilen optimal veri yapıları (Min-Heap ve Union-Find) kullanıldığında, her iki algoritma da en kötü durumda graf kenarlarını ve düğümlerini benzer oranda tarar ve zaman karmaşıklıkları O(E \log V) olur.)
Soru: Kruskal ve Prim MST algoritmaları hakkında hangisi doğrudur? (Prim'in Binary Heap ile, Kruskal'ın Union by Rank ile uygulandığını varsayarak)

Cevap: A) Her iki algoritmanın da en kötü durum (worst case) zaman karmaşıklığı aynıdır.
----------------------------------------------------------------------------------------
Question 19 (Bu tür sorular, önceden oluşturulmuş bir Huffman ağacındaki harf atamalarını yan yana birleştirmeyi gerektirir. (Örn: d-e-a-d sırasındaki bitler arka arkaya eklenir).)
Soru: 2. soruda (Not: Burada soru bankasının diğer sorularına atıf var, a, b, c, d, e, f harfli örneği kasteder), "dead" kelimesini hangisi temsil eder?

A) 1011111100101
B) 0100000011010
C) Both A and B
D) None of these
Cevap: (Test bankasının bağlamına göre değişir ancak genellikle Soru 5'teki değerlerle C veya ilgili özel tablodan çözülür)
----------------------------------------------------------------------------------------
Question 20 (Toplam 100 karakter sıkıştırılmadan önce 800 bit yer kaplar. Huffman kodlaması yapıldığında, yüksek frekanslılara az bit verilerek toplam mesaj boyutu 224 bite düşürülür. Elde edilen tasarruf 800 - 224 = 576 bittir.)
Soru: Bir ağ şirketi mesajları Huffman kodlamasıyla sıkıştırmaktadır. (a:5, b:9, c:12, d:13, e:16, f:45). Her karakter başlangıçta 1 bayt (8 bit) alıyorsa, mesajda kaç bit tasarruf edilecektir?

Cevap: C) 576
----------------------------------------------------------------------------------------
Question 21 (Bu soru, Soru 4'ün varyasyonudur. Bellman-Ford, tüm durumu adım adım değerlendiren ve geri dönüşlere açık olan Dinamik Programlama prensibiyle çalışır; Greedy değildir.)
Soru: Aşağıdaki standart algoritmalardan hangisi bir Açgözlü (Greedy) algoritma değildir?

Cevap: E) Bellmen Ford Shortest path algorithm
----------------------------------------------------------------------------------------
Question 22 (Dijkstra her zaman o anki en kısa mesafeye sahip düğümü seçer. P(0)'den sonra Q(1), Q'dan sonra R(2), R'den sonra U(3), sonra S(4 veya 5) ve en son T şeklinde ilerleyen sıra B şıkkıdır.)
Soru: P düğümü kaynak olmak üzere Dijkstra algoritması çalıştırıldığında, düğümler hangi sırada en kısa yol mesafeleri kesinleşmiş olarak kümeye dahil edilir?

Cevap: B) P, Q, R, U, S, T