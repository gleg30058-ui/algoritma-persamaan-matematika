# Algoritma Menghitung X = a³ + b² + c

## 1. Penjelasan Persamaan

Persamaan yang akan kita hitung adalah:
```
X = a³ + b² + c
```

Dimana:
- **a³** = a dipangkatkan 3 (kubus dari a)
- **b²** = b dipangkatkan 2 (kuadrat dari b)
- **c** = nilai konstanta c
- **X** = hasil akhir penjumlahan ketiga komponen di atas

---

## 2. Langkah-Langkah Algoritma

### Pseudocode:

```
ALGORITMA HitungPersamaan(input: a, b, c)
BEGIN
    // Langkah 1: Deklarasi variabel
    DECLARE a, b, c AS INTEGER/FLOAT
    DECLARE hasil_a3, hasil_b2, X AS INTEGER/FLOAT
    
    // Langkah 2: Baca input nilai a, b, dan c
    INPUT a, b, c
    
    // Langkah 3: Hitung a pangkat 3
    hasil_a3 ← a * a * a
    // atau: hasil_a3 ← a^3
    
    // Langkah 4: Hitung b pangkat 2
    hasil_b2 ← b * b
    // atau: hasil_b2 ← b^2
    
    // Langkah 5: Hitung jumlah ketiga komponen
    X ← hasil_a3 + hasil_b2 + c
    
    // Langkah 6: Tampilkan hasil
    OUTPUT X
    
END
```

---

## 3. Flowchart

```
          ┌─────────────┐
          │   MULAI     │
          └──────┬──────┘
                 │
          ┌──────▼──────────┐
          │ INPUT a, b, c   │
          └──────┬──────────┘
                 │
          ┌──────▼────────────────┐
          │ hasil_a3 = a * a * a  │
          └──────┬────────────────┘
                 │
          ┌──────▼─────────────┐
          │ hasil_b2 = b * b   │
          └──────┬─────────────┘
                 │
          ┌──────▼───────────────────────────┐
          │ X = hasil_a3 + hasil_b2 + c      │
          └──────┬───────────────────────────┘
                 │
          ┌──────▼──────────────┐
          │ OUTPUT X            │
          └──────┬──────────────┘
                 │
          ┌──────▼─────────┐
          │   SELESAI       │
          └─────────────────┘
```

---

## 4. Kompleksitas Algoritma

### Kompleksitas Waktu (Time Complexity):
- **O(1)** - Waktu konstan
- Karena algoritma hanya melakukan operasi dasar:
  - 2 operasi perkalian untuk menghitung a³
  - 1 operasi perkalian untuk menghitung b²
  - 2 operasi penjumlahan
  - Total = 5 operasi, yang merupakan konstanta

### Kompleksitas Ruang (Space Complexity):
- **O(1)** - Ruang konstan
- Hanya menggunakan beberapa variabel (a, b, c, hasil_a3, hasil_b2, X)
- Tidak bergantung pada ukuran input

---

## 5. Contoh Eksekusi Manual

### Contoh 1:
```
Input:
  a = 2
  b = 3
  c = 5

Proses:
  hasil_a3 = 2 * 2 * 2 = 8
  hasil_b2 = 3 * 3 = 9
  X = 8 + 9 + 5 = 22

Output: X = 22
```

### Contoh 2:
```
Input:
  a = 3
  b = 4
  c = 1

Proses:
  hasil_a3 = 3 * 3 * 3 = 27
  hasil_b2 = 4 * 4 = 16
  X = 27 + 16 + 1 = 44

Output: X = 44
```

### Contoh 3:
```
Input:
  a = 1
  b = 1
  c = 1

Proses:
  hasil_a3 = 1 * 1 * 1 = 1
  hasil_b2 = 1 * 1 = 1
  X = 1 + 1 + 1 = 3

Output: X = 3
```

---

## 6. Keuntungan dan Kekurangan

### ✅ Keuntungan:
- **Sederhana**: Logika algoritma sangat mudah dipahami
- **Efisien**: Kompleksitas waktu dan ruang sangat kecil (O(1))
- **Cepat**: Eksekusi sangat cepat karena hanya operasi aritmatika dasar
- **Fleksibel**: Bisa diimplementasikan di hampir semua bahasa pemrograman

### ❌ Kekurangan:
- **Tidak scalable untuk persamaan kompleks**: Jika persamaan lebih rumit, algoritma ini tidak mudah dikembangkan
- **Input terbatas**: Hanya menerima 3 parameter input

---

## 7. Variasi Implementasi

Algoritma ini dapat diimplementasikan dengan beberapa cara:

1. **Cara 1 - Langsung tanpa variabel antara:**
   ```
   X = (a*a*a) + (b*b) + c
   ```

2. **Cara 2 - Menggunakan fungsi power:**
   ```
   X = pow(a, 3) + pow(b, 2) + c
   ```

3. **Cara 3 - Menggunakan operator perpangkatan (jika tersedia):**
   ```
   X = a^3 + b^2 + c
   ```

---

## 8. Kasus Khusus

| Kondisi | Hasil |
|---------|-------|
| a = 0, b = 0, c = 0 | X = 0 |
| a = -2, b = 3, c = 1 | X = -8 + 9 + 1 = 2 |
| a = 0, b = 5, c = -3 | X = 0 + 25 - 3 = 22 |
| a = 1, b = 0, c = 0 | X = 1 + 0 + 0 = 1 |

---

Sekarang Anda memiliki pemahaman lengkap tentang algoritma ini! Apakah Anda ingin saya membuat implementasi kode dalam bahasa pemrograman tertentu?
