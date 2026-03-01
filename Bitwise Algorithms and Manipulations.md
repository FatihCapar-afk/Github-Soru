Question 1 (XOR operatörünün x \oplus x = 0 ve x \oplus 0 = x özellikleri sayesinde üç adımda iki değişkenin değeri birbirine aktarılabilir.)
Soru: İki sayıyı (geçici değişken kullanmadan) takas etmek (swap) için hangi bit düzeyinde operatör kullanılır?

Cevap: D) Bitwise XOR ^
----------------------------------------------------------------------------------------
Question 2 (Bu algoritma bir sayının ikili (binary) temsilindeki 1'lerin sayısını hesaplar. 15'in ikili karşılığı 1111 olduğu için sonuç 4'tür.)
Soru: num = 15 girdisi için aşağıdaki kodun çıktısı nedir?

Python
def fun(n):
    count = 0
    while n:
        count += n & 1
        n >>= 1
    return count
Cevap: C) 4
----------------------------------------------------------------------------------------
Question 3 (%x sayıyı sadece hex formatında yazdırırken, # bayrağı (flag) başına teknik ön ek olan 0x eklenmesini sağlar.)
Soru: Onaltılık (hexadecimal) gösterimde sayının başına 0x ekleyerek yazdırmak için kullanılan biçim belirleyici hangisidir?

Cevap: D) %#x
----------------------------------------------------------------------------------------
Question 4 (Bir biti 1 ile XOR işlemine sokmak, o bit 0 ise 1, 1 ise 0 yapar (yani tersine çevirir).)
Soru: Aşağıdakilerden hangisi bir biti tersine çevirme (toggling) operatörüdür?

Cevap: B) Bitwise XOR Operator (^)
----------------------------------------------------------------------------------------
Question 5 (Bit düzeyinde VEYA (OR) işlemi, karşılaştırılan bitlerden en az biri 1 ise sonucu 1 yapar. 000111 | 001010 = 011111 (İkilik sistemde toplama gibi çalışır ancak taşıma yapmaz).)
Soru: Aşağıdaki ifadenin çıktısı nedir? 000111 | 01010

Cevap: C) 010111
----------------------------------------------------------------------------------------
Question 6 (Bir maske oluşturup ~ ile ters çevirdikten sonra sayı ile & işlemine sokmak (örn: n & ~mask), maskelenen bitleri 0 yapar.)
Soru: Bit düzeyinde & (AND), bir sayıdaki 1 veya daha fazla biti kapatmak için ~ (NOT) operatörü ile birlikte kullanılabilir.

Cevap: A) True
----------------------------------------------------------------------------------------
Question 7 (Bit düzeyinde toplama mantığında XOR işlemi "elde hariç toplamı" verir, AND işlemi ise sadece "eldeleri" bulur.)
Soru: İki sayıyı elde (carry) olmadan toplamak için hangi bit düzeyinde operatör kullanılmalıdır?

Cevap: D) None (Aslında XOR toplama yapar ama şıklarda XOR tek başına değil).
----------------------------------------------------------------------------------------
Question 8 (Python'da negatif sayılar için sağa kaydırma, sayıyı 2'ye bölüp aşağı yuvarlar (floor division). -5 // 2 = -3.)
Soru: Çıktıyı tahmin edin:
# x is initialized to -5
x = -5
# Right shift operation
x = x >> 1
# Print the result
print(x)
Cevap: B) -3
----------------------------------------------------------------------------------------
Question 9 (~0 (NOT 0) işlemi tüm bitleri ters çevirerek -1 sonucunu verir. -1 == 1 ifadesi yanlış olduğu için "No" yazdırılır.)
Soru: Aşağıdaki kodun çıktısı nedir?

Python
if ~0 == 1:
    print("Yes")
else:
    print("No")
Cevap: B) No
----------------------------------------------------------------------------------------
Question 10 (Belirli bir konumdaki biti 1 yapmak (set etmek) için 1 << pos ile bir maske oluşturulur ve | (OR) ile sayıya uygulanır.)
Soru: Aşağıdaki kod ne yapar?

def set_bit(num, pos):
    return num | (1 << pos)
Cevap: D) set the given position (pos) of a number (num).
----------------------------------------------------------------------------------------
Question 11 (5 sayısı 101 şeklindedir. 2. bit (0'dan başlayarak) 1'dir. Kod bu bitin "dolu" (set) olup olmadığını kontrol eder.)
Soru: N = 5 ve K = 2 için aşağıdaki kodun çıktısı nedir?

def function(n, k):
    bit = n & (1 << k)
    return bool(bit)
Cevap: D) 1 (Python'da True döner, sayısal olarak 1 kabul edilir).
----------------------------------------------------------------------------------------
Question 12 (Kaydırma operatörleri doğrudan kare almasa da, 2'nin kuvvetleri ile çarpma/bölme işlemlerinde kullanılır; ancak genel kare alma bit düzeyinde tek bir operatörle değil, çarpma mantığıyla yapılır. (Soru bağlamında kaydırmalar üstel işlemlerle ilgilidir).)
Soru: Hangi bit düzeyinde operatörü kullanarak bir sayının karesini bulabiliriz?

Cevap: D) Left shift (<<) and right shift(>>)
----------------------------------------------------------------------------------------
Question 13 (İki sayının işaret bitleri farklıysa XOR işleminin sonucu negatiftir. Kod, sayılardan birinin pozitif diğerinin negatif olup olmadığını kontrol eder.)
Soru: Aşağıdaki kod ne yapar?

def fun(x, y):
	return (x ^ y) < 0
Cevap: B) Check the numbers are of same signs or not.
----------------------------------------------------------------------------------------
Question 14 (Bu "Brian Kernighan" algoritmasıdır. Her adımda en sağdaki 1 bitini silerek toplam 1'lerin sayısını çok hızlı bulur.)
Soru: Aşağıdaki kod parçacığında ne yapıyoruz?

def function(n):
    count = 0
    while n:
        n &= (n - 1)
        count += 1
    return count
Cevap: A) finding the number of set bits present in the n.
----------------------------------------------------------------------------------------
Question 15 (ASCII tablosunda büyük ve küçük harf arasındaki fark 32'dir ($2^5$). 32. biti temizlemek (& ~32), küçük harfi büyük harfe dönüştürür.)
Soru: Aşağıdaki kod parçacığı ne yapar? (x = 32)

def function(a):
    return ''.join(chr(ord(char) & ~x) for char in a)
Cevap: C) convert the characters into uppercase letters.
----------------------------------------------------------------------------------------
Question 16 (Dizideki tüm elemanlar XOR'lanırsa, çift sayıda tekrar edenler birbirini yok eder (x \oplus x = 0). Tek sayıda kalan eleman (bu örnekte 9) sonuç olarak döner.)
Soru: Verilen dizi için fonksiyonun dönüş değeri nedir? arr[] = {9, 12, 2, 11, 2, 2, 10, 9, 12, 10, 9, 11, 2}

Cevap: B) 9
----------------------------------------------------------------------------------------
Question 17 (Bir kümedeki her eleman, alt kümeler oluşturulduğunda eşit sayıda (çift sayıda) görünür. Çift sayıda aynı sayının XOR toplamı her zaman 0'dır.)
Soru: {1, 2, 3} kümesinin tüm alt kümelerinin XOR toplamını bulun.

Cevap: D) 0
----------------------------------------------------------------------------------------
Question 18 (~ (NOT) operatörü sadece bir sayı üzerinde işlem yapar, diğerleri (&, |, ^) iki sayı gerektirir.)
Soru: Aşağıdakilerden hangisi tek işlenenli (unary) bir operatördür?

Cevap: B) ~ Bitwise Negate Operator
----------------------------------------------------------------------------------------
Question 19 (Sayıyı sürekli 2'ye bölüp kalanları ters sırada yazdıran özyinelemeli (recursive) bir ikilik sistem dönüştürücüsüdür.)
Soru: Aşağıdaki kod ne yapar?

def bin(n):
    if n > 1:
        bin(n // 2)
    print(n % 2, end='')
Cevap: C) print the binary representation of a number
----------------------------------------------------------------------------------------
Question 20 (128, 2'nin 7. kuvvetidir (2^7). Kod, sayının içindeki tek 1 bitinin pozisyonunu bulur (1'den başladığı için 7+1=8).)
Soru: N = 128 için aşağıdaki kodun çıktısı nedir?

Cevap: D) 8
----------------------------------------------------------------------------------------
Question 21 (Eğer sayının son biti 1 ise sayı tektir, 0 ise çifttir. n & 1 işlemi bu son biti kontrol eder.)
Soru: Bit düzeyinde operatör kullanarak sayının tek mi çift mi olduğunu anlamak için boşluğa ne gelmelidir?

Cevap: B) n & 1
----------------------------------------------------------------------------------------
Question 22 (Bir sayının bitlerini ters çevirip (~) 1 eklemek, o sayının negatifini elde etmeyi sağlayan "2'ye tümleyen" (2's complement) yöntemidir. Sonuç -5 olur.)
Soru: Aşağıdaki kod ne yapar? (num = 5)

print(~num + 1)
Cevap: A) It will print 2's complement of a number.
----------------------------------------------------------------------------------------
Question 23 (Bit düzeyinde DEĞİL (NOT) operatörü tüm 0'ları 1, 1'leri 0 yapar.)
Soru: Bir sayının tüm bitlerini tersine çevirmek (invert) için hangi operatör kullanılmalıdır?

Cevap: A) ~
----------------------------------------------------------------------------------------
Question 24 (Listenin tüm elemanlarını ve olması gereken tüm sayıları (1'den 6'ya) birlikte XOR'larsanız, mevcut olanlar birbirini yok eder ve geriye sadece eksik olan sayı kalır.)
Soru: 1'den 6'ya kadar olan sayılardan biri eksik olan 5 elemanlı bir listede eksik sayıyı hangi ifade verir?

Cevap: B veya C (İfadeye göre 1-6 arası tüm sayılarla listenin XOR'lanması gerekir).
----------------------------------------------------------------------------------------
Question 25 (Sağa kaydırma sayıyı 2'ye böler, sola kaydırma ise 2 ile çarpar.)
Soru: Sağa kaydırma (>>) ve Sola kaydırma (<<), sırasıyla 2 ile hangi işleme eşdeğerdir?

Cevap: B) Divide and multiply
----------------------------------------------------------------------------------------
Question 26 (1'den N'e kadar olan sayıların ardışık XOR toplamı her 4 adımda bir kendini tekrar eden bir model izler; bu kod o modeli uygular.)
Soru: Aşağıdaki kod bit manipülasyonunda ne yapar?

def function(n):
    if n % 4 == 0: return n
    if n % 4 == 1: return 1
    if n % 4 == 2: return n + 1
    else: return 0
Cevap: D) It will give the xor of numbers from 1 to N.
----------------------------------------------------------------------------------------
Question 27 (& ~ (1 << k) işlemi, sayının $k$. bitini 0 yapmak (temizlemek) için kullanılan standart yöntemdir.)
Soru: Aşağıdaki kodun çıktısı nedir? (num = [7], k = 1)

Cevap: C) It will unset the kth bit of num
----------------------------------------------------------------------------------------
Question 28 (0 sayısı için de bu ifade True döner, ancak 0 bir 2'nin kuvveti değildir. Fonksiyonun x > 0 kontrolü de yapması gerekir.)
Soru: Sayının 2'nin kuvveti olup olmadığını kontrol eden aşağıdaki fonksiyondaki hata nedir?

def is_power_of_two(x):
    return (x & (x - 1)) == 0
Cevap: C) It does not work for x = 0
----------------------------------------------------------------------------------------
Question 29 (Bir sayıdan 1 çıkarıp kendisiyle AND işlemine sokmak, sayının en sağındaki (ilk karşılaşılan) 1 bitini 0'a dönüştürür.)
Soru: x = x & (x-1) ifadesi ne yapar?

Cevap: C) Turns off the rightmost set bit
----------------------------------------------------------------------------------------
Question 30 (x<<1 (2x) + x (1x) + x>>1 (0.5x$) toplamda 3.5x yapar.)
Soru: x = (x<<1) + x + (x>>1) ifadesi ne yapar?

Cevap: B) Multiplies an integer with 3.5