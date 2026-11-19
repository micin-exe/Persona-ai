PERSONA AI COMMUNITY — PAKET AWAL v1

Isi paket:
- index.html       tampilan chatroom dan koneksi Firebase (opsional)
- manifest.json    identitas PWA
- sw.js            service worker dasar
- icon.svg         ikon aplikasi
- firestore.rules  aturan keamanan awal Firestore
- README-ID.txt    panduan

PENTING:
1. Saat pertama dibuka, website berada dalam MODE DEMO LOKAL. Pesan hanya tersimpan di browser/perangkat yang sama.
2. Agar pesan benar-benar dibagikan antarperangkat, Aika perlu membuat project Firebase, mengaktifkan Authentication > Anonymous, membuat Firestore Database, memasukkan konfigurasi web Firebase ke index.html, dan menerapkan firestore.rules.
3. Jangan pernah menaruh private key, service account, atau kunci rahasia AI di file website/GitHub Pages.
4. Paket ini belum membuat Aita dan Eta membalas otomatis. Itu tahap berikutnya dan membutuhkan backend serta layanan AI yang dipilih dengan persetujuan Aika.
5. Target paket ini tidak memerlukan aktivasi paket berbayar. Jangan masukkan kartu pembayaran atau upgrade plan untuk mengikuti panduan.

CARA PUBLIKASI VIA GITHUB PAGES (setelah file diekstrak):
1. Buat repository GitHub baru, misalnya persona-ai-community.
2. Unggah semua file dari paket ini ke root repository (bukan folder zip).
3. Buka Settings > Pages.
4. Pada Build and deployment, pilih Deploy from a branch.
5. Pilih branch main dan folder /(root), lalu Save.
6. Tunggu URL Pages muncul. Buka URL itu melalui Chrome Android.
7. Untuk memasang: menu Chrome ⋮ > Add to Home screen / Install app (nama menu bisa berbeda).

CATATAN FIREBASE:
- Untuk percobaan lintas perangkat, buat project Firebase pada Spark plan.
- Tambahkan Web App dan salin firebaseConfig ke bagian const firebaseConfig di index.html.
- Authentication > Sign-in method > Anonymous: Enable.
- Firestore Database: buat database, lalu terapkan isi firestore.rules melalui tab Rules.
- Jika Firebase belum disiapkan, biarkan konfigurasi ISI_... apa adanya agar demo lokal tetap berjalan.

BATASAN:
Ini starter prototype, bukan layanan produksi. Aturan akses saat ini mengizinkan semua pengguna anonim yang berhasil masuk untuk membaca dan mengirim pesan. Jangan gunakan untuk data pribadi/sensitif. Batasi akses sebelum dipakai publik.
