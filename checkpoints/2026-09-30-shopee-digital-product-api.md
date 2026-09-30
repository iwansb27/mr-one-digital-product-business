# CHECKPOINT — SHOPEE DIGITAL PRODUCT / API
Tanggal: 30 September 2026

## Fokus lanjutan
Checkpoint ini menjadi titik mulai untuk obrolan berikutnya.

### 1. Shopee Digital Product Ability
Status: ⚠️ BELUM TERBUKTI

Yang masih harus diverifikasi:
- Apakah akun/toko Shopee dapat menjual produk digital sesuai aturan dan fitur Shopee saat ini.
- Jalur/fitur resmi yang tersedia untuk digital product.
- Batasan kategori, listing, delivery/fulfillment, dan persyaratan seller.
- Bukti harus berasal dari pengujian nyata atau sumber resmi; jangan menganggap tersedia hanya karena marketplace/akun lain dapat melakukannya.

### 2. Shopee Seller Management API
Status: ⚠️ BELUM TERBUKTI

Yang masih harus diverifikasi:
- Apakah akses seller-management resmi tersedia untuk kebutuhan kita.
- Endpoint yang benar-benar dapat dipakai untuk operasi toko/listing/product/order atau fungsi terkait.
- Model autentikasi/OAuth, permission/scope, approval, dan batas akses.
- Apakah akses tersebut dapat dihubungkan ke workflow bisnis digital product secara aman.

Aturan:
- Jangan menyatakan API aktif sebelum endpoint dan permission benar-benar diuji.
- Prioritaskan jalur resmi Shopee Open Platform/Partner App.
- Jangan menggunakan credential melalui tool tidak resmi.
- Free/Zero Rupiah First tetap berlaku.

### 3. Integrasi ke workflow bisnis
Status: ⚠️ BELUM TERBUKTI

Tujuan tahap berikutnya:
- Setelah kemampuan Shopee dan API terbukti, tentukan titik integrasi ke workflow bisnis digital product.
- Integrasi tidak boleh dipaksakan sebelum capability dan permission Shopee terbukti.
- Gunakan prinsip READ → VERIFY → DECIDE → ACT.

## Batasan checkpoint
Checkpoint ini **khusus untuk bisnis digital product dan jalur Shopee**.

Sistem, repository, manager, atau proyek lain tidak menjadi bagian dari checkpoint ini dan tidak perlu disebutkan di sini.

## Next Action
1. Verifikasi kemampuan Shopee untuk digital product.
2. Verifikasi akses resmi Shopee Seller Management/Open Platform API.
3. Catat hasil sebagai FACT / SIGNAL / INFERENCE / ASSUMPTION.
4. Baru tentukan bentuk integrasi ke workflow bisnis.
5. Jangan membangun automation sebelum capability dan permission terbukti.

## Prinsip
READ → VERIFY → DECIDE → ACT

Tidak ada klaim "sudah terintegrasi" sebelum benar-benar diuji.
