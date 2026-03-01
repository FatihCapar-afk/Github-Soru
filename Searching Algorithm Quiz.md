Soru 1 (Eğer x dizideki en büyük sayıdan bile büyükse, i değişkeni sürekli artarak dizinin uzunluğu olan n değerine ulaşır. Döngü bitip alt satıra geçildiğinde a[i] yani a[n] çağrılır, ancak son indeks n-1 olduğu için program "Index Error" verir.)
Aşağıdaki program, sıralı (sorted) bir a[] dizisinde x elemanını "İkili Arama" (Binary Search) kullanarak bulmaya çalışıyor. N > 1 olduğunu varsayalım. Bu programda mantıksal bir hata var. Hangi durumda bu program başarısız olur ve çöker (Out of Bounds hatası vb. verebilir)?

def find(a, n, x):
i = 0
j = n
while i < j:
k = (i + j) // 2
if a[k] < x:
i = k + 1
else:
j = k

if i < len(a) and a[i] == x:
    print("x is in the array")
else:
    print("x is not in the array")
Cevap: x is greater than all elements of the array a[] (Aranan x elemanı, dizideki tüm elemanlardan büyükse)
----------------------------------------------------------------------------------------
Soru 2 ("Doğrusal", elemanların baştan sona tek tek, bir "dizi" (sequence) halinde kontrol edildiğini ifade eder. Bu yüzden İngilizce literatürde genellikle "Sequential Search" olarak da geçer.)
Doğrusal Arama (Linear Search) algoritmasının diğer adı nedir?

Cevap: Ardışık Arama (Sequential search)
----------------------------------------------------------------------------------------
Soru 3 (Dizi zaten sıralı verildiği için, elemanları tek tek gezmek (O(n)) yerine, İkili Arama (Binary Search) tekniği hafifçe modifiye edilerek tavan değeri logaritmik sürede çok hızlıca bulunabilir.)
Sıralı bir tamsayı dizisinde, verilen bir x sayısının "tavanını" (ceiling) bulmak için gereken en kötü durum (worst-case) zaman karmaşıklığı nedir?
(Tavan, dizideki x'ten büyük veya ona eşit olan en küçük elemandır. Örn: dizi = {12, 67, 90, 100, 300, 399}, x = 95 ise tavan 100'dür).

Cevap: O(log(n))
----------------------------------------------------------------------------------------
Soru 4 (En yavaşı tek tek bakan Linear Search'tür (O(N)). Jump search bloklar atlayarak aradığı için daha hızlıdır (O(√N)). Binary search ise veriyi sürekli yarıya böldüğü için içlerinde en hızlı olanıdır (O(log N)).)
Arama algoritmalarının performanslarını (yavaş çalışandan hızlı çalışana doğru) sıralayınız:

Cevap: linear search < jump search < binary search
----------------------------------------------------------------------------------------
Soru 5 (En iyi durum (Best Case) elemanın en başta (1. adımda) bulunmasıdır. En kötü durum (Worst Case) en sonda veya hiç olmamasıdır. Ortalama durum ise istatistiksel olarak elemanın dizinin ortalarında (~ N/2. adımda) bulunmasıdır.)
Doğrusal Arama (Linear Search) algoritmasında "ortalama durum" (average case) ne zaman gerçekleşir?

Cevap: Aranan eleman dizinin orta kısımlarında bir yerlerde bulunduğunda.
----------------------------------------------------------------------------------------
Soru 6 (Bu hatalı bir kod blokudur. İki if şartı birbirini bozar. x == listA[k] olduğunda hem j hem de i değişir. Döngü bittiğinde k hedefi göstermez, bu yüzden alttaki kontrol her zaman başarısız olup -1 döner.)
Aşağıdaki fonksiyon sıralı (artan) bir listA dizisini işlemektedir. Bu kod parçası hakkında hangi ifade DOĞRUDUR?

def ProcessArray(listA, x, n):
i = 0
j = n - 1
while i <= j:
k = (i + j) // 2
if x <= listA[k]:
j = k - 1
if listA[k] <= x:
i = k + 1
if listA[k] == x:
return k
else:
return -1

Cevap: x dizide bulunsa bile fonksiyon her zaman -1 döndürür. (It will return −1 even when x is present in listA.)
----------------------------------------------------------------------------------------
Soru 7 (İlk elemanı bulma ihtimali 1, son elemanı bulma ihtimali n'dir. Eşit olasılıklı bir dağılımda ortalama adım sayısı (1+2+3+...+n) / n matematiksel işlemi sonucu (n+1)/2 çıkar. (Pratikte n/2 gibi düşünülür).)
n uzunluğundaki bir listede "başarılı" (elemanın kesinlikle dizide olduğu) bir ardışık (sequential/linear) arama işleminde, ortalama olarak kaç adet anahtar karşılaştırması yapılır?

Cevap: (n+1)/2
----------------------------------------------------------------------------------------
Soru  (Binary search ortadaki elemana bakıp "sağa mı gideyim, sola mı gideyim" diye karar verir. Eğer dizi sıralı değilse (küçükten büyüğe/büyükten küçüğe), bu mantık tamamen çöker.)
Bir dizide İkili Arama (Binary Search) kullanabilmek için en temel şart nedir?

Cevap: Dizi sıralı (sorted) olmalıdır.
----------------------------------------------------------------------------------------
Soru 9 (Kodda da görüldüğü gibi, aranan aralığın sınırları 2'nin kuvvetleri şeklinde üssel (exponentially) olarak büyütülüyor. Hedefin olduğu aralık bulununca, sadece o dar alanda ikili arama (binary search) uygulanıyor.)
Aşağıdaki arama algoritmasının adı nedir?
(Kod önce i'yi 1, 2, 4, 8... şeklinde katlayarak aralığı bulur, sonra o aralıkta binary search yapar.)

Cevap: Üstel Arama (Exponential Search)
----------------------------------------------------------------------------------------
Soru 10 (Jump search, diziyi √N büyüklüğünde bloklara böler. En kötü senaryoda √N kadar sıçrama yapar ve hedef bloğun içinde de maksimum √N kadar doğrusal arama yapar. Optimal zamanı O(√N)'dir.)
Sıçramalı Arama (Jump Search) algoritmasının zaman karmaşıklığı nedir?

Cevap: O(√N)
----------------------------------------------------------------------------------------
Soru 11 (Algoritma her adımda işlenecek veriyi ikiye böldüğü için fonksiyon kendini T(n/2) olarak çağırır. Ortadaki elemanı kontrol etmek ise sabit zaman yani O(1) alır.)
İkili Arama'nın (Binary Search) en kötü durumu (worst case) için doğru özyinelemeli (recurrence) formül hangisidir?

Cevap: T(n) = T(n/2) + O(1) ve T(1) = T(0) = O(1)
----------------------------------------------------------------------------------------
Soru 12 (Dizi sıralı olduğu için ilk eleman bir for döngüsüyle (n kere) seçilir. Kalan iki eleman ise kalan dizi üzerinde (Two-Pointer tekniği ile) n zamanda aranır. Toplam süre n * n = O(n^2) olur. Kaba kuvvetle (iç içe 3 döngü) denenseydi O(n^3) olurdu.)
n elemanlı "sıralı" bir dizide, toplamı verilen bir x sayısına eşit olan "üçlü" (triplet) bir kombinasyonu bulmak için bilinen en iyi algoritmanın zaman karmaşıklığı nedir?

Cevap: O(n^2)
----------------------------------------------------------------------------------------
Soru 13 (Binary search aralığı tam ortadan 2'ye bölerken (1/2), Ternary search aralığı üç eşit parçaya böler. Bu nedenle toplam uzunluğun (right - left) 1/3'lük ve 2/3'lük noktaları hesaplanır.)
Üçlü Arama (Ternary Search) algoritmasında aralığı 3'e bölmek için kullanılan doğru iki orta nokta formülü hangisidir?

Cevap: mid1 = left + (right - left) / 3, mid2 = right - (right - left) / 3
----------------------------------------------------------------------------------------
Soru 14 (Algoritma tüm elemanları gezmek yerine, örneğin üçer üçer zıplar (0, 3, 6, 9...). Eğer aranan sayı 6. ve 9. indeks arasındaki bir değerden küçükse, hedefin bu blokta olduğunu anlayıp 6'dan 9'a kadar tek tek arar.)
Sıralı bir dizide Sıçramalı Arama (Jump Search), bir sonraki aramayı nereye yapacağına nasıl karar verir?

Cevap: Sabit bir blok boyutu kadar ileri zıplar (jump) ve uygun aralığı bulunca o blok içinde doğrusal (linear) arama yapar.
----------------------------------------------------------------------------------------
Soru 15 (İnterpolasyon araması telefon rehberi mantığıyla çalışır. Eğer aranan isim "Z" ile başlıyorsa ortadan başlamak yerine doğrudan rehberin sonuna atlar. Bu formülün çalışması için sayıların belli bir düzende artması (örneğin 10, 20, 30, 40...) gereklidir.)
İnterpolasyon Araması (Interpolation Search) kullanmak için en ideal durum (best use case) aşağıdakilerden hangisidir?

Cevap: Veriler sıralı olduğunda (sorted) ve "düzenli / eşit" bir dağılıma (uniformly distributed) sahip olduğunda.