Question 1 (Parantez eşleşmelerinde açılan her parantez yığına atılır ve kapanan bir parantez görüldüğünde en son açılanla eşleştirilip çıkarılır; bu LIFO (Son Giren İlk Çıkar) mantığına en uygun yapıdır.)
Soru: Bir aritmetik ifadedeki parantezlerin dengeli olup olmadığını kontrol etmek için en iyi veri yapısı hangisidir?

Cevap: B) Stack (Yığın)
----------------------------------------------------------------------------------------
Question 2 (Bir yığın elemanları eklemek (enqueue), diğeri ise elemanların sırasını tersine çevirip çıkarmak (dequeue) için kullanılır.)
Soru: Bir kuyruğu (queue) uygulamak için gereken minimum yığın (stack) sayısı kaçtır?

Cevap: C) 2
----------------------------------------------------------------------------------------
Question 3 (İşlemler sonucu yığının en altında kalan "A" elemanına ulaşılır. Diğerleri kuyruk ve yığın arasındaki transferler sırasında çıkarılmıştır.)
Soru: Beş öğe (A, B, C, D ve E), A'dan başlayarak sırayla bir yığına itiliyor (push). Yığından dört öğe çıkarılıyor (pop) ve her biri bir kuyruğa ekleniyor. Kuyruktan iki öğe siliniyor ve tekrar yığına geri itiliyor. Şimdi yığından bir öğe çıkarılıyor. Çıkarılan bu öğe nedir?

Cevap: A) A
----------------------------------------------------------------------------------------
Question 4 (Yığın kısıtlamaları nedeniyle "c" elemanı yazdırıldıktan sonra "a" elemanına doğrudan ulaşılamaz; çünkü "a", "b"nin altında veya B yığınında kalmış olur.)
Soru: Stack A has the entries a, b, c (with a on top). Stack B is empty. An entry popped out of stack A can be printed immediately or pushed to stack B. An entry popped out of the stack B can be only be printed. In this arrangement, which of the following permutations of a, b, c are not possible?

Cevap: C) c a b
----------------------------------------------------------------------------------------
Question 5 (Yığın ve kuyruk operasyonları sonucu yığında en son kalan eleman başlangıçtaki ilk eleman olan A'dır.)
Soru: (Soru 3 ile aynıdır) 
Cevap: A) A
----------------------------------------------------------------------------------------
Question 6 (Yığınlar; fonksiyon çağrılarını yönetmek, ifade değerlendirmek ve özel algoritmik problemleri (stock span gibi) çözmek için temel yapıdır.)
Soru: Aşağıdakilerden hangisi Yığın (Stack) veri yapısının bir uygulamasıdır?

Cevap: D) All of the above (Hepsi)
----------------------------------------------------------------------------------------
Question 7 (Verimli bir yığın için ekleme (push) ve çıkarma (pop) işlemleri bağlı listenin her zaman aynı ucundan (genellikle başından) yapılmalıdır; şıklardaki zıt uç eşleşmeleri verimsizdir.)
Soru: Yığının bağlı liste (linked list) uygulaması hakkında aşağıdakilerden hangisi doğrudur?

Cevap: D) None of the above (Hiçbiri)
----------------------------------------------------------------------------------------
Question 8 (Yığında son çıkarılan s=62, kuyrukta sırası gelen q=24 olur. Toplamları 86'dır.)
Soru: Boş bir yığın üzerinde şu işlemler yapılıyor:
Push(54);push(52);pop();push(55);push(62);s=pop();
Boş bir kuyruk üzerinde şu işlemler yapılıyor:
enqueue(21);enqueue(24);dequeue();enqueue(28);enqueue(32);q=dequeue();
s+q değeri kaçtır?

Cevap: A) 86
----------------------------------------------------------------------------------------
Question 9 (İşlem önceliğine göre önce parantez içindeki üs (^), sonra toplama (+), ardından bölme (/) ve çıkarma işlemleri postfix dizilimine uygun sıralanır.)
Soru: Aşağıdaki infix ifadeyi eşdeğer postfix ifadesine dönüştürün: (A + B^ D) / (E – F) + G

Cevap: A) ABD^ + EF – / G+
----------------------------------------------------------------------------------------
Question 10 (İş çizelgeleme işlemleri genellikle "ilk gelen ilk hizmet alır" mantığıyla çalıştığı için Stack değil, Queue (Kuyruk) yapısını kullanır.)
Soru: Aşağıdakilerden hangisi yığının (stack) doğal/dahili bir uygulaması değildir?

Cevap: C) Job scheduling (İş çizelgeleme)
----------------------------------------------------------------------------------------
Question 11 (Yapılan işlemler yığın kapasitesini (5) aşmaz ve boş yığından eleman çıkarma hatası (underflow) oluşturmaz; bu yüzden işlemler sorunsuz tamamlanır.)
Soru: 5 boyutlu bir yığında şu işlemler yapılıyor: Push (a); Pop(); Push(b); Push(c); Pop(); Push(d); Pop(); Pop(); Push (e). Hangisi doğrudur?

Cevap: B) Stack operations are performed smoothly
----------------------------------------------------------------------------------------
Question 12 (Karmaşık transfer işlemlerinden sonra yığından pop edilen son eleman en başta en alta konulan A elemanıdır.)
Soru: (Soru 3 ile aynıdır) 

Cevap: A) A
----------------------------------------------------------------------------------------
Question 13 (LIFO kuralına göre her pop işlemi, o an yığının en üstünde hangi sayı varsa onu dışarı çıkarır.LIFO kuralına göre her pop işlemi, o an yığının en üstünde hangi sayı varsa onu dışarı çıkarır.)
Soru: Eğer bir yığında push (1), push (2), pop, push (1), push (2), pop, pop, pop, push (2), pop işlemleri yapılırsa, çıkan değerlerin sırası ne olur?

Cevap: A) 2, 2, 1, 1, 2
----------------------------------------------------------------------------------------
Question 14 (Elemanların yığın ve kuyruk arasındaki yer değiştirme sırası takip edildiğinde, son pop işleminde yığının üstünde B elemanı bulunur.)
Soru: A, B, C, D, E, F ve G elemanları bir yığına ters sırada (G'den başlayarak) itiliyor. Yığından beş pop yapılıp kuyruğa ekleniyor. Kuyruktan iki eleman silinip yığına geri itiliyor. Sonra yığından bir pop yapılıyor. Çıkarılan öğe nedir?

Cevap: B) B
----------------------------------------------------------------------------------------
Question 15 (Sayının 2'ye bölümünden kalanlar (bitler) yığına atılır; yığın ters sırada (LIFO) boşaltıldığında sayının doğru ikili (binary) karşılığı ekrana yazılmış olur.)
Soru: Aşağıdaki fonksiyon genel olarak ne yapar?
def fun(n):
    S = []  # Say it creates an empty stack S
    while n > 0:
        # This line pushes the value of n%2 to stack S
        S.append(n % 2)
        n = n // 2

    # Run while Stack S is not empty
    while S:
        print(S.pop(), end=' ')  # pop an element from S and print it
Cevap: B) Prints binary representation of n
----------------------------------------------------------------------------------------
Question 16 (5 ve 6 yığındayken 7, 8 ve 9 sırayla girip çıkabilir, ardından yığında bekleyen 6 ve en alttaki 5 çıkarılabilir.)
Soru: Giriş sırası 5, 6, 7, 8, 9 olduğunda, bir yığın kullanılarak hangi çıktı sırası elde edilebilir?

Cevap: C) 7, 8, 9, 6, 5
----------------------------------------------------------------------------------------
Question 17 (Yığın yapısını taklit etmek için en son giren elemanın en küçük anahtara sahip olması gerekir ki DELETEMIN yapıldığında en son giren ilk çıksın.)
Soru: Bir öncelikli kuyruk (Q), karakter saklayan bir yığın (S) simüle etmek için kullanılıyor. PUSH işlemi INSERT(Q, C, K) ile, POP ise DELETEMIN(Q) ile yapılıyor. Anahtarlar (K) hangi sırada seçilmelidir?

Cevap: D) strictly decreasing order (kesinlikle azalan)
----------------------------------------------------------------------------------------
Question 18 (Bir min-heap (küçükten büyüğe yığın) kullanarak k yığının tepesindeki elemanları karşılaştırıp birleştirmek (k-way merge) bu karmaşıklığı sağlar.)
Soru: k adet yığına eşit dağıtılmış n eleman var (her biri kendi içinde sıralı). Bunları tek bir sıralı kuyruğa dizmek için en iyi algoritmanın zaman karmaşıklığı nedir?

Cevap: A) O(n logk)
----------------------------------------------------------------------------------------
Question 19 (Bağlı listenin başına ekleme ve başından silme işlemleri listenin uzunluğundan bağımsız olarak sabit zamanda yapılır.)
Soru: Yığın bağlı liste ile verimli uygulanırsa push ve pop karmaşıklığı ne olur?

Cevap: B) O(1) for insertion and O(1) for deletion
----------------------------------------------------------------------------------------
Question 20 (Program bir postfix hesaplayıcıdır. (5*2) + (3*(3+2)) işlemini yaparak 25 sonucunu bulur.)
Soru: Aşağıdaki programda 5 2 * 3 3 2 + * + girdisi için çıktı ne olur?
class Stack:
    def __init__(self):
        self.items = []
    def push(self, item):
        self.items.append(item)  # push the argument on the stack
    def pop(self):
        return self.items.pop() if self.items else -1  # pop the top of the stackdef flagError():
    print("Error!")
    exit(1)s = Stack()while True:
    try:
        c = input()
        if c == '':
            break
        c = ord(c)
        if c >= ord('0') and c <= ord('9'):
            s.push(c - ord('0'))
        elif c == ord('+') or c == ord('*'):
            m = s.pop()
            n = s.pop()
            r = n + m if c == ord('+') else n * m
            s.push(r)
        elif c != ord(' '):
            flagError()
    except EOFError:
        breakprint(s.pop())
Cevap: B) 25
-
Question 21 (İşlemler sırayla yapılır: f(2)=2, f(2,-3)=-1, f(2,-3,2)=2, f(2,-3,2,-1)=1, f(2,-3,2,-1,2)=3 bulunur.)
Soru: f(∅) = 0 ve f(push(S, i)) = max(f(S), 0) + i fonksiyonuna göre; tabandan tepeye 2, -3, 2, -1, 2 sayılarını içeren yığın için f(S) nedir?

Cevap: C) 3
----------------------------------------------------------------------------------------
Question 22 ((10+5)*(60/6) - 8->15 *10 - 8->150 - 8 = 142.)
Soru: 10 5 + 60 6 / * 8 – postfix ifadesinin sonucu nedir?

Cevap: C) 142
----------------------------------------------------------------------------------------
Question 23 (Standart bir aritmetik ifadeyi (operatör ve işlenenleri) yönetmek için tek bir yığın veri yapısı yeterlidir.)
Soru: Fonksiyon çağrısı içermeyen düz bir ifadeyi değerlendirmek için kaç yığın gerekir?

Cevap: B) One stack is enough
----------------------------------------------------------------------------------------
Question 24 (Postfix yazımında operatörler işlenenlerden sonra gelir ve öncelik sırasına (üs, çarpma, toplama) göre dizilirler.)
Soru: a + b × c - d ^ e ^ f ifadesinin postfix hali nedir?

Cevap: A) abc × + def ^ ^ -
----------------------------------------------------------------------------------------
Question 25 (İki yığının tepe işaretçileri yan yana geldiğinde (arada boşluk kalmadığında) dizi tamamen dolmuş demektir.)
Soru: Tek bir dizide iki yığın zıt uçlardan birbirine doğru büyüyorsa "yığın dolu" durumu hangisidir?

Cevap: D) top1 = top2 - 1
----------------------------------------------------------------------------------------
Question 26 (Elemanların yığında kalma sürelerinin aritmetik ortalaması, toplam işlem ve bekleme sürelerinin n elemana dağılımı ile hesaplanır.)
Soru: n elemanlı bir yığında her işlem X saniye, aralar Y saniye sürüyorsa bir elemanın ortalama yığın ömrü nedir?

Cevap: C) n(X + Y) - X
----------------------------------------------------------------------------------------
Question 27 (İşlem sırasında 2*3 = 6 bulunur; yığında bu sonucun altında önceki işlemlerden kalan 1 değeri vardır.)
Soru: 8 2 3 ^ / 2 3 * + 5 1 * - ifadesinde ilk * (çarpma) yapıldıktan sonra yığının en üstündeki iki eleman nedir?

Cevap: A) 6, 1
----------------------------------------------------------------------------------------
Question 28 (Kod, döngü bittiğinde yığının boş olup olmadığını kontrol etmediği için, fazla açılan parantezler (yığında kalanlar) olsa bile hata vermez.)
Soru: Aşağıdaki hatalı algoritma hangi dengesiz parantez dizisini "dengeli" sanır?
   declare a character stack    
   while ( more input is available)   
   {      
      read a character      
      if ( the character is a '(' )          
         push it on the stack      
      else if ( the character is a ')' and the stack is not empty )         
         pop a character off the stack      
      else         
         print "unbalanced" and exit    
   }    
   print "balanced"

Cevap: A) ((())
----------------------------------------------------------------------------------------
Question 29 (Karakterler sırayla yığına atılıp sonra tek tek çıkarıldığı için kelime tersten yazdırılmış olur.)
Soru: "geeksquiz" girdisi için aşağıdaki kodun çıktısı nedir?
# Declare a stack of charactersword = "example"  
char_stack = []
for c in word:
    char_stack.append(c)  # Push
while char_stack:
    c = char_stack.pop()  # Pop
    print(c, end='')

Cevap: B) ziuqskeeg
----------------------------------------------------------------------------------------
Question 30 (Kuyrukları dairesel bir dizide (circular array) tutmak, elemanlar silindikçe oluşan boş alanı tekrar kullanmayı sağladığı için doğrusal diziden çok daha verimlidir.)
Soru: Veri yapıları hakkındaki aşağıdaki ifadelerden hangisi doğrudur?

Cevap: C) (iii) is true