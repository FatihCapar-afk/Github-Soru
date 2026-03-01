Soru 1 (Matrislerde hücre adresleri doğrudan hesaplanabildiği için erişim hızı sabittir.)
Soru: Satır ve sütun indeksleri verilen bir 2D matriste bir elemana erişmenin zaman karmaşıklığı nedir?
Cevap: A) O(1)
----------------------------------------------------------------------------------------
Soru 2 (Tüm matris sıralı bir dizi gibi düşünülebildiği için ikili arama (binary search) ile logaritmik sürede arama yapılabilir.)
Soru: Satır öncelikli (row-major) sıralanmış bir matriste bir elemanı aramanın zaman karmaşıklığı nedir?
Cevap: C) O(\log(m*n))
----------------------------------------------------------------------------------------
Soru 3 (90 derece döndürme işleminde satırlar ilgili sütun pozisyonlarına dikey olarak yerleşir.)
Soru: Kare bir matrisi saat yönünde 90 derece döndürmenin sonucu ne olur?
Cevap: D) İlk satır ilk sütun olur, ikinci satır ikinci sütun olur ve bu şekilde devam eder.
----------------------------------------------------------------------------------------
Soru 4 (Matris sıralı olmadığı için her bir elemanı en az bir kez kontrol etmek zorunludur.)
Soru: m*n boyutundaki sıralanmamış bir matriste en küçük (minimum) elemanı bulmanın zaman karmaşıklığı nedir?
Cevap: A) O(m*n)
----------------------------------------------------------------------------------------
Soru 5 (Kod, matrisin köşegenine göre elemanları takas ederek satırları sütunlara dönüştürür.)
Kod:
def transpose_matrix(matrix):
    for i in range(len(matrix)):
        for j in range(i, len(matrix[0])):
            matrix[i][j], matrix[j][i] = matrix[j][i], matrix[i][j]
    return matrix
Soru: Yukarıdaki Python kodu verildiğinde, bu fonksiyonun çıktısı ne olacaktır?
Cevap: B) Orijinal matris yerinde (in-place) transpoze edilir.
----------------------------------------------------------------------------------------
Soru 6 (Kod, sınırları (top, bottom, left, right) daraltarak matrisi dıştan içe doğru dolanır.)
Kod:
def func(matrix):
    result = []
    if not matrix:
        return result
    top, bottom, left, right = 0, len(matrix)-1, 0, len(matrix[0])-1
    while top <= bottom and left <= right:
        for i in range(left, right + 1):
            result.append(matrix[top][i])
        top += 1
        for i in range(top, bottom + 1):
            result.append(matrix[i][right])
        right -= 1
        if top <= bottom:
            for i in range(right, left - 1, -1):
                result.append(matrix[bottom][i])
            bottom -= 1
        if left <= right:
            for i in range(bottom, top - 1, -1):
                result.append(matrix[i][left])
            left += 1
    return result
Soru: Yukarıdaki kod verildiğinde, func fonksiyonu ne döndürür?
Cevap: C) Matrisin elemanlarını spiral düzende döndürür.
----------------------------------------------------------------------------------------
Soru 7 (2D Prefix Sum mantığında her hücre, kendisinin sol üstünde kalan alanın toplamını tutar.)
Kod:
void prefixSum2D(int a[][C]) {
    int psa[R][C];
    psa[0][0] = a[0][0];
    for (int i = 1; i < C; i++)
        psa[0][i] = psa[0][i - 1] + a[0][i];
    for (int i = 1; i < R; i++)
        psa[i][0] = psa[i - 1][0] + a[i][0];
    for (int i = 1; i < R; i++) {
        for (int j = 1; j < C; j++)
            psa[i][j] = psa[i - 1][j] + psa[i][j - 1] - psa[i - 1][j - 1] + a[i][j];
    }
}
Soru: Tamamı 1'lerden oluşan 3x3'lük bir matris üzerinde bu fonksiyon çalıştırılırsa çıktı ne olur?
Cevap: B) [[1, 2, 3], [2, 4, 6], [3, 6, 9]]
----------------------------------------------------------------------------------------
Soru 8 (Dıştaki döngü sütunları (j), içteki döngü satırları (i) döndüğü için tarama sütun sütun gerçekleşir.)
Kod:
def traversal(matrix):
    result = []
    if not matrix:
        return result
    rows, cols = len(matrix), len(matrix[0])
    for j in range(cols):
        for i in range(rows):
            result.append(matrix[i][j])
    return result
Soru: Yukarıdaki kod verilen matris üzerinde ne tür bir işlem yapar?
Cevap: D) Matrisin elemanlarını sütun bazlı (column-wise) sırada döndürür.
----------------------------------------------------------------------------------------
Soru 9 (Satır indeksi artarken, sütun indeksinin toplam eleman sayısından geriye doğru gelmesi gerekir.)
Soru: Bir n*n kare matrisin "non-leading diagonal" (ikincil köşegen - sağ üstten sol alta) elemanlarını yazdıran sözde kod hangisidir?
Cevap: A) For i = 0 to n-1: Print matrix[i][n-1-i]