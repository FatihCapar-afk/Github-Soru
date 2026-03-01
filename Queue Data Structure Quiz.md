Question 1 (Kuyruk FIFO (ilk giren ilk çıkar), yığın ise LIFO (son giren ilk çıkar) mantığıyla çalışır. Elemanların sırasını tersine çevirip kuyruk düzenini sağlamak için en az iki yığın gereklidir.)
Soru: Bir kuyruğu (queue) uygulamak için gereken minimum yığın (stack) sayısı kaçtır?

Cevap: C) 2
----------------------------------------------------------------------------------------
Question 2 (Dairesel diziler, kuyruktan eleman çıkarıldığında önde oluşan boş alanları tekrar kullanmamızı sağlayarak bellek israfını önler. Diğer maddelerdeki FIFO/LIFO eşleşmeleri yanlıştır.)
Soru: Aşağıdaki ifadelerden hangisi doğrudur?
i. FIFO tipi hesaplamalar yığınlar (STACKS) tarafından verimli desteklenir.
ii. Liste işlemlerinin çoğu için bağlı liste, diziden daha verimlidir.
iii. Kuyruğu dairesel dizide uygulamak, iki indeksli doğrusal diziden daha verimlidir.
iv. LIFO tipi hesaplamalar kuyruklar (QUEUES) tarafından verimli desteklenir.

Cevap: C) (iii) is true
----------------------------------------------------------------------------------------
Question 3 (Birinci yığın elemanları kabul eder, ikinci yığın ise elemanları ters çevirerek FIFO sırasını simüle eder.)
Soru: Bir kuyruk, dairesel olmayan tek yönlü bir bağlı liste (singly linked list) kullanılarak uygulanmıştır. Kuyruğun şekilde gösterildiği gibi bir head (baş) ve bir tail (kuyruk) işaretçisi vardır. n kuyruktaki düğüm sayısını temsil etsin. enqueue işleminin listenin başına yeni bir düğüm eklenerek, dequeue işleminin ise listenin sonundan (tail) bir düğüm silinerek uygulandığını varsayalım. Bu veri yapısı için sırasıyla enqueue ve dequeue işlemlerinin en verimli uygulamasının zaman karmaşıklığı nedir?

Cevap: B) Θ(1),Θ(n)
----------------------------------------------------------------------------------------
Question 4 (Dairesel kuyruklar, son elemandan sonra tekrar başa döndüğü için bir halka (ring) yapısı oluşturur, bu yüzden ağ ve ses işlemlerinde "Ring Buffer" olarak adlandırılır.)
Soru: Dairesel kuyruğa (Circular queue) aynı zamanda ne ad verilir?

Cevap: A) Ring Buffer
----------------------------------------------------------------------------------------
Question 5 (Tek yönlü bağlı listede son elemanı silmek için bir önceki elemana (penultimate) gitmek gerekir. Elimizde geriye doğru bir bağlantı olmadığı için baştan sona tarama yapmak gerekir, bu da O(n) sürer.)
Soru: Bağlı liste ile uygulanan bir kuyrukta; Rear işaretçisi son düğümü, Front işaretçisi ise ilk düğümü göstermektedir. Aşağıdaki işlemlerden hangisinin O(1) sürede yapılması imkansızdır?

Cevap: B) Delete the rear from the list.
----------------------------------------------------------------------------------------
Question 6 (Kod mantıksal olarak doğrudur. Katman bazlı (Level Order) ilerler ve her katmanın son elemanını (i == n - 1) yazdırır, bu da bize ağacın sağdan görünümünü verir.)
Soru: Bir ikili ağacın "Sağ Görünümünü" (Right View) kuyruk kullanarak yazdıran aşağıdaki kodda ne yanlıştır?
from collections import deque
class Node:
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None

def printRightView(root):
    if root is None:
        return

    q = deque([root])
    while q:
        n = len(q)
        for i in range(n):
            x = q.popleft()
            if i == n - 1:
                print(x.data, end=' ')
            if x.left:
                q.append(x.left)
            if x.right:
                q.append(x.right)
Cevap: D) None
----------------------------------------------------------------------------------------
Question 7 (Öncelikli kuyruklar, en küçük elemana öncelik veren "Ascending" (Artan) veya en büyük elemana öncelik veren "Descending" (Azalan) şeklinde iki tipte olabilir.)
Soru: Aşağıdakilerden hangisi bir öncelikli kuyruk (Priority Queue) tipidir?

Cevap: D) Both A and B.
----------------------------------------------------------------------------------------
Question 8 (Deque yapısı hem çift yönlü bağlı listelerle (doubly linked list) hem de dairesel dizilerle (circular array) her iki uçtan ekleme/çıkarma yapılabilecek şekilde verimli uygulanabilir.)
Soru: Deque (çift uçlu kuyruk) uygulamak için hangi veri yapısı kullanılır?

Cevap: D) Both B and C
----------------------------------------------------------------------------------------
Question 9 (Dairesel kuyruklar; belleği verimli kullanır (Memory Management), bilgisayar ağlarında veri trafiğini yönetir ve CPU çizelgeleme algoritmalarında yaygın kullanılır.)
Soru: Dairesel kuyruğun (Circular Queue) avantajları nelerdir?

Cevap: D) All of the above
----------------------------------------------------------------------------------------
Question 10 (Kod, bir kuyruk kullanarak ağacı katman katman (soldan sağa, yukarıdan aşağıya) gezer; bu işleme "Level Order Traversal" denir.)
Soru: Aşağıdaki programın ne yaptığını belirleyin.
class Node:
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
from collections import deque
def function(root):
    if root is None:
        return
    q = deque()
    q.append(root)
    while q:
        node = q.popleft()
        print(node.data, end=' ')
        if node.left is not None:
            q.append(node.left)
        if node.right is not None:
            q.append(node.right)
Cevap: C) Level order traversal of a tree
----------------------------------------------------------------------------------------
Question 11 (Monotonik yapılar, içindeki verinin sürekli artış veya azalış eğiliminde olduğu, genellikle kayan pencere (sliding window) problemlerinde kullanılan özel yapılardır.)
Soru: Elemanları kesinlikle artan veya kesinlikle azalan sırada saklayan deque yapısına ne ad verilir?

Cevap: C) Monotonic Deque
----------------------------------------------------------------------------------------
Question 12 (Olaylar (events) meydana geliş sırasına göre bir kuyruğa alınır ve sırayla işlenir, bu yüzden simülasyonların temel taşı kuyruk yapısıdır.)
Soru: Bilgisayar ağları veya trafik simülasyonları gibi karmaşık sistemlerin olay güdümlü simülasyonunda yaygın olarak hangi veri yapısı kullanılır?

Cevap: D) Queue
----------------------------------------------------------------------------------------
Question 13 (REAR ve FRONT aynı noktadaysa kuyruk boştur; REAR'ın bir sonraki adımı modüler aritmetik ile FRONT'a denk geliyorsa kuyruk doludur.)
Soru: n elemanlı bir diziyle uygulanan (n-1) kapasiteli dairesel bir kuyrukta, dolu ve boş olma koşulları nelerdir?

Cevap: A) Full: (REAR+1) mod n == FRONT, empty: REAR == FRONT
----------------------------------------------------------------------------------------
Question 14 (Kuyruklar LRU (En son kullanılan) algoritmasında sayfa değişimini takip etmek için kullanılır, ancak Quick Sort algoritması temelinde yığın (stack) yapısını (veya özyinelemeyi) kullanır.)
Soru: Aşağıdaki seçeneklerden hangisi yanlıştır?

Cevap: D) Both (A) and (C)
----------------------------------------------------------------------------------------
Question 15 (Kaynak paylaşımı (yazıcı sırası), asenkron veri transferi (buffer) ve yük dengeleme işlemlerinin tamamı kuyruk mantığıyla çalışır.)
Soru: Aşağıdakilerden hangisi Kuyruk (Queue) veri yapısının bir uygulamasıdır?

Cevap: D) All of the above
----------------------------------------------------------------------------------------
Question 16 (Kuyruktaki elemanlar yığına atıldığında sıraları tersine döner; yığından geri kuyruğa eklendiklerinde kuyruk tamamen ters çevrilmiş (reversed) olur.)
Soru: Bir kuyruğu (Q) argüman alan ve işlem yapmak için yığın (S) kullanan şu fonksiyon ne yapar?
def fun(Q):
    S = []
    while not Q.is_empty():
        S.append(Q.deQueue())
    while S:
        Q.enQueue(S.pop())
Cevap: D) Reverses the Q
----------------------------------------------------------------------------------------
Question 17 (q[2]'den başlayarak 9 eleman saydığımızda (2, 3, 4, 5, 6, 7, 8, 9, 10) dizi sonuna geliriz; dairesel yapı gereği bir sonraki eleman q[0]'a eklenir.)
Soru: Boyutu 11 olan bir dairesel kuyrukta Front ve Rear başlangıçta q[2] noktasını göstermektedir. Dokuzuncu eleman hangi pozisyona eklenir?

Cevap: A) q[0]
----------------------------------------------------------------------------------------
Question 18 (Fonksiyon elemanları tek tek çıkarıp sistem yığınında (call stack) tutar, en son elemana ulaşıldığında geri dönüş yolunda elemanları kuyruğa ekler; bu da kuyruğu ters çevirir.)
Soru: Aşağıdaki özyinelemeli (recursive) f fonksiyonu bir kuyruk üzerinde hangi işlemi gerçekleştirir?
def f(Q):
    if Q:
        i = Q.pop(0)
        f(Q)
        Q.append(i)
Cevap: B) Reverses the order of the elements in the queue Q
----------------------------------------------------------------------------------------
Question 19 (En kötü durumda (örneğin sayılar azalan sıradaysa), her eleman için yığın işlemleri tekrar tekrar yapılabilir; bu da n^2 yani 16*6 = 256 işlem gerektirebilir.)
Soru: 16 sayı içeren bir kuyruk ve bir yığın kullanılarak yapılan algoritmanın (Top(S) ≤ Head(Q) kontrolü ile) maksimum iterasyon sayısı kaçtır?

Cevap: C) 256
----------------------------------------------------------------------------------------
Question 20 (Dairesel dizi mantığı kullanılarak hem ekleme hem de çıkarma işlemleri dizinin boyutu ne olursa olsun sabit zamanda (O(1)) gerçekleştirilir.)
Soru: Dizi ile uygulanan bir kuyrukta ENQUEUE ve DEQUEUE işlemleri verimli yapılıyorsa zaman karmaşıklıkları nedir?

Cevap: A) Both operations can be performed in O(1) time
----------------------------------------------------------------------------------------
Question 21 (Ekleme için PUSH, çıkarma için ise REVERSE + POP + REVERSE yapılabileceği gibi, modifiye edilmiş bu yapıda kuyruk davranışı tekil komutlarla simüle edilebilir.)
Soru: Bir yığın; standart işlemlere ek olarak tüm yığını ters çeviren bir REVERSE komutunu destekliyorsa hangisi doğrudur?

Cevap: D) A queue can be implemented where both ENQUEUE and DEQUEUE take a single instruction each.
----------------------------------------------------------------------------------------
Question 22 (Enqueue (ekle), Dequeue (çıkar) ve Peek (bak) temel kuyruk işlemleridir; Shuffle (karıştır) standart bir kuyruk operasyonu değildir.)
Soru: Kuyruk veri yapısında hangisi yaygın bir işlem değildir?

Cevap: D) Shuffle
----------------------------------------------------------------------------------------
Question 23 (Kuyrukta her seferinde önceki iki sayıyı tutarak toplamlarını ekleyen bu mantık, Fibonacci serisini (0, 1, 1, 2, 3...) üretir.)
Soru: Aşağıdaki fonksiyon ne iş yapar?
# fun(int n) pseudocode
q.enqueue(0); q.enqueue(1);
for (int i = 0; i < n; i++) {
    int a = q.dequeue();
    int b = q.dequeue();
    q.enqueue(b);
    q.enqueue(a + b);
    print(a);
}
Cevap: C) Prints first n Fibonacci numbers
----------------------------------------------------------------------------------------
Question 24 (Amortize analiz yapıldığında; bir eleman sadece bir kez eklenebilir ve sadece bir kez silinebilir. Toplam operasyon sayısı toplam eklenen eleman sayısını geçemez, bu yüzden O(n) olur.)
Soru: Başlangıçta boş olan bir kuyrukta, k kadar elemanı silen MultiDequeue işleminin n kez yapıldığı bir dizinin en kötü durum zaman karmaşıklığı nedir?

Cevap: A) Theta(n)
----------------------------------------------------------------------------------------
Question 25 (Her eleman en az bir kez S1'e girip (push) çıkar (pop) ve en az bir kez S2'ye girip çıkar. Toplam operasyon sayısı eleman sayısının iki katı mertebesindedir.)
Soru: İki yığın (S1 ve S2) ile uygulanan bir kuyrukta n ekleme ve m silme işlemi yapıldığında, toplam push (x) ve pop (y) sayıları için hangisi doğrudur?

Cevap: D) 2m <= x < 2n and 2m <= y <= 2n
----------------------------------------------------------------------------------------
Question 26 (7 eklendiğinde heap kuralını korumak için yukarı doğru kaydırılır (bubble-up), sonuç olarak 7 uygun pozisyona yerleşir.)
Soru: Başlangıçta [10, 8, 5, 3, 2] şeklinde olan bir Max-Heap'e sırasıyla 1 ve 7 sayıları eklenirse yeni seviye-sırası (level-order) ne olur?

Cevap: D) 10, 8, 7, 3, 2, 1, 5
----------------------------------------------------------------------------------------
Question 27 (Kuyruk FIFO mantığıyla çalıştığı için bir uçtan (End/Rear) ekleme yapılırken, diğer uçtan (Beginning/Front) çıkarma yapılmalıdır.)
Soru: Kuyruğun bağlı liste uygulaması hakkında hangisi doğrudur?

Cevap: B) In push operation, if new nodes are inserted at the end, then in pop operation, nodes must be removed from the beginning
----------------------------------------------------------------------------------------
Question 28 (Heap yapıları, hem ekleme hem de en öncelikliyi çıkarma işlemlerini O(\log n) gibi düşük bir sürede yaptığı için bu senaryoda en idealidir.)
Soru: Ekleme, bakma ve çıkarma işlemlerinin sıklığının eşit olduğu bir durumda öncelikli kuyruk en verimli nasıl uygulanır?

Cevap: C) Heap Data Structures like Binary Heap, Fibonacci Heap
----------------------------------------------------------------------------------------
Question 29 (Düzgün uygulanmış (dairesel dizi veya işaretçili liste) bir kuyrukta başa ekleme ve sondan çıkarma işlemleri her zaman sabit sürede yapılır.)
Soru: Kuyrukta hangi işlemlerin zaman karmaşıklığı O(1)'dir?

Cevap: A) A and B (Enqueue and Dequeue)
----------------------------------------------------------------------------------------
Question 30 (Birinci yığın elemanları kabul eder, ikinci yığın ise elemanları ters çevirerek FIFO sırasını simüle eder.Birinci yığın elemanları kabul eder, ikinci yığın ise elemanları ters çevirerek FIFO sırasını simüle eder.)
Soru: Başka hiçbir veri yapısı (dizi, liste vb.) yoksa, bir kuyruk uygulamak için kaç yığın gereklidir?

Cevap: B) 2