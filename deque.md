Question 1 (Deque (Double-Ended Queue), elemanların hem en başından hem de en sonundan eklenip çıkarılabildiği çift uçlu bir kuyruk veri yapısıdır.)
Soru: Deque nedir?
Cevap: A) Kuyruğun hem ön hem de arka uçları için tanımlanmış ekleme/silme işlemlerine sahip bir yapıdır.
----------------------------------------------------------------------------------------
Question 2 (Deque'ler kullanım amacına göre özelleşebilir; Giriş Kısıtlamalı olanlarda ekleme sadece bir uçtan yapılırken, Çıkış Kısıtlamalı olanlarda silme işlemi sadece bir uçtan yapılır.)
Soru: Aşağıdakilerden hangileri kısıtlanmış deque (restricted deques) türleridir?

Cevap: A) Giriş Kısıtlamalı Deque (Input Restricted Deque) / Çıkış Kısıtlamalı Deque (Output Restricted Deque)
----------------------------------------------------------------------------------------
Question 3 (Python'daki collections.deque nesnesi doğrudan yazdırıldığında (print), içeriğini deque([...]) formatında gösterir.)
Soru: Verilen kodun çıktısı nedir?
from collections import deque
queue = deque(['name','age','DOB'])
print(queue)

Cevap: D) deque(['name', 'age', 'DOB'])
----------------------------------------------------------------------------------------
Question 5 (Her iki uçtan erişim gerektiği için çift yönlü bağlı liste (doubly-linked list) veya dairesel dizi (circular array) en yaygın uygulama yöntemleridir.)
Soru: Deque aşağıdakilerden hangisi kullanılarak uygulanabilir?

B) Çift yönlü bağlı liste
C) Çift yönlü bağlı liste
D) Dairesel bir dizi
Cevap: B, C veya D (Genelde verimlilik için Çift Yönlü Bağlı Liste veya Dairesel Dizi tercih edilir).
----------------------------------------------------------------------------------------
Question 6 (Deque her iki uçtan ekleme-çıkarmaya izin verdiği için hem LIFO (Yığın) hem de FIFO (Kuyruk) davranışlarını tek başına sergileyebilir.)
Soru: Deque ne olarak uygulanabilir?

A) Yığın (Stack) ve kuyruk (Queue)
Cevap: A
----------------------------------------------------------------------------------------
Question 7 (Python deque modülünde insert() metodu önce konumu (index), sonra eklenecek değeri (value) parametre olarak alır.)
Soru: Deque içinde 'i' pozisyonuna 'a' elemanını eklemek için doğru metot imzası hangisidir?

A) insert(position, element)
Cevap: A
----------------------------------------------------------------------------------------
Question 8 (extendleft fonksiyonu, verilen listedeki elemanları sırayla tek tek sol tarafa eklediği için, listenin orijinal sırası deque içerisinde tersine dönmüş olur.)
Soru: extendleft(iterable) ne için kullanılır?

A) Bu fonksiyon, deque'in sol ucuna birden fazla değer eklemek için kullanılır. Geçilen argüman yinelenebilir (iterable) olmalıdır. Sol eklemelerin bir sonucu olarak sıralama tersine döner.
Cevap: A
----------------------------------------------------------------------------------------
Question 9 (Deque veri yapısı, uç noktalara doğrudan erişim sağladığı için başa/sona ekleme ve çıkarma işlemlerini her zaman sabit sürede (O(1)) gerçekleştirir.)
Soru: Aşağıdakilerden hangisi doğrudur?

A) Deque, ekleme (append) ve çıkarma (pop) işlemleri için $O(1)$ zaman karmaşıklığı sağlar.
Cevap: A
----------------------------------------------------------------------------------------
Question 10 (Standart append() fonksiyonu, yeni bir elemanı veri yapısının en sonuna (sağ ucuna) eklemek için kullanılır.)
Soru: append() fonksiyonu ne için kullanılır?

D) Bu fonksiyon, argümanındaki değeri deque'in sağ ucuna eklemek için kullanılır.
Cevap: D