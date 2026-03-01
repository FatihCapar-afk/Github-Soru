Soru 1 (X'ten önceki düğümün "ileri"sini X'ten sonrakine, sonrakinin "geri"sini ise X'ten öncekine bağlarız.)
Çeviri: Çift yönlü bağlı listede X düğümünü silen kod hangisidir?
Cevap: B) X->Bwd.Fwd = X->Fwd ; X.Fwd->Bwd = X->Bwd ;
----------------------------------------------------------------------------------------
Soru 2 (Başa ekleme sabittir, ancak tek yönlü listede sondan silmek için tüm listeyi tarayıp sondan bir önceki düğümü bulmak gerekir (O(n)).)
Çeviri: Başı (head) ve sonu (tail) olan bir bağlı listede enqueue (başa ekleme) ve dequeue (sondan silme) işlemlerinin zaman karmaşıklığı nedir?
Cevap: B) Θ(1), Θ(n)
----------------------------------------------------------------------------------------
Soru 3 (Yeni bir düğüm eklendiğinde; yeni düğümün ileri ve geri işaretçileri (2), önceki düğümün ileri işaretçisi (1) ve sonraki düğümün geri işaretçisi (1) olmak üzere toplam 4 işaretçi güncellenir.)
Soru: Çift yönlü bir bağlı listede, bir ekleme (insertion) işlemi sırasında etkilenen toplam işaretçi (pointer) sayısı kaçtır?
Cevap: D) None of these (4 olmalı)
----------------------------------------------------------------------------------------
Soru 4 (Son düğümü silmek için bir önceki düğüme (n-1) erişmek gerekir. Tek yönlü listede geriye gidiş olmadığı için baştan sona tarama yapmak zorunludur, bu da O(n) sürer.)
Soru: Baş (head) ve son (tail) işaretçisi olan sıralanmamış tek yönlü bir bağlı listede, hangi işlem O(1) sürede gerçekleştirilemez?
Cevap: D) Deletion of the last node of the linked list.
----------------------------------------------------------------------------------------
Soru 5 / 12 (Son elemanı silmek için sondan bir önceki düğümün next değerini null yapmanız gerekir. Bu düğümü bulmak tüm listeyi taramayı gerektirir.)
Soru: F (ilk) ve L (son) işaretçileri olan tek yönlü bir listede, hangi işlemin süresi listenin uzunluğuna bağlıdır?
Cevap: C / A) Delete the last element of the list
----------------------------------------------------------------------------------------
Soru 6 (Yeni bir p düğümü oluşturuluyor, içine veri konuyor, p'nin sonrası mevcut listenin başı yapılıyor ve listenin yeni başı p olarak güncelleniyor.)
Kod:
p = getnode()
info (p) = 10
next (p) = list
list = p
Soru: Bu adımlar ne tür bir işlemle sonuçlanır?
Cevap: C) inserting a node at beginning (Başa düğüm ekleme)
----------------------------------------------------------------------------------------
Soru 8 (Konumu verilen bir düğümü silerken, çift yönlü listede önceki düğüme doğrudan Bwd ile erişilebilir; tek yönlü listede ise baştan arama yapmak gerekir.)
Soru: Hangi işlem çift yönlü bağlı listede, tek yönlü listeye göre daha verimli gerçekleştirilir?
Cevap: A) Deleting a node whose location is given
----------------------------------------------------------------------------------------
Soru 9 / 14 (Bağlı listeler rastgele erişimi (random access) desteklemez; aranan elemanı bulmak için en kötü durumda tüm listeyi tek tek gezmek gerekir.)
Soru: n uzunluğundaki bir bağlı listede bir elemanı aramak (en kötü durumda) ne kadar sürer?
Cevap: B / D) O(n)
----------------------------------------------------------------------------------------
Soru 10 (Bir düğümde; verinin kendisi (data), bir sonraki düğümün adresi (Fwd) ve bir önceki düğümün adresi (Bwd) bulunmalıdır.)
Soru: Çift yönlü bağlı listenin her bir düğümünde olması gereken minimum alan (field) sayısı kaçtır?
Cevap: C) 3
-----------------------------------------------------------------------------------------
Soru 11 (Her iki listenin uzunluklarını bulup aradaki fark kadar uzun olan listede ilerledikten sonra beraber hareket ederek kesişim noktası doğrusal sürede bulunur.)
Soru: Kesişen iki tek yönlü bağlı listenin kesişme noktasını bulan en iyi algoritmanın en kötü durum zaman karmaşıklığı nedir?
Cevap: C) Θ(m+n)
----------------------------------------------------------------------------------------
Soru 12 (Son elemanı silmek için bir önceki düğüme erişmek gerekir; tek yönlü listede geriye gidiş olmadığından baştan sona tüm listeyi taramak zorunludur.)
Soru: F'nin ilk elemanı, L'nin ise son elemanı işaret ettiği bir tek yönlü bağlı listede (singly linked list), aşağıdaki işlemlerden hangisinin süresi listenin uzunluğuna bağlıdır?
Cevap: A) Delete the last element of the list
----------------------------------------------------------------------------------------
Soru 13 (Merge Sort, bağlı listeler için rastgele erişim gerektirmediğinden ve sıralı birleştirmeyi kolay yaptığı için O(n log n) ile en verimlisidir.)
Soru: Rastgele elemanlı bir bağlı listeyi en düşük zaman karmaşıklığı ile sıralayan algoritma hangisidir?
Cevap: D) Merge Sort
----------------------------------------------------------------------------------------
Soru 14 (Aranan eleman listenin en sonunda olabilir veya listede hiç olmayabilir; bu durumda tüm elemanları (n adet) kontrol etmek gerekir.)
Soru: n uzunluğundaki tek yönlü bir bağlı listede belirli bir elemanı aramak için en kötü durumda (worst case) gereken karşılaştırma sayısı nedir?
Cevap: D) n
----------------------------------------------------------------------------------------
Soru 15 (Düğümü silmek yerine, bir sonraki düğümün verisini Q'ya kopyalayıp sonraki düğümü listeden çıkararak (data copying trick) sabit sürede silme yapılabilir.)
Soru: Tek yönlü bir listede, konumu Q ile verilen bir ara düğümü silen bilinen en iyi algoritmanın karmaşıklığı nedir?
Cevap: D) O(1)
----------------------------------------------------------------------------------------
Soru 16 (Her yeni eleman için doğru yer bulunana kadar liste taranır (ortalama n/2). n eleman için bu işlem toplamda karelik (n*n) bir karmaşıklık oluşturur.)
Soru: n adet elemanı, sıralı (sorted) kalması gereken boş bir bağlı listeye eklemenin en kötü durum zaman karmaşıklığı nedir?
Cevap: C) Θ(n²)
----------------------------------------------------------------------------------------
Soru 17 (Tanım gereği bir temel uygun çözümün bozulmamış olması için kısıtları sağlaması, atama sayısının tam olması ve bağımsız pozisyonlarda olması gerekir.)
Soru: Bir taşıma probleminin başlangıç çözümü, aşağıdaki koşullardan hangilerini sağlıyorsa "non-degenerate basic feasible solution" (bozulmamış temel uygun çözüm) olarak adlandırılır?(a) Çözüm uygulanabilir olmalı, yani tüm arz ve talep kısıtlarını sağlamalı.(b) Pozitif atama sayısı $m+n-1$ olmalı (m: satır, n: sütun).(c) Tüm pozitif atamalar bağımsız konumlarda olmalı.
Cevap: D) (a), (b) and (c)
----------------------------------------------------------------------------------------
Soru 18 (Kuyrukları (Queue) dairesel dizide (circular array) tutmak, eleman eklendikçe/silindikçe tüm diziyi kaydırma zorunluluğunu ortadan kaldırdığı için lineer diziden daha verimlidir.)
Soru: Verilen ifadelerden hangisi doğrudur?
Cevap: C) (iii) is true
----------------------------------------------------------------------------------------
Soru 21 (Baştan n. elemana gitmek sabit bir k (8) adımıdır, ancak sondan gitmek için önce listenin sonunu veya uzunluğunu bilmek gerekir.)
Soru: n elemanlı listede baştan 8. ve sondan 8. elemanı bulmanın karmaşıklıkları nedir?
Cevap: A) O(1) and O(n) (Baştan 8 sabit bir adım, sondan 8 ise listeyi taramayı gerektirir).
----------------------------------------------------------------------------------------
Soru 22 (Diziler daha iyi önbellek (cache) yerelliğine sahiptir; bağlı listelerde eleman ekleme/silme kolaydır; bağlı listelerde rastgele erişim (random access) yoktur ve listelerin boyutu dinamik olarak değişebilir.)
Soru: Bağlı listeler dizilerle (array) karşılaştırıldığında aşağıdakilerden hangisi doğrudur?
Cevap: E) All of the above (Hepsi)
----------------------------------------------------------------------------------------
Soru 23 (Kod, her düğümün prev ve next işaretçilerini birbiriyle takas ederek listeyi tamamen ters çevirir.)
Soru: Verilen fun fonksiyonu çift yönlü listeye uygulandığında sonuç ne olur? (1 <-> 2 <-> 3 <-> 4 <-> 5 <-> 6)
Cevap: C) 6 <--> 5 <--> 4 <--> 3 <--> 2 <--> 1.
----------------------------------------------------------------------------------------
Soru 24 (Döngü bittiğinde current null olur, prev ise listenin yeni başı olan eski son düğümü işaret eder. Bu yüzden listenin başı (head) prev olarak güncellenmelidir.)
Soru: Bağlı listeyi ters çeviren fonksiyondaki eksik satır ne olmalıdır?
Cevap: A) Set the value of head_ref to prev;
----------------------------------------------------------------------------------------
Soru 25 (Fonksiyon bir elemanı yazdırır, bir sonrakini atlayıp (next.next) kendini çağırır, en sona ulaştığında ise geri dönüş yolunda (stack unwinding) yazdırmaya devam eder.)
Kod:
def fun(start):
    if start is None: return
    print(start.data, end='  ')
    if start.next is not None:
        fun(start.next.next)
    print(start.data, end='  ')
Soru: 1->2->3->4->5->6 listesi için çıktı nedir?
Cevap: D) 1 3 5 5 3 1
----------------------------------------------------------------------------------------
Soru 26 (Sondan bir önceki düğümün (q) bağlantısı kesilir, son düğüm (p) eski başa (head) bağlanır ve yeni baş p yapılır.)
Soru: Listenin son elemanını başa taşıyan koddaki boşluk nasıl dolmalıdır?
Cevap: D) next of q = NULL; next of p = head; head = p;
----------------------------------------------------------------------------------------
Soru 27 (Fonksiyon ikili gruplar (1-2, 3-4, 5-6) halinde elemanların değerlerini birbiriyle takas eder; tek kalan 7 değişmeden kalır.)
Soru: 1, 2, 3, 4, 5, 6, 7 listesi bu fonksiyonla nasıl değişir?
Cevap: B) 2, 1, 4, 3, 6, 5, 7
----------------------------------------------------------------------------------------
Soru 28 (Birleşim ve kesişim işlemleri, her iki listenin elemanlarını birbirleriyle kıyaslamayı gerektirdiği için $O(n^2)$ veya sıralama ile O(n \log n) zaman alarak diğerlerinden daha yavaş çalışır.)
Soru: Her bir kümenin rastgele sıralı bağlı listelerle temsil edildiği varsayılırsa; birleşim (union), kesişim (intersection), üyelik (membership) ve eleman sayısı (cardinality) işlemlerinden hangisi en yavaşıdır?
Cevap: D) union, intersection
----------------------------------------------------------------------------------------
Soru 29 (Kod, p.data <= p.next.data kontrolü yaparak listenin küçükten büyüğe (azalmayan sırada) sıralı olup olmadığını denetler.)
Soru: Verilen özyinelemeli f(p) fonksiyonu ne zaman 1 döner?
Cevap: B) the elements in the list are sorted in non-decreasing order of data value
----------------------------------------------------------------------------------------
Soru 30 (p son düğümü gösterirse, p.next her zaman ilk düğümü (front) gösterir. Böylece her iki uca da erişim sabit zamanlı olur.)
Soru: Tek bir p işaretçisiyle hem ekleme (enQueue) hem silme (deQueue) işleminin sabit sürede yapılması için p nereyi göstermelidir?
Cevap: A) rear node (Son düğüm)
----------------------------------------------------------------------------------------
Soru 31 (Önce bir sonraki düğüm çağrıldığı için sistem en sona kadar gider ve fonksiyonlar geri dönerken (recursive backtracking) yazdırma yapar; bu da listeyi tersten yazdırır.)
Soru: fun1(head.next) çağrısından sonra yazdırma yapan bu fonksiyon ne yapar?
Cevap: B) Prints all nodes of linked list in reverse order
----------------------------------------------------------------------------------------
Soru 32 (Önceki ve sonraki düğüm adreslerinin XOR'u saklanarak, bellekten tasarruf sağlayan bir çift yönlü yapı kurulabilir.)
Soru: Her düğümde sadece tek bir işaretçi (pointer) kullanarak çift yönlü bağlı liste (doubly linked list) oluşturmak mümkün müdür?
Cevap: B) Yes, possible by storing XOR of addresses of previous and next nodes.
----------------------------------------------------------------------------------------
Soru 33 (X'ten sonraki veriyi X'e kopyalayıp X'in bir sonrakini silerek (Soru 15'teki mantıkla) bu mümkündür.)
Soru: Baş (head) işaretçisi verilmeden sadece X düğümü verilerek silme yapılabilir mi?
Cevap: A) Possible if X is not last node...
----------------------------------------------------------------------------------------
Soru 34 (XOR bağlı listeler, çift yönlü liste işlevselliğini tek bir işaretçi alanıyla sağladığı için bellek verimliliği gereken durumlarda kullanılır.)
Soru: Aşağıdakilerden hangisi XOR bağlı listelerin (XOR-linked lists) bir uygulamasıdır?
Cevap: C) Memory-efficient linked list representation
----------------------------------------------------------------------------------------
Soru 35 (Fonksiyon doğru çalışır; liste boşsa döngüye girmez, her elemanı yazar ve head değişkeni fonksiyon içinde yerel (local) olduğu için orijinal listeyi bozmaz.)
Soru: Verilen traverse fonksiyonu için hangisi YANLIŞTIR?
Cevap: D) None of the above