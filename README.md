# Uji Kompetensi DDP 2

Mata Kuliah Dasar Pemrograman, dengan bahasa C++

## Soal 1
```bash
### **STEP 4: Perbaiki Kode dan Tambahkan Komentar** 🔧

Buka file yang sudah Anda copy dengan text editor favorit: 

#### **Format Komentar yang Harus Ditambahkan:**

```cpp
// ============================================
// NAMA  : [Nama Lengkap Anda]
// NIM   :  [2500018XXX]
// QUIZ  : [Nama Quiz yang dipilih]
// TANGGAL: [DD/MM/YYYY]
// ============================================

#include <iostream>
using namespace std;

int faktorial(int n) {
    // ❌ KESALAHAN 1: Base case salah - seharusnya return 1, bukan 0
    // SEBELUM: if (n == 0) return 0;
    // PERBAIKAN: 
    if (n == 0 || n == 1) {  // ✅ DIPERBAIKI
        return 1;  // ✅ Faktorial 0 dan 1 adalah 1
    }
    
    // ❌ KESALAHAN 2: Operasi salah - harus perkalian (*), bukan penjumlahan (+)
    // SEBELUM: return n + faktorial(n - 1);
    // PERBAIKAN:
    return n * faktorial(n - 1);  // ✅ DIPERBAIKI - menggunakan perkalian
}

int main() {
    int angka;
    cout << "Masukkan angka:  ";
    cin >> angka;
    
    // ❌ KESALAHAN 3: Kondisi terbalik - harus angka < 0, bukan angka > 0
    // SEBELUM: if (angka > 0)
    // PERBAIKAN: 
    if (angka < 0) {  // ✅ DIPERBAIKI - cek bilangan negatif
        cout << "Faktorial tidak terdefinisi untuk bilangan negatif!" << endl;
    } else {
        cout << "Faktorial dari " << angka << " adalah: " << faktorial(angka) << endl;
    }
    
    return 0;
}

// ============================================
// RINGKASAN KESALAHAN YANG DITEMUKAN:
// 1. Base case return 0 → diperbaiki menjadi return 1
// 2. Operasi penjumlahan (+) → diperbaiki menjadi perkalian (*)
// 3. Kondisi angka > 0 → diperbaiki menjadi angka < 0
// ============================================

#### **📌 Format Komentar Wajib:**

Setiap kesalahan yang ditemukan HARUS diberi komentar dengan format:

```cpp
// ❌ KESALAHAN [nomor]:  [Penjelasan kesalahan]
// SEBELUM: [kode yang salah]
// PERBAIKAN:
[kode yang benar]  // ✅ DIPERBAIKI
```

## Hasil
 - User melakukan input yang diminta soal yaitu 5, 10, dan 1.
 
<img width="315" height="330" alt="image" src="https://github.com/user-attachments/assets/213da456-af29-4576-bc72-22a1c7d35004" />

## Penjelasan
menganalisis kesalahan pada fungsi rekursif yang diberikan. Setiap kesalahan diidentifikasi berdasarkan alur logika program dan hasil output yang tidak sesuai. 
Perbaikan dilakukan dengan memperbaiki base case rekursi, operasi rekursif, serta pemanggilan fungsi agar sesuai dengan spesifikasi soal. 
Setelah perbaikan, program diuji menggunakan beberapa test case untuk memastikan hasil sudah benar.

