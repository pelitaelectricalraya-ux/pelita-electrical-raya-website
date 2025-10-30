
Pelita Electrical Raya - Website package (2025)
-----------------------------------------------

Konten ini termasuk file siap pakai untuk di-upload ke GitHub Pages / Netlify.
Folder: pelitaelectricalraya_website

Files:
- index.html
- assets/css/style.css
- assets/js/script.js
- assets/images/per2025.png  (logo yang Anda berikan)

EMAILS to create (suggested, not auto-created):
- pelitaelectricalraya@gmail.com  (existing)
- support@pelitaelectricalraya.com
- maintenance@pelitaelectricalraya.com
- info@pelitaelectricalraya.com

SHORT DEPLOY GUIDE:
1. Upload folder contents to a GitHub repo and enable GitHub Pages (branch: main, folder: / (root)).
2. Or sign up at Netlify and drag-drop the folder to publish instantly.
3. For custom domain (free): register a Freenom domain (example: pelitaelectricalraya.tk) and point it to Netlify/GitHub Pages via DNS.
4. Use Cloudflare to proxy traffic (enable SSL) and manage DNS records.
5. Use Zoho Mail (free tier) to host your custom domain email. Follow Zoho's settings to add MX and TXT records via Cloudflare.

HOW TO SEND THIS ZIP FILE TO pelitaelectricalraya@gmail.com
- I cannot send emails on your behalf. To email the file:
  1. Download the zip from the link provided in this message.
  2. Compose a new Gmail message to pelitaelectricalraya@gmail.com and attach the zip.
  3. Or use command-line: 
     - Linux/Mac:  `echo "See attachment" | mutt -s "Website files" -a pelitaelectricalraya_website.zip -- pelitaelectricalraya@gmail.com`
     - Windows: attach in Outlook or webmail client.

If you want, I can also provide:
- A step-by-step script of exact DNS records and verification steps for Zoho Mail + Cloudflare.
- A ready Git repo structure (I already made the folder).

Thank you!


# Panduan Publikasi Website Pelita Electrical Raya

Selamat! Anda memiliki website yang siap digunakan. Panduan ini akan memandu Anda langkah demi langkah untuk mempublikasikannya secara **GRATIS** selamanya tanpa harus sewa hosting atau beli domain.

Kami akan menggunakan layanan berikut:
1.  **Domain Gratis:** Freenom (untuk domain `.tk`, `.ml`, `.ga`, dll.)
2.  **Hosting Gratis:** GitHub Pages (untuk menyimpan file website Anda)
3.  **Email Kustom:** Forwarding email dari domain Anda ke Gmail Anda.

---

### Langkah 1: Siapkan Aset Website

Sebelum mulai, pastikan Anda memiliki semua file website:
1.  **Logo:** Unduh logo `per2025.png` dan simpan di folder `images/` dengan nama `logo.png`.
2.  **Gambar Hero:** Cari gambar berkualitas tinggi tentang listrik/industri di [Unsplash](https://unsplash.com) (gratis). Simpan di folder `images/` dengan nama `hero-bg.jpg`.
3.  **Ikon Kontak:** Unduh ikon untuk Telepon, WhatsApp, SMS, Email, dll. dari [Flaticon](https://www.flaticon.com) (gratis dengan atribusi). Simpan di folder `images/` dengan nama yang sesuai (`icon-phone.png`, `icon-whatsapp.png`, dll.).

Pastikan semua file ini ada di dalam folder `pelita-electrical-raya-website/`.

---

### Langkah 2: Dapatkan Hosting Gratis dengan GitHub Pages

GitHub Pages adalah layanan dari GitHub untuk meng-hosting website statis secara gratis.

1.  **Buat Akun GitHub:** Jika belum punya, daftar di [github.com](https://github.com).
2.  **Buat Repository Baru:**
    *   Klik tombol `+` di kanan atas dan pilih "New repository".
    *   Beri nama repository: `pelitaelectricalraya.github.io` (ini adalah format penamaan khusus agar langsung aktif).
    *   Pilih "Public".
    *   Klik "Create repository".
3.  **Upload File Website:**
    *   Di halaman repository baru, klik "uploading an existing file".
    *   Drag dan drop seluruh folder `pelita-electrical-raya-website` Anda ke area upload.
    *   Pastikan Anda mengupload folder beserta isinya (folder `css`, `js`, `images`, dan file `index.html`, `README.md`).
    *   Scroll ke bawah dan klik "Commit changes".

Website Anda sekarang sudah online! Anda bisa mengaksesnya sementara di `https://pelitaelectricalraya.github.io`.

---

### Langkah 3: Dapatkan Domain Gratis dari Freenom

1.  **Kunjungi Freenom:** Buka [www.freenom.com](https://www.freenom.com).
2.  **Cari Domain:** Di kotak pencarian, ketik `pelitaelectricalraya` dan pilih ekstensi `.tk` (atau yang lain jika tersedia).
3.  **Checkout:** Klik "Checkout". Pilih durasi 12 bulan (gratis).
4.  **Isi Data:** Isi formulir dengan data Anda yang valid (nama, email, alamat). Gunakan email yang aktif karena akan digunakan untuk verifikasi.
5.  **Verifikasi:** Cek email Anda dari Freenom dan klik link verifikasi untuk mengaktifkan domain.

Sekarang Anda memiliki domain `pelitaelectricalraya.tk`.

---

### Langkah 4: Hubungkan Domain Freenom ke GitHub Pages (DNS)

Ini adalah langkah "mengatur DNS server sendiri" yang Anda minta.

1.  **Buka Dashboard Freenom:** Login ke akun Freenom Anda.
2.  **Pilih Domain:** Klik "Services" -> "My Domains". Klik pada domain `pelitaelectricalraya.tk` Anda.
3.  **Kelola DNS:** Klik tombol "Manage Domain". Pilih tab "Management Tools" dan kemudian "Nameservers".
4.  **Gunakan Custom Nameserver:** Pilih "Use custom nameservers" dan masukkan nameserver milik GitHub:
    *   Nameserver 1: `ns1.github.io`
    *   Nameserver 2: `ns2.github.io`
    *   Klik "Change Nameservers".
5.  **Tunggu Propagasi:** Perubahan DNS butuh waktu (beberapa menit hingga 48 jam). Biasanya cukup cepat.

---

### Langkah 5: Konfigurasi DNS di GitHub

Agar GitHub tahu bahwa domain `pelitaelectricalraya.tk` milik Anda:

1.  **Buka Repository GitHub:** Kembali ke repository `pelitaelectricalraya.github.io` Anda.
2.  **Buka Settings:** Klik tab "Settings".
3.  **GitHub Pages:** Di menu sebelah kiri, scroll ke bawah dan klik "Pages".
4.  **Tambahkan Custom Domain:**
    *   Di bagian "Custom domain", ketik `pelitaelectricalraya.tk`.
    *   Centang kotak "Enforce HTTPS".
    *   GitHub akan secara otomatis membuat file `CNAME` di repository Anda yang berisi nama domain Anda.

**Selesai!** Setelah propagasi DNS selesai, website Anda akan dapat diakses di **`https://pelitaelectricalraya.tk`**.

---

### Langkah 6: (Opsional) Setup Email Forwarding

Anda tidak bisa membuat email inbox `info@pelitaelectricalraya.tk` gratis, tapi Anda bisa membuat **forwarding**. Artinya, email yang dikirim ke `info@pelitaelectricalraya.tk` akan otomatis diteruskan ke `pelitaelectricalraya@gmail.com`.

1.  **Buka Dashboard Freenom:** Kembali ke "My Domains" di Freenom.
2.  **Kelola Domain:** Klik "Manage Domain" pada `pelitaelectricalraya.tk`.
3.  **Forwarding:** Pilih tab "Management Tools" dan kemudian "URL Forwarding".
4.  **Atur Forwarding:**
    *   **Forwarding Type:** Pilih "URL Forwarding".
    *   **Host/Domain:** Kosongkan (atau isi dengan `@`).
    *   **Redirect To:** Isi dengan alamat email Gmail Anda: `pelitaelectricalraya@gmail.com`.
    *   **Type:** Pilih "Permanent (301)".
    *   Klik "Save Changes".

Ulangi langkah ini untuk setiap alamat email yang Anda inginkan (`support@`, `maintenance@`, `layanan@`), dan arahkan semuanya ke `pelitaelectricalraya@gmail.com`.

---

### **Kesimpulan**

Website Anda sekarang:
*   **Elegan dan Profesional:** Desain modern dan user-friendly.
*   **Online 24/7:** Hosting gratis di GitHub.
*   **Domain Kustom:** `pelitaelectricalraya.tk` gratis dari Freenom.
*   **Siap Publikasi:** Semua informasi kontak, peta, dan layanan sudah terpasang dengan benar.

Selamat, website Pelita Electrical Raya Anda sudah siap diluncurkan!