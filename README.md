DASHBOARD PEMANTAUAN PERFORMA PACKING & QUALITY CONTROL (QC)



1. LATAR BELAKANG MASALAH

Pada lini produksi manufaktur pangan, proses packing merupakan titik krusial yang menentukan kualitas produk akhir sebelum sampai ke konsumen. Tanpa pemantauan berbasis data, tim produksi dan Quality Control (QC) kesulitan mengidentifikasi sumber reject terbesar, membedakan cacat yang bersifat constraint proses dengan cacat yang dapat segera diperbaiki, serta mengukur distribusi beban kerja antar tim (ASST, SPV, dan Operator).

Dashboard ini dibangun menggunakan Power BI untuk memantau performa output packing dan menganalisis akar penyebab reject secara terstruktur guna mendukung pengambilan keputusan perbaikan kualitas.



2. RINGKASAN METRIK UTAMA

Periode Data: [Periode Data : 01 November 2025 - 30-11-2025]

- Total Pack: 946K pack

- Total Berat Produksi: 264.53M [220 + 300 gram]

- Total Reject (ALL Reject): 25K 

- Overall Reject Rate: 2.65%



3. STRUKTUR DASHBOARD

Dashboard dibagi menjadi dua halaman utama agar alur pembacaan mengalir dari gambaran makro ke analisis akar masalah:



Halaman 1: Overview (Performa Produksi)

- KPI Cards: Menampilkan ringkasan Total Pack, Total Berat Produksi, ALL Reject, dan % Reject Rate.

- Total Pack by ASST: Membandingkan capaian output antar koordinator/asisten (AZ: 328.96K, KZ: 315.32K, MG: 301.48K).

- Produksi /SPV: Menampilkan kontribusi output masing-masing supervisor (SPV-01 s.d. SPV-09) yang dipecah berdasarkan jenis produk (FG-01, FG-02, FG-03).

<img width="1102" height="618" alt="image" src="https://github.com/user-attachments/assets/0111e551-8a3a-432e-9b9e-3730927cffa3" />




Halaman 2: Quality Control (Analisis Reject)

- Pareto Chart % Reject Rate: Mengidentifikasi kategori cacat paling dominan beserta persentase kontribusi kumulatifnya (Pinggir, Tengah, Lubang, Belang, Sobek, Bentuk, Jatuh, Bintik hitam/merah).

- Total Reject per Produk: Memetakan volume reject pada produk FG-01, FG-02, dan FG-03.

- Hasil Pack/Operator: Menampilkan distribusi output packing antar operator (OP-01 s.d. OP-06).

- % Reject Rate per Jenis Reject: Memvisualisasikan persentase reject rate dari masing-masing jenis cacat terhadap total produksi.

<img width="1102" height="622" alt="image" src="https://github.com/user-attachments/assets/6b5ffa66-b769-4197-8733-94b1839b0351" />


4. KEY INSIGHTS & REKOMENDASI AKSI

- Prinsip Pareto (91% Reject dari 2 Kategori): Jenis reject Pinggir (15,153.55 atau 60%) dan Tengah (7,662.10) secara kumulatif menyumbang 91% dari seluruh reject, disusul oleh Lubang (1,341.00, kumulatif 96%) dan Belang (772.30, kumulatif 99%).

- Prioritas Perbaikan Operasional: Meskipun reject Pinggir mendominasi, kategori ini merupakan constraint bawaan proses. Oleh karena itu, prioritas perbaikan QC difokuskan pada dua cacat yang paling actionable:

  1) Reject Tengah: Melakukan evaluasi dan kalibrasi kecepatan (speed) mesin slice.

  2) Reject Lubang: Melakukan pengecekan berkala pada mesin filler dan sistem vacuum.

- Fokus Produk: Produk FG-01 menyumbang volume reject paling tinggi dibandingkan FG-02 dan FG-03, sehingga pengetatan inspeksi in-process perlu diprioritaskan pada lini FG-01.

- Distribusi Output Tim: Beban kerja antar ASST relatif seimbang di rentang 301.48K - 328.96K pack, sementara di level SPV dan Operator terlihat variasi output yang dipimpin oleh SPV-04 dan OP-04.



5. TOOLS & PRIVASI DATA

- Tools: Microsoft Power BI Desktop, Power Query (data cleaning & transformasi), dan DAX (perhitungan measure % Reject Rate serta akumulasi Pareto).

- Data Anonymization: Seluruh nama produk, supervisor, asisten, dan operator telah dianonimisasi (FG-01 s.d. FG-03, SPV-01 s.d. SPV-09, OP-01 s.d. OP-06, AZ/KZ/MG) untuk menjaga kerahasiaan data internal perusahaan.
