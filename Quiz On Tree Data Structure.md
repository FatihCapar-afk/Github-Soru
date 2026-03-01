Question 1 (İfade ağacında post-order dolaşım "Sol-Sağ-Kök" sırasını izler; bu sıralama aynı zamanda ifadenin "Postfix" (Reverse Polish Notation) gösterimidir.)
Soru: (7-(4*5))+(9/3) ifadesi için aşağıdakilerden hangisi post-order ağaç dolaşımı (traversal) sonucudur?

*Cevap: C) 745-93/+**
----------------------------------------------------------------------------------------
Question 2 (Bir kuyruk (Queue) kullanarak düğümleri katman katman (yukarıdan aşağıya, soldan sağa) gezme işlemi "Level Order" dolaşımıdır.)
Soru: Aşağıdaki sözde kod (pseudo code) hangi ağaç dolaşımına aittir?
order(node)
Q → Queue()
Q.push(node)
while !Q.empty():
    current_node = Q.pop()
    print current_node.value
if current_node.left is not NULL:
    Q.push(current_node.left)
if current_node.right is not NULL:
    Q.push(current_node.right)

Cevap: A) Level order
----------------------------------------------------------------------------------------
Question 3 (Önce sol alt ağacı ziyaret eden, sonra kök düğümü yazdıran ve en son sağ alt ağaca giden bu yapı "In-order" (Sol-Kök-Sağ) dolaşımıdır.)
Soru: Aşağıdaki sözde kod hangi ağaç dolaşımını göstermektedir?
Order(node):
  if node is not null:
   Order(node.left)
  print node.value
    Order(node.right)

Cevap: A) In-order
----------------------------------------------------------------------------------------
Question 4 (Hangi düğümün yaprak olduğunu anlamak için ağaçtaki tüm düğümleri en az bir kez ziyaret etmek gerekir, bu da doğrusal zaman karmaşıklığı (O(n)) oluşturur.)
Soru: n düğümlü bir ikili ağaçta tüm yaprak düğümlerin (leaf nodes) toplamını hesaplamanın zaman karmaşıklığı nedir?

Cevap: D) O(n)
----------------------------------------------------------------------------------------
Question 5 (Full Binary Tree tanımı gereği bir düğümün ya hiç çocuğu yoktur (yaprak) ya da tam olarak iki çocuğu vardır; tek çocuklu düğüm bulunmaz.)
Soru: Full Binary Tree (Tam İkili Ağaç) nedir?

Cevap: A) Each node has exactly zero or two children
----------------------------------------------------------------------------------------
Question 6 (Huffman kodlaması, veri sıkıştırma algoritmalarında karakterleri temsil etmek için ikili ağaç yapısını (Huffman Tree) temel alır.)
Soru: İkili ağacın (binary tree) önemli bir uygulaması hangisidir?

Cevap: A) Huffman coding
----------------------------------------------------------------------------------------
Question 7 (Full Binary Tree'lerde yaprak sayısı ve toplam düğüm sayısı arasındaki matematiksel ilişki her zaman $N = 2L - 1$ formülüyle sağlanır.)
Soru: Bir "Full Binary Tree" yapısında L adet yaprak (leaf) varsa, toplam düğüm sayısı N nedir?

Cevap: D) N = 2L – 1
----------------------------------------------------------------------------------------
Question 8 (Post-order dolaşım mantığı "Sol alt ağaç -> Sağ alt ağaç -> Kök" sıralamasıyla çalışır.)
Soru: Aşağıdakilerden hangisi post-order dolaşım için doğru sözde koddur?

Cevap: A)
----------------------------------------------------------------------------------------
Question 9 (Post-order dizisinin son elemanı (M) bize her zaman kök düğümü verir. In-order dizisinde M'yi bulduğumuzda, solunda kalanlar (N) sol alt ağacı, sağında kalanlar (P, O, Q) ise sağ alt ağacı oluşturur. Post-order'da sağ alt ağaç grubunun son elemanı olan O, sağ tarafın köküdür. Bu mantıkla düğümler yerleştirildiğinde doğru yapı C şıkkındaki ağaç olur.)
Soru: Aşağıda verilen post-order ve in-order dizilerini kullanarak bir ikili ağaç (binary tree) oluşturun.
In-order: N, M, P, O, Q
Post-order: N, P, Q, O, M

Cevap: C (Kök düğümü M olan ağaç)
----------------------------------------------------------------------------------------
Question 10 (Geri Al/Yinele işlemleri (Undo/Redo) tipik olarak LIFO mantığına dayandığı için Yığın (Stack) veri yapısı ile gerçekleştirilir, ağaç yapısı ile değil.)
Soru: Aşağıdakilerden hangisi ağaç yapılarının (trees) avantajlarından biri değildir?

Cevap: D) Undo/Redo operations in a notepad
