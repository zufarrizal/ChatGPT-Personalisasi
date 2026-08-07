# ChatGPT Personalisasi

Kumpulan instruksi berbahasa Indonesia untuk mengarahkan ChatGPT atau AI coding assistant agar bekerja seperti **Senior Full-Stack Developer** yang sistematis, aman, efisien, dan transparan.

Instruksi di repository ini menekankan implementasi yang utuh, scope MVP yang jelas, kode reusable, validasi dan pengujian nyata, dokumentasi yang selalu sinkron, serta penggunaan Git dan GitHub secara aman.

> [!NOTE]
> Repository ini berisi dokumen instruksi, bukan aplikasi atau package. Tidak ada dependency, proses instalasi, database, maupun build yang perlu dijalankan.

## Isi Repository

| File | Keterangan |
| --- | --- |
| [`Personalisasi Final.md`](./Personalisasi%20Final.md) | Versi utama dan paling lengkap. Direkomendasikan untuk penggunaan baru. |
| [`Personalisasi.md`](./Personalisasi.md) | Versi ringkas dengan aturan inti dan format laporan yang lebih sederhana. |
| [`LICENSE`](./LICENSE) | Lisensi MIT untuk penggunaan, perubahan, dan distribusi. |

## Cakupan Instruksi

Versi final mengatur cara AI menangani pekerjaan pengembangan dari awal sampai pelaporan, meliputi:

- Analisis kebutuhan dan akar masalah sebelum mengubah kode.
- Implementasi langsung dan terintegrasi ketika akses proyek tersedia.
- Pemeliharaan struktur, framework, dependency, dan pola arsitektur proyek.
- Pemilihan tech stack yang efisien untuk proyek baru.
- Penggunaan komponen, utility, service, dan konfigurasi yang reusable.
- Pendekatan Minimum Viable Product (MVP) tanpa menambah scope sepihak.
- Efisiensi frontend, backend, database, dan API.
- Validasi input, pengelolaan secret, serta keamanan aplikasi dasar.
- Konsistensi UI/UX dan penggunaan komponen dialog atau notifikasi profesional.
- Lint, formatter, type checking, test, build, dan smoke test yang dilaporkan secara jujur.
- Build aplikasi desktop setelah perubahan stabil.
- Praktik Git dan GitHub yang aman tanpa force push atau rilis tanpa izin.
- Sinkronisasi dokumentasi dengan implementasi aktual.
- Delegasi multi-agent secara terukur untuk pekerjaan kompleks.
- Format laporan akhir yang mencakup hasil, pengujian, build, Git, risiko, dan pekerjaan yang belum selesai.

## Perbedaan Versi

| Aspek | `Personalisasi.md` | `Personalisasi Final.md` |
| --- | --- | --- |
| Tujuan | Instruksi inti yang ringkas | Pedoman kerja menyeluruh |
| Jumlah aturan utama | 9 | 24 |
| Arsitektur dan reusable code | Dasar | Lebih rinci |
| Database, API, dan keamanan | Umum | Bagian khusus |
| UI/UX | Fokus pada modal | Konsistensi, state, dan interaksi penting |
| Testing dan build | Ringkas | Checklist validasi dan batas klaim yang jelas |
| Git dan GitHub | Aturan dasar | Workflow aman dan persetujuan rilis |
| Dokumentasi | Pembaruan umum | Sinkronisasi dokumentasi secara menyeluruh |
| Multi-agent | Tidak dibahas | Strategi peran dan orkestrasi |
| Laporan akhir | 7 bagian | 12 bagian |

Gunakan **versi final** jika platform mendukung instruksi panjang. Gunakan **versi ringkas** jika tersedia batas karakter yang lebih kecil atau jika hanya diperlukan aturan inti.

## Cara Menggunakan

### Sebagai instruksi personalisasi AI

1. Buka file [`Personalisasi Final.md`](./Personalisasi%20Final.md).
2. Salin seluruh isinya.
3. Tempelkan ke bagian instruksi khusus atau personalisasi pada platform AI yang digunakan.
4. Simpan perubahan, lalu mulai percakapan baru agar instruksi diterapkan sejak awal.
5. Berikan konteks proyek, tujuan, batas scope, dan kriteria selesai pada setiap tugas.

Nama menu dan kapasitas instruksi dapat berbeda antarplatform. Jika dokumen lengkap melebihi batas yang tersedia, gunakan [`Personalisasi.md`](./Personalisasi.md) atau pilih bagian yang paling relevan dengan workflow Anda.

### Sebagai instruksi repository

Jika coding assistant yang digunakan mendukung file instruksi tingkat repository seperti `AGENTS.md`, salin versi yang dipilih ke root proyek:

```powershell
Copy-Item -LiteralPath "Personalisasi Final.md" -Destination "AGENTS.md"
```

Sesuaikan instruksi umum dengan kebutuhan proyek, misalnya:

- Command lint, test, dan build yang benar.
- Struktur folder dan pola arsitektur yang digunakan.
- Aturan penamaan dan formatting.
- Batas file atau module yang boleh diubah.
- Workflow branch, commit, dan deployment.

Instruksi khusus proyek sebaiknya dibuat lebih spesifik dan tidak bertentangan dengan aturan tim yang sudah berlaku.

## Contoh Permintaan

Setelah personalisasi diterapkan, berikan permintaan yang konkret:

```text
Periksa repository ini, temukan akar penyebab form pembayaran terkirim dua kali,
implementasikan perbaikannya tanpa mengganti framework, tambahkan test yang relevan,
perbarui dokumentasi yang terdampak, lalu laporkan hasil aktualnya.
```

Untuk hasil yang lebih terarah, sertakan:

- Tujuan utama.
- Perilaku saat ini dan perilaku yang diharapkan.
- Batas scope.
- Teknologi atau folder yang terkait.
- Kriteria selesai.
- Izin atau larangan untuk commit, push, deployment, dan release.

## Batasan

- Instruksi meningkatkan konsistensi cara kerja AI, tetapi tidak menjamin seluruh jawaban atau perubahan kode selalu benar.
- Hasil tetap perlu ditinjau, terutama untuk keamanan, migrasi database, transaksi, deployment, dan perubahan destruktif.
- Jangan memasukkan password, token, API key, atau data sensitif ke dalam instruksi maupun percakapan.
- Kemampuan mengedit file, menjalankan test, membuat build, commit, atau push bergantung pada akses dan tool yang tersedia di lingkungan AI.
- GitHub Release dan push tag tetap memerlukan persetujuan eksplisit sesuai dokumen versi final.

## Menyesuaikan Instruksi

Anda bebas mengubah dokumen sesuai kebutuhan. Agar tetap efektif:

1. Pertahankan aturan yang konkret dan dapat diverifikasi.
2. Hapus bagian yang tidak relevan dengan jenis proyek Anda.
3. Tambahkan command dan konvensi proyek secara eksplisit.
4. Hindari aturan yang saling bertentangan.
5. Tinjau ulang instruksi ketika workflow atau tech stack berubah.

## Lisensi

Repository ini menggunakan [MIT License](./LICENSE). Anda dapat menggunakan, menyalin, mengubah, dan mendistribusikan isinya sesuai ketentuan lisensi tersebut.
