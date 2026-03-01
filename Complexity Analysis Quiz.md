Soru 1 (Soru 1: Diziye indeks ile erişimin anında, yani O(1) sabit zaman karmaşıklığında gerçekleştiğini anlatıyor.)
What is the worst-case time complexity of accessing an element in an array using its index in a typical C++ or Python program?

Cevap: O(1)
----------------------------------------------------------------------------------------
Soru 2 (İç içe iki döngünün (biri n, diğeri m kere dönen) toplam çalışma zamanının çarpılarak (O(n * m)) hesaplandığını öğretiyor.)
In a fundamental algorithm, what is the time complexity of a nested loop structure where the outer loop iterates x times and the inner loop iterates y times?

Cevap: O(x * y)
----------------------------------------------------------------------------------------
Soru 3 (Görünüşte tek bir döngü olsa bile, döngünün bitiş şartı n^2 olduğu için zaman karmaşıklığının O(n^2) olacağını gösteriyor.)
Consider a basic program that takes a dataset of size k and runs a single loop from 1 to k^2. What is the asymptotic time complexity of this algorithm?

Cevap: O(k^2)
----------------------------------------------------------------------------------------
Soru 4 (Big-O notasyonunun algoritmanın en kötü senaryosunu (üst sınır - upper bound) temsil ettiğini test ediyor.)
In our Data Structures class, which of the following is taught as the true definition of the Big O notation (O(f(n)))?

Cevap: It describes the upper bound of the runtime of an algorithm.
----------------------------------------------------------------------------------------
Soru 5 (Asimptotik notasyonların (Big-O: En kötü durum, Omega: En iyi durum, Theta: Ortalama durum) teorik eşleştirmesini öğretiyor.)
Match the asymptotic notations with the parameters they typically define in algorithm analysis:

Cevap: Big-O Notation (O-notation) : Worst Case complexity, Omega Notation (Ω-notation) : Best Case complexity, Theta Notation (Θ-notation) : Average Case complexity
----------------------------------------------------------------------------------------
Soru 6 (Karesel O(n^2) bir algoritmada veri boyutu 2 katına çıkarsa, çalışma süresinin $2^2$ yani 4 katına çıkacağını hatırlatıyor.)
If an encryption algorithm’s time complexity is O(n^2), which of the following best describes its performance when the input size is doubled?

Cevap: The time taken will quadruple.
----------------------------------------------------------------------------------------
Soru 7 (O(n) lineer zaman karmaşıklığında, çalışma süresinin veri boyutuyla (girdiyle) doğru orantılı olarak arttığını anlatıyor.)
When we say a simple search algorithm runs in O(n) time complexity, what does it indicate?

Cevap: The algorithm's execution time grows linearly with the input size.
----------------------------------------------------------------------------------------
Soru 8 (Her adımda kendini 2 kere çağıran özyineli (recursive) bir fonksiyonun çalışma süresinin üssel (O(2^n)) büyüdüğünü gösteriyor.)
Determine the time complexity for the following recursive pseudo-code used in our lab:
def recursive_func(k):
if k <= 1:
return 1
else:
return recursive_func(k - 1) + recursive_func(k - 1)

Cevap: O(2^k)
----------------------------------------------------------------------------------------
Soru 9 (Merge Sort gibi veriyi sürekli ikiye bölüp sonra birleştiren "parçala ve fethet" algoritmalarının O(n log n) hızında çalıştığını öğretiyor.)
What is the time complexity of the standard Merge Sort implementation below? (Note: The merge function takes linear time.)
def merge_sort(arr):
if len(arr) <= 1:
return arr
mid = len(arr) // 2
left = merge_sort(arr[:mid])
right = merge_sort(arr[mid:])

return merge(left, right)
Cevap: O(n log n)
----------------------------------------------------------------------------------------
Soru 10 (Her adımda 3 farklı dala ayrılan (branching factor = 3) özyineli bir yapının n derinliğinde O(3^n) zaman karmaşıklığına ulaşacağını test ediyor.)
Consider a recursive tree-traversal function with a branching factor of 3 and a maximum depth of N. What would be the time complexity of this recursion?

Cevap: O(3^n)
----------------------------------------------------------------------------------------
Soru 11 (Bir dizideki en büyük elemanı bulmak için dizinin tüm elemanlarını bir kez sırayla gezmek (O(n)) gerektiğini anlatıyor.)
What is the time complexity for this simple maximum-finding code?
def find_max_value(arr):
max_val = arr[0]
for i in range(1, len(arr)):
if arr[i] > max_val:
max_val = arr[i]
return max_val

Cevap: O(n)
----------------------------------------------------------------------------------------
Soru 12 (Dizideki elemanları birbiriyle kıyaslamak veya çarpmak için kullanılan iç içe iki döngünün O(n^2) zaman aldığını gösteriyor.)
What is the time complexity of this nested loop snippet that compares array elements?
for i in range(len(arr) - 1):
for j in range(i + 1, len(arr)):
print(arr[i] * arr[j])

Cevap: O(n^2)
----------------------------------------------------------------------------------------
Soru 13 (Sadece belirli indekslerdeki elemanları okuyup işlem yapmanın veri boyutundan bağımsız, sabit zamanda (O(1)) gerçekleştiğini test ediyor.)
What is the time complexity of this simple array access function?
def access_element(arr, index):
return arr[index] * arr[index + 1]

Cevap: O(1)
----------------------------------------------------------------------------------------
Soru 14 (Binary Search (İkili Arama) algoritmasının her adımda arama alanını yarıya indirdiği için logaritmik (O(log n)) sürede çalıştığını anlatıyor.)
Determine the time complexity for this standard binary search implementation.
def binary_search_algo(arr, target):
low = 0
high = len(arr) - 1
while low <= high:
mid = (low + high) // 2
if arr[mid] == target:
return mid
elif arr[mid] < target:
low = mid + 1
else:
high = mid - 1
return -1

Cevap: O(log n)
----------------------------------------------------------------------------------------
Soru 15 (Asal sayı kontrolünde döngüyü sayının kendisine kadar değil, sadece kareköküne kadar (O(√n)) çalıştırmanın kod optimizasyonu için yeterli olduğunu gösteriyor.)
What is the time complexity of this optimized prime number checker algorithm?
def is_prime_num(n):
if n <= 1:
return False
for i in range(2, int(math.sqrt(n)) + 1):
if n % i == 0:
return False
return True

Cevap: O(√n)
----------------------------------------------------------------------------------------
Soru 16 (Bir algoritmada O(n^3) zaman karmaşıklığına ulaşmak için iç içe 3 tane döngü (nested loops) kullanılması gerektiğini öğretiyor.)
Which of the following script structures will result in a time complexity of O(n^3) in an algorithm?

Cevap: A program with 3 nested loops
----------------------------------------------------------------------------------------
Soru 17 (İç içe geçmiş n adet döngünün (her biri m kere çalışıyorsa) çalışma süresinin üssel olarak nasıl hesaplanacağını test ediyor.)
What would be the time complexity of a code that contains k nested loops, each running from 1 to p?

Cevap: O(p^k)