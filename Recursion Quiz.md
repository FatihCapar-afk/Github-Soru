Soru 1 (Bu fonksiyon aslında Catalan Sayıları (C_{n-1}) dizisini hesaplar. fun(1)=1, fun(2)=1, fun(3)=2, fun(4)=5, fun(5)=14 şeklinde giderdi ancak bu koddaki toplama yapısı fun(5)=26 sonucunu verir.)
def fun(n):
  x = 1
  if n == 1:
    return x
  for k in range(1, n):
    x += fun(k) * fun(n - k)
  return x
Çeviri: Verilen fun(n) fonksiyonunda fun(5) değeri kaçtır?
Cevap: B) 26
----------------------------------------------------------------------------------------
Soru 2 (Kod, yan yana olan elemanları karşılaştırıp (arr[i] > arr[i+1]) yer değiştiriyor ve her adımda en büyük elemanı sona "ittiriyor". Bu tipik bir Bubble Sort algoritmasıdır.)
def fun(arr, n):
    if n == 1:
        return

    count = 0
    for i in range(n - 1):
        if arr[i] > arr[i + 1]:
            arr[i], arr[i + 1] = arr[i + 1], arr[i]
            count += 1
    fun(arr, n - 1)
Çeviri: Aşağıdaki program hangi işlemi gerçekleştirmektedir?
Cevap: B) Bubble Sort Recursively (Özyinelemeli Baloncuk Sıralaması)
----------------------------------------------------------------------------------------
Soru 3 (A. Özyineleme (Base Case/Taban Durumu), B. İkili Arama (Sıralı Dizi gerekir), C. Sıralama (O(N \log N) karmaşıklığı), D. Dinamik Programlama (Özyinelemeyi kullanır).)
List 1	List 2
A. Recursion	1. Sorted Array
B. Binary Seach	2. Recursion
C. Sorting	3 Base case
D. Dynamic Programming	4.O(NlogN)
Çeviri: Listeleri birbiriyle eşleştirin.
Cevap: C) A – 3, B – 1, C – 4, D – 2
----------------------------------------------------------------------------------------
Soru 4 (Kod, verilen aralıktaki en küçük elemanı bulup (minIndex) onu en başa taşıyor ve kalan dizi için kendini tekrar çağırıyor. Bu özyinelemeli Selection Sort'tur.)
def fun2(arr, start_index, end_index):
    if start_index >= end_index:
        return
    min_index = minIndex(arr, start_index, end_index)
    arr[start_index], arr[min_index] = arr[min_index], arr[start_index]
    fun2(arr, start_index + 1, end_index)
Çeviri: Verilen program hangi problemi/algoritmayı tanımlar?
Cevap: A) Selection Sort Recursive implementation
----------------------------------------------------------------------------------------
Soru 5 (Fonksiyon dizideki tüm sayıları topluyor: 1+2+3+4+5+6 = 21)
def fun(arr, n):
	if n <= 0:
		return 0
	return fun(arr, n - 1) + arr[n - 1]
Çeviri: arr = {1,2,3,4,5,6} ve N=6 için çıktı nedir?
Cevap: A) 21
----------------------------------------------------------------------------------------
Soru 6: (In-order gezinme, ağacı soldan sağa doğru bir izdüşümle okumak gibidir.)
Çeviri: Verilen ikili ağaç (binary tree) için aşağıdaki Python programının çıktısı ne olur? (Program print_inorder fonksiyonunu kullanıyor).
def print_inorder(node):
    if node is None:
        return

    print_inorder(node.left)
    print(node.data, end=' ')
    print_inorder(node.right)
Doğru Cevap: C (4 2 5 1 3)

Çözüm: In-order (iç-sıralı) gezinme prensibi şudur: Sol Alt Ağaç -> Kök -> Sağ Alt Ağaç.
En sola git: 4
Köküne dön: 2
Sağına geç: 5
Ana köke dön: 1
En sağa geç: 3
----------------------------------------------------------------------------------------
Soru 7 (Kodun yapısı (diski bir çubuktan diğerine taşıma mantığı), klasik Hanoi Kuleleri bulmacasının çözüm adımlarıdır.)
def fun(n, from_rod, to_rod, aux_rod):
	if n == 0:
		return
	fun(n - 1, from_rod, aux_rod, to_rod)
	print(f"Move disk {n} from rod {from_rod} to rod {to_rod}")
	fun(n - 1, aux_rod, to_rod, from_rod)
Çeviri: Aşağıdaki özyinelemeli programın adı nedir?
Cevap: B) Tower of Hanoi (Hanoi Kuleleri)
----------------------------------------------------------------------------------------
Soru 8 (j değerini 1'den başlatıp her seferinde j ve n-j ikilisini yazdırıyor. n-j >= j koşulu bozulana kadar (yani 4 >= 4 son adım) devam eder.)
def print_pairs(n, j):
    if j >= n:
        return
    if n - j > 0 and n - j >= j:
        print(j, n - j)
    print_pairs(n, j + 1)

n = 8
print_pairs(n, 1)
Çeviri: Verilen programın çıktısı nedir? (n = 8)
Cevap: B) 1 7, 2 6, 3 5, 4 4
----------------------------------------------------------------------------------------
Soru 9 (Fonksiyon, verilen sayıyı sürekli 2'ye bölerek kalanları sondan başa doğru yazdırıyor. Bu işlem, sayının ikilik tabandaki (binary) karşılığını verir. 173'ün ikilik karşılığı 10101101'dir.)
def f(n):
    if n <= 1:
        print(n, end='')
    else:
        f(n // 2)
        print(n % 2, end='')
Çeviri: f(173) ne yazdırır?
Cevap: D) 10101101
----------------------------------------------------------------------------------------
Soru 10 (Bu, ünlü Collatz Sanısı'na (3n+1 problemi) benzer bir yapıdır. Matematiksel olarak tüm sayılar için sonlandığı kanıtlanmamıştır ancak sonsuz sayıda değer için sonlandığı (2'nin kuvvetleri gibi) bilinir.)
def f(n):
    if n <= 1:
        return 1
    elif n % 2 == 0:
        return f(n // 2)
    else:
        return f(3 * n - 1)
Çeviri: f fonksiyonunun sonlanması (terminates) hakkında hangisi doğrudur?
Cevap: D) (ii) and (iv)
----------------------------------------------------------------------------------------
Soru 11 (Master Teoremi uygulanırsa, her adımda veri setinin belirli bir oranda azaldığı ve sabit bir iş (+1) yapıldığı görülür. Bu da logaritmik zaman karmaşıklığı (O(\log m)) üretir.)
Çeviri: T(m) = T(3m/4) + 1 bağıntısının çözümü nedir?
Cevap: A) θ (lg m)
----------------------------------------------------------------------------------------
Soru 12 (Genel olarak döngü (non-recursive) kullanan programlar, fonksiyon çağrısı yükü ve yığın (stack) belleği kullanımı olmadığı için hem zaman hem alan açısından daha verimlidir.)
Çeviri: Özyinelemeli (recursive) ve özyinelemeli olmayan (iterative) programlar hakkında hangisi doğrudur?
Cevap: B) Both time and space complexities are better in non-recursive than in recursive program.
----------------------------------------------------------------------------------------
Soru 13 (P1, önce özyinelemeli çağrıyı yapıp sonra yazdırma işlemini yaptığı için doğru sırayı korur. P2 ise önce yazdırıp sonra çağırdığı için sonucu ters yazdırır.)
def f(n):
    if n <= 1:
        print(n, end='')
    else:
        f(n // 2)
        print(n % 2, end=''

void f (int n)
{
    if (n/2)  {
        f(n/2);
    }
    printf ("%d", n%2);
}

void f (int n)
{
    if (n <=1)  {
        printf ("%d", n);
    }
    else {
        printf ("%d", n%2);
        f (n/2);
    }
}
Çeviri: P1 ve P2 kodlarından hangisi f(173) ile aynı çıktıyı (ikilik taban karşılığını) üretir?
Cevap: C) P1 only
----------------------------------------------------------------------------------------
Soru 14 (global d değişkeni her adımda artıyor. Fonksiyon içeri girerken (n, d) ikilisini yazdırıyor, en derin noktadan geri dönerken de güncel d değerini tekrar yazdırıyor.)
d = 1

def count(n):
    global d
    print(n, end=' ')
    print(d, end=' ')
    d += 1
    if n > 1:
        count(n - 1)
    print(d, end=' ')

count(3)
Çeviri: JAVA programının çıktısı nedir?
Cevap: A) 3 1 2 2 1 3 4 4 4
----------------------------------------------------------------------------------------
Soru 15 (Fonksiyonun her çağrıda oluşturduğu dallanma ağacını (tree) çizdiğinde (6->    5, 3->...), toplam 25 tane düğüm (çağrı) olduğunu görürsün.)
def get(n):
    if n < 1:
        return
    get(n - 1)
    get(n - 3)
    print(n)
Çeviri: get(6) çağrıldığında toplam kaç kez get() fonksiyonu çalıştırılır?
Cevap: B) 25
----------------------------------------------------------------------------------------
Soru 16 (`2 * fun(3) \rightarrow 2 * (2 * fun(4)) \rightarrow 2 * 2 * 4 = 16$.)
def fun(n):
    if n == 4:
        return n
    else:
        return 2 * fun(n + 1)

print(fun(2))
Çeviri: fun(2) program çıktısı nedir?
Cevap: C) 16
----------------------------------------------------------------------------------------
Soru 17 (Global i değeri her adımda artıyor. f(1, i=1)-> f(2, i=2)-> f(4, i=3)-> f(7, i=4). Sonuç 7'dir çünkü 5'ten büyüktür.)
def f(n):
   global i
   if 'i' not in globals():
       i = 1
   if n >= 5:
       return n
   n = n + i
   i += 1
   return f(n)
Çeviri: f(1) değeri nedir?
Cevap: C) 7
----------------------------------------------------------------------------------------
Soru 18 (Fonksiyon içinde f(i) tekrar çağrılıyor ve i her zaman 50 olduğu için bir çıkış koşulu (base case) oluşmaz; bu da sonsuz döngüye ve yığın taşmasına (stack overflow) neden olur.)
def f(j):
    i = 50
    if i == j:
        print("something")
        k = f(i)
        return 0
    else:
        return 0
Çeviri: j=50 olduğunda ne olur?
Cevap: D) The function will exhaust the runtime stack or run into an infinite loop when j = 50.
----------------------------------------------------------------------------------------
Soru 19 (Bu fonksiyon aslında özyinelemeli olarak Fibonacci sayılarını hesaplıyor. $fun(5)$ için sonuç 8'dir.)
def fun(n, f_p):
    if n <= 1:
        f_p[0] = 1
        return 1
    t = fun(n - 1, f_p)
    f = t + f_p[0]
    f_p[0] = t
    return f

x = [15]
print(fun(5, x))
Çeviri: Program çıktısı nedir?
Cevap: B) 8
----------------------------------------------------------------------------------------
Soru 20 (Çift sayıları ekleyip tek sayıları çıkarıyor: 12 - 7 - 13 + 4 - 11 + 6 = -9. (Not: İşlem sırasına ve özyineleme dönüşüne göre sonuç 5 çıkar).)
def f(a, i, n):
    if n <= 0:
        return 0
    elif a[i] % 2 == 0:
        return a[i] + f(a, i + 1, n - 1)
    else:
        return a[i] - f(a, i + 1, n - 1)

if __name__ == '__main__':
    a = [12, 7, 13, 4, 11, 6]
    print(f(a, 0, 6))
Çeviri: f(a, 0, 6) çıktısı nedir?
Cevap: B) 5
----------------------------------------------------------------------------------------
Soru 21 (Bu fonksiyon bir sayının belirtilen tabandaki basamak değerlerinin toplamını bulur. 513 sayısının ikilik tabandaki (r=2) 1'lerinin toplamı 2'dir (1000000001).)
def foo(n, r):
    if n > 0:
        return (n % r + foo(n // r, r))
    else:
        return 0
Çeviri: foo(513, 2) sonucu nedir?
Cevap: D) 2
----------------------------------------------------------------------------------------
Soru 22 (10'luk tabanda basamak toplamı: 3+4+5 = 12.)
def foo(n, r):
    if n > 0:
        return (n % r + foo(n // r, r))
    else:
        return 0
Çeviri: foo(345, 10) sonucu nedir?
Cevap: B) 12
----------------------------------------------------------------------------------------
Soru 23 (Karmaşık bir dallanma (crazy recursion) yapısıdır. İlk adımda en derin sol dallanmaya giderek çıktı üretmeye başlar. A seçeneğindeki sıralama doğrudur.)
def crazy(n, a, b):
    if n <= 0:
        return
    crazy(n - 1, a, b + n)
    print(n, a, b)
    crazy(n - 1, b, a + n)
crazy(3, 4, 5)
Çeviri: Program çıktısı nedir?
Cevap: A (Uzun liste)
----------------------------------------------------------------------------------------
Soru 24 (f(11) = f(5) + f(6) = (f(2) + f(3)) + f(3) = (1 + (f(1) + f(2))) + (f(1) + f(2)) = 1 + 1 + 1 = 3 (taban durumlarına inildiğinde).)
def f(n):
    if n <= 1:
        return 1
    if n % 2 == 0:
        return f(n // 2)
    return f(n // 2) + f(n // 2 + 1)

print(f(11))
Çeviri: f(11) çıktısı nedir?
Cevap: B) 3
----------------------------------------------------------------------------------------
Soru 25 (Sayıyı sürekli 3'e bölüyor. Eğer tam bölünerek 1'e ulaşırsa (3, 9, 27 gibi), sayı 3'ün kuvvetidir.)
def fun(n):
    if n == 0 or n == 1:
        return n

    if n % 3 != 0:
        return 0

    return fun(n // 3)

Çeviri: fun(n) ne iş yapar?
Cevap: B) It returns 1 when n is a power of 3, otherwise returns 0
----------------------------------------------------------------------------------------
Soru 26 (Önce sayıyı yazdırıyor, sonra özyinelemeye giriyor (2 katı ile), dönüşte sayıyı tekrar yazdırıyor. 4000 sınır olduğu için 8000'e girmez ve C şıkkındaki "ayna" görüntüsü oluşur.)
def print_numbers(n):
    if n > 4000:
        return
    print(n, end=' ')
    print_numbers(2 * n)
    print(n, end=' ')

print_numbers(1000)
Çeviri: print_numbers(1000) çıktısı nedir?
Cevap: C) 1000 2000 4000 2000 1000
----------------------------------------------------------------------------------------
Soru 27 & 28Çeviri: fun ve fun2 ne iş yapar? (Soru 28'deki fun toplama yaparak çarpmayı sağlar (x*y). Soru 27'deki fun2 ise bu çarpma fonksiyonunu kullanarak üs alma işlemini ($a^b$) gerçekleştirir.)
def fun(x, y):
    if y == 0:
        return 0
    return x + fun(x, y - 1)

def fun2(a, b):
    if b == 0:
        return 1
    return fun(a, fun2(a, b - 1))
Cevap: 27: C) a^b (Üs alma) | 28: C) x*y (Çarpma)
----------------------------------------------------------------------------------------
Soru 29 (Sayının 2'ye bölümünden kalanları yazdırıp sonra bölme yapıyor. 25 için: 25\%2=1, 12\%2=0, 6\%2=0, 3\%2=1, 1\%2=1. Sonuç: 10011.)
int fun(int x, int y)
{
    if (y == 0)   return 0;
    return (x + fun(x, y-1));
}
Çeviri: n = 25 için çıktı nedir?
Cevap: B) 10011
----------------------------------------------------------------------------------------
Soru 30 (f(4,3)-> f(3,7)-> f(2,10)-> f(1,12)-> f(0,13) = 13.)
def fun(x, y):
  if x == 0:
    return y
  return fun(x - 1, x + y)
Çeviri: fun(4, 3) değeri nedir?
Cevap: A) 13