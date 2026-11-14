# Rangkuman Konseling

Aplikasi web satu halaman untuk merekam sesi konseling, membuat transkrip dengan pemisahan suara Psikolog/Klien, lalu menyusun rangkuman DAP/SOAP memakai Gemini API. Hasil dapat diedit dan diekspor ke Word, PDF, atau WhatsApp.

## Cara kerja dan privasi
- Seluruh aplikasi berjalan di browser. Tidak ada server milik pengembang.
- Audio dan teks dikirim langsung dari browser ke Google (Gemini API) memakai API key pengguna sendiri.
- API key hanya disimpan di browser perangkat pengguna (jika opsi "Ingat key" dicentang), tidak ada di repo ini.
- Tidak ada data klien yang disimpan di repo atau server. **Jangan pernah mengunggah rekaman, transkrip, atau rangkuman ke repo ini.**
- Gunakan API key dari proyek Google dengan billing aktif dan rekam hanya dengan persetujuan klien (untuk siswa di bawah umur, persetujuan orang tua/wali).

## Menjalankan di GitHub Pages
1. Buat repository baru di GitHub (mis. `rangkuman-konseling`).
2. Unggah `index.html` dan `README.md` ke cabang `main` (Add file → Upload files → Commit).
3. Buka **Settings → Pages**. Pada *Build and deployment*, pilih **Deploy from a branch**, cabang **main**, folder **/(root)**, lalu **Save**.
4. Tunggu 1 sampai 2 menit. Alamatnya: `https://NAMA-AKUN.github.io/NAMA-REPO/`.
5. Buka alamat itu di Chrome, buka **Pengaturan API**, isi API key, lalu tekan **Tes koneksi**.

## Catatan keamanan
- Situs GitHub Pages **bisa dibuka siapa saja** yang tahu alamatnya (kecuali memakai GitHub Enterprise). Kodenya tidak berisi rahasia, tetapi jangan membagikan alamatnya sembarangan.
- Di Google Cloud Console, API key dapat dibatasi hanya untuk alamat situs ini (HTTP referrer), sehingga key tidak berguna jika bocor di tempat lain.
- Jangan commit API key ke repo.
