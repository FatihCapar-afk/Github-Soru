Question 1 (Seyrek (sparse) graflarda komşuluk listesi sadece var olan kenarları sakladığı için bellekten tasarruf sağlar ve dolaşım sırasında boş hücreleri taramak zorunda kalmaz; bu da onu matris yöntemine göre çok daha verimli kılar.)
Soru: Çok iyi bağlantılı (well-connected) olmayabilecek genel bir graf için BFS ve DFS dolaşımlarını verimli bir şekilde temsil etmek amacıyla aşağıdakilerden hangisi tercih edilir?

Cevap: B) Adjacency List
----------------------------------------------------------------------------------------
Question 2 (Kenar sayısı ile köşe sayısı arasındaki bu ilişki bir "Ağaç" (Tree) yapısının temel özelliğidir. Döngüsüz ve bağlı her grafta kenar sayısı her zaman köşe sayısının bir eksiğidir (e = v - 1).)
Soru: v adet köşesi (vertex) ve e adet kenarı (edge) olan, bağlı ve döngüsüz (no cycles) bir G grafı için aşağıdakilerden hangisi doğrudur?

Cevap: B) v = e+1
----------------------------------------------------------------------------------------
Question 3 (BFS katman katman ilerlediği için, ağırlıksız graflarda bir düğüme ulaştığı an o düğüme giden en kısa yolu (en az kenar sayısını) bulmuş olur.)
Soru: Ağırlıksız, bağlı ve yönsüz bir grafın (belirli bir kaynaktan) BFS dolaşımı hakkında aşağıdakilerden hangisi doğrudur?

Cevap: A) The paths found in the BFS traversal are the shortest paths from source to every other vertex
----------------------------------------------------------------------------------------
Question 4 (DFS dolaşımında her köşe bir kez ziyaret edilir ve her kenar komşuluk listesi üzerinden bir kez taranır, bu nedenle toplam süre köşe ve kenar sayısının toplamı kadardır.)
Soru: Komşuluk listesi olarak temsil edilen bir grafın DFS dolaşımının zaman karmaşıklığı nedir? (V köşe, E kenar sayısıdır).

Cevap: A) O(V + E)
----------------------------------------------------------------------------------------
Question 5 (Yönsüz graflarda bir düğümden geldiğiniz ebeveyne geri dönmek döngü sayılmaz; ancak ebeveyn olmayan ve daha önce ziyaret edilmiş bir düğüme rastlamak grafın kapandığını ve bir döngü oluştuğunu gösterir.)
Soru: Yönsüz bir grafta DFS kullanarak döngü (cycle) nasıl tespit edilir?

Cevap: B) If current vertex has an adjacent that is already visited and is not parent (in DFS Tree) of the current vertex, then there is a cycle.
----------------------------------------------------------------------------------------
Question 6 (Graf kopuk olsa bile, her bileşen için BFS çalıştırıldığında toplamda yine tüm köşeler ve tüm kenarlar birer kez işlenir; bu yüzden karmaşıklık değişmez.)
Soru: Bağlantılı olmayabilen (disconnected) bir grafın tam BFS dolaşımının zaman karmaşıklığı nedir? (Graf komşuluk listesi ile temsil edilmektedir).

Cevap: A) O(V + E)
----------------------------------------------------------------------------------------
Question 7 (Dijkstra algoritması her zaman en yakın (en küçük maliyetli) düğümü seçerek ilerlediği için, bu işlemi en hızlı yapan yapı "Min-Priority Queue"dur (genelde bir Min-Heap ile uygulanır).)
Soru: Dijkstra Algoritmasını uygulamak için en yaygın kullanılan veri yapısı hangisidir?

Cevap: D) Min priority queue
----------------------------------------------------------------------------------------
Question 8 (Her kenar için öncelikli kuyrukta bir güncelleme yapılması ($E$) ve bu kuyruğun her seferinde yeniden düzenlenmesi (\log V) gerektiği için karmaşıklık bu şekildedir.)
Soru: Komşuluk listesi ile temsil edilen bir graf için Dijkstra algoritmasının zaman karmaşıklığı nedir?

Cevap: A) O(E Log V)
----------------------------------------------------------------------------------------
Question 9 (Topolojik sıralama öncelik ilişkilerini takip eder; üzerinde hiçbir bağımlılık olmayan (giriş derecesi 0 olan) düğümler ilk sırada işlenmeye en uygun adaylardır.)
Soru: Çoğu durumda, topolojik sıralama (topological sort) hangi düğümden başlar?

Cevap: D) Zero Degree (In-degree Zero)
----------------------------------------------------------------------------------------
Question 10 (Topolojik sıralama, DFS (bitiş zamanlarına göre) veya BFS tabanlı Kahn algoritması kullanılarak başarılı bir şekilde uygulanabilir.)
Soru: Topolojik sıralama hangisi kullanılarak uygulanabilir?

Cevap: C) Using Depth or Breadth First Search