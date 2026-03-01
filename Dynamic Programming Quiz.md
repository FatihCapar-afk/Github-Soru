Question 1 (Memoization, daha önce çözülen alt problemlerin sonuçlarını saklar. Böylece her alt problem sadece bir kez çözülür ve çözüm süresi alt problem sayısına (genellikle doğrusal) düşer.)
Soru: Dinamik programlamada, örtüşen alt problemlerin (overlapping subproblems) olduğu bir problemi memoization (not tutma) kullanarak çözmenin zaman karmaşıklığı nedir?

Cevap: C) O(n)
----------------------------------------------------------------------------------------
Question 2 (Verilen bir metnin, belirli bir sözlükteki kelimelerin birleşimiyle oluşturulup oluşturulamayacağını kontrol eden bir problemdir.)
Soru: "Word Break Problem"ın (Kelime Bölme Problemi) temel amacı nedir?

Cevap: B) To determine if a string can be segmented into a sequence of words from a dictionary.
----------------------------------------------------------------------------------------
Question 3 (Partition problem, bir sayı kümesini toplamları eşit iki alt kümeye bölmeye çalışır. Bu, aslında hedef toplamın tüm sayıların toplamının yarısı olduğu bir "Alt Küme Toplamı" (Subset Sum) problemidir.)
Soru: "Partition Problem" (Bölme Problemi) hangi iyi bilinen probleme indirgenebilir?

Cevap: C) Subset Sum Problem
----------------------------------------------------------------------------------------
Question 4 (Bu problemde her yumurta ve her kat için deneme yapılırken, o kattan altındaki ve üstündeki tüm olasılıklar taranır. Bu da O(K*N*N) karmaşıklığına yol açar.)
Soru: "Egg Dropping Puzzle"da (Yumurta Bırakma Bilmecesi), $K$ yumurta ve $N$ kat için dinamik programlama yaklaşımının zaman karmaşıklığı nedir?

evap: C) O(K * N^2)
----------------------------------------------------------------------------------------
Question 5 (Standart DP çözümünde her eleman (i), kendinden önceki tüm elemanlarla (j < i) karşılaştırılır. Bu da iç içe iki döngü gerektirir (O(n^2)). Not: O(n \log n) çözümü de mevcuttur ancak temel DP sorulmaktadır.)
Soru: n uzunluğundaki bir dizi için "Longest Increasing Subsequence" (LIS - En Uzun Artan Alt Dizi) probleminin standart dinamik programlama yaklaşımıyla zaman karmaşıklığı nedir?

Cevap: C) O(n^2)
----------------------------------------------------------------------------------------
Question 6 (Her iki problem de belirli bir hedef toplama ulaşmak için verilen sayı kümesinin kombinasyonlarını kullanmayı hedefler.)
Soru: Aşağıdaki problemlerden hangisi "Subset Sum" (Alt Küme Toplamı) problemiyle yakından ilişkilidir ve dinamik programlama ile çözülebilir?

Cevap: C) Coin Change Problem
----------------------------------------------------------------------------------------
Question 7 (Bir dizginin en uzun palindromik alt dizisi, o dizgi ile onun tersi arasındaki "En Uzun Ortak Alt Dizi"dir (LCS).)
Soru: "LPS" (Longest Palindromic Subsequence) problemiyle yakından ilişkili olan ve DP ile çözülebilen problem hangisidir?

Cevap: A) Longest Common Subsequence Problem
----------------------------------------------------------------------------------------
Question 8 (0-1 Knapsack probleminde eşyalar bölünemez. Eğer eşya sığmıyorsa o eşya atlanır ve kapasite değişmeden bir sonraki eşyaya geçilir.)
Soru: "0-1 Knapsack" (0-1 Sırt Çantası) probleminde, bir eşyanın ağırlığı çantanın kalan kapasitesinden büyükse ne yapılır?

Cevap: A) Ignore the item and move to the next one
----------------------------------------------------------------------------------------
Question 9 (Algoritma, eşya sayısı ($n$) ve çanta kapasitesi ($W$) boyutunda bir tablo doldurur, bu yüzden karmaşıklık O(n*W) olur.)
Soru: Tabulation (aşağıdan yukarıya) yöntemiyle "0-1 Knapsack" problemini çözmenin zaman karmaşıklığı nedir?

Cevap: C) O(n * capacity)
----------------------------------------------------------------------------------------
Question 10 (Soru 5 ile aynıdır; her eleman için geçmişe bakıldığı için O(n^2)'dir.)
Soru: "LIS" (Longest Increasing Subsequence) probleminin DP yaklaşımı için zaman karmaşıklığı nedir?

Cevap: C) O(n^2)
----------------------------------------------------------------------------------------
Question 11 (DP, üstel karmaşıklıktaki kaba kuvvet (brute force) çözümlerini, sonuçları saklayarak polinom zamanlı (örneğin
O(n^2)) çözümlere indirger.)
Soru: Dinamik programlama, özellikle üstel (exponential) zaman karmaşıklığına sahip problemlerin çözümünde yararlıdır.

Cevap: A) True
----------------------------------------------------------------------------------------
Question 12 (Kod en uzun artan alt diziyi bulur. Bu dizide artan alt dizi {3, 10, 20} şeklindedir ve uzunluğu 3'tür.)
Soru: n=5 ve arr[] = {3, 10, 2, 1, 20} için aşağıdaki kodun çıktısı ne olur?

function(arr):
    n = len(arr)
    lis = [1] * n
    for i in range(1, n):
        for j in range(i):
            if arr[i] > arr[j] and lis[i] < lis[j] + 1:
                lis[i] = lis[j] + 1
    return max(lis)
Cevap: D) 3
----------------------------------------------------------------------------------------
Question 13 (Alt problemlerin çözümlerini bir hafızada (genelde bir tablo veya hash map) saklayıp, aynı problemle tekrar karşılaşıldığında doğrudan oradan okuma tekniğidir.)
Soru: Dinamik programlama bağlamında "memoization" nedir?

Cevap: B) A way to avoid solving subproblems by storing their solutions and reusing them.
----------------------------------------------------------------------------------------
Question 14 (DP hem Memoization (yukarıdan aşağıya) hem de Tabulation (aşağıdan yukarıya - Bottom-Up) yöntemleriyle çözülebilir.)
Soru: Dinamik programlama problemlerini çözmek için kullanılan farklı teknikler nelerdir?

Cevap: C) Both
----------------------------------------------------------------------------------------
Question 15 (İki dizgi arasındaki farkları bulmak için kullanılan Edit Distance, LCS mantığına dayanır ve ekleme, silme, değiştirme işlemlerini maliyetlendirir.)
Soru: "Edit Distance" algoritması hangi DP problemi yardımıyla çözülebilir?

Cevap: A) Longest Common Subsequence (LCS)
----------------------------------------------------------------------------------------
Question 16 (Bir problemin DP ile çözülebilmesi için en uygun alt yapıya (optimal substructure) ve tekrar eden/üst üste binen alt problemlere (overlapping subproblems) sahip olması şarttır.)
Soru: Ne zaman dinamik programlama yaklaşımını kullanırız?

Cevap: B) The solution has optimal substructure and overlapping subproblems
----------------------------------------------------------------------------------------
Question 17 (Basit özyineleme her adımda iki yeni çağrı yapar, bu da bir ağaç gibi büyüyerek üstel (O(2^n)) bir karmaşıklığa yol açar.)
Soru: Fibonacci dizisinin kaba kuvvet (naive recursive) uygulamasının zaman karmaşıklığı nedir?

Cevap: D) O(2^n)
----------------------------------------------------------------------------------------
Question 18 (Eğer mevcut karakterler eşleşmiyorsa (X[i-1] != Y[j-1]), bir karakteri bir diziden veya diğerinden eksilterek elde edilen en büyük uzunluk seçilir.)
Soru: LCS probleminde l(i,j) uzunluğu için aşağıdaki özyinelemeli tanımda eksik olan ifadeler nedir?

Cevap: C) expr2 ≡ max(l(i-1, j), l(i, j-1))
----------------------------------------------------------------------------------------
Question 19 (Prim algoritması bir Greedy (Açgözlü) algoritmadır. Diğerleri (Bellman-Ford, Floyd-Warshall, 0-1 Knapsack) DP kullanır.)
Soru: Aşağıdaki standart algoritmalardan hangisi Dinamik Programlama tabanlı değildir?

Cevap: D) Prim's Minimum Spanning Tree
----------------------------------------------------------------------------------------
Question 20 (j toplamına ulaşmak için ya bir önceki elemanla zaten ulaşılmış olmalıdır (X[i-1, j]) ya da mevcut eleman çıkarıldığında kalan toplama ulaşılabiliyor olmalıdır (X[i-1, j-ai]).)
Soru: "Subset-sum" probleminde a_i =< > j =<> W durumu için hangi ifade geçerlidir?

Cevap: B) X[i, j] = X[i - 1, j] ∨ X[i - 1, j - ai]
----------------------------------------------------------------------------------------
Question 21 (Matris zinciri çarpımı (Matrix Chain Multiplication) algoritmasıyla en uygun gruplandırma yapıldığında (örneğin ((M_1*(M_2*M_3))*M_4)) 19.000 işlem sonucuna ulaşılır.)
Soru: p=10, q=100, r=20, s=5, t=80 boyutlarındaki 4 matrisin çarpımı için gereken minimum skaler çarpım sayısı nedir?

Cevap: C) 19000
----------------------------------------------------------------------------------------
Question 22 (Bu dizgiler için LCS uzunluğu x=4 ve bu uzunlukta 3 farklı dizgi (y=3) vardır. 4 + (10*3) = 34.)
Soru: A = "qpqrr" ve B = "pqprqrp" dizgileri için en uzun ortak alt dizi uzunluğu x ve bu uzunluktaki farklı alt dizi sayısı y ise x + 10y kaçtır?

Cevap: D) 34
----------------------------------------------------------------------------------------
Question 23 (Subset sum problemi üstel zamanlı bir problem olsa da DP ile psödo-polinom zamanda çözülebilir.)
Soru: Verilen bir kümede toplamı K olan bir alt küme olup olmadığını en kısa sürede belirlemek için hangi yöntem kullanılır?

Cevap: B) Dynamic Programming
----------------------------------------------------------------------------------------
Question 24 (F(0)=1, F(1)=1. F(2) = 10(1) + 100(1) = 110. F(3) = 10(110) + 100(1) = 1200.)
Soru: F_{00}(0)=1, F_{00}(1)=1 ve n -> 2 için F_{00}(n) = 10*F_{00}(n-1) + 100*F_{00}(n-2) ise dizinin değerleri nelerdir?

Cevap: A) (1, 110, 1200)
----------------------------------------------------------------------------------------
Question 25 (En uygun parantezleme ile hesaplandığında (genelde en küçük ortak boyutları merkeze alarak) 1500 çarpım yapılır.)
Soru: 10*5, 5*20, 20*10 ve 10*5 boyutlu matrislerin çarpımı için gereken minimum skaler çarpım sayısı nedir?

Cevap: A) 1500
----------------------------------------------------------------------------------------
Question 26 (Memoization (top-down), özyinelemeli çağrılar ve sonuçları saklamak için ek bellek (stack space + table) kullanır ancak zaman karmaşıklığını ciddi oranda düşürür.)
Soru: Dinamik programlamada yukarıdan aşağıya (top-down) yaklaşım uygulandığında ne olur?

Cevap: B) It increases the space complexity and decreases the time complexity.
----------------------------------------------------------------------------------------
Question 27 (Bellman-Ford O(V*E) sürer. Tam bir grafta kenar sayısı (E) yaklaşık n^2 olduğu için toplam karmaşıklık n*n^2 = n^3 olur.)
Soru: n köşeli tam bir graf üzerinde Bellman-Ford algoritmasının zaman karmaşıklığı nedir?

Cevap: C) θ(n3)
----------------------------------------------------------------------------------------
Question 28 (DP problemleri sadece ardışık (sıralı) çözmek değil, karmaşık alt problemlerin birleşimiyle çözmekle ilgilidir. A, B ve D şıkları DP'nin temel özellikleridir.)
Soru: Aşağıdakilerden hangisi dinamik programlamanın bir özelliği değildir?

Cevap: C) Solving problems in a sequential manner.
----------------------------------------------------------------------------------------
Question 29 (Verilen matematiksel ifade, problemin çözümünü daha küçük alt problemlerin (Li+1) sonuçlarını kullanarak inşa etmektedir. Bu durum, dinamik programlama yaklaşımının (memoization veya tabulation) temel özelliğidir.)
Soru: Bir dizideki en uzun monoton artan dizinin uzunluğunu bulan algoritma verilmiştir. Hangisi doğrudur?

Cevap: A) The algorithm uses dynamic programming paradigm