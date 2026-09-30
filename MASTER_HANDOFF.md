# MASTER HANDOFF — MR.ONE DIGITAL PRODUCT BUSINESS & MARKETPLACE

MASTER WORKING CONTEXT — CHECKPOINT 30 SEPTEMBER 2026

## 0. STATUS HANDOFF
- Nama sistem/proyek: MR.ONE Digital Product Business & Marketplace
- Tujuan: membangun mesin bisnis produk digital yang dimulai Rp0/modal seminimal mungkin, berdasarkan kebutuhan pasar nyata, lalu diproduksi, dijual, diukur, dan bertahap diotomatisasi oleh MR.ONE.
- Status: MASTER HANDOFF
- Prinsip: ACTION FIRST — FREE FIRST — MARKET BEFORE PRODUCTION — PROOF BEFORE BUILD

## 1. TUJUAN UTAMA
Urutan: Cari kebutuhan pasar → validasi → pilih beberapa produk → cari produksi gratis → produksi → buka/lengkapi toko → listing → jual → ukur → revisi → scale → otomasi.
Target akhir adalah mesin bisnis yang benar-benar menghasilkan transaksi. Aplikasi, AI, repository, connector, automation, dan marketplace hanyalah alat.

## 2. PRINSIP KERJA
### 2.1 FREE / ZERO RUPIAH FIRST
Prioritaskan tool gratis, free tier, open-source bila relevan, trial tanpa pembayaran, dan infrastruktur yang sudah dimiliki. Biaya baru dipertimbangkan setelah ada bukti pendapatan.

### 2.2 MARKET BEFORE PRODUCTION
Periksa demand, produk yang benar-benar dijual, buyer signal, harga, sales bila tersedia, persaingan, keluhan/kebutuhan, dan gap. Setelah minimum evidence tersedia: STOP RESEARCH → START BUILD.

### 2.3 BUKAN SATU PRODUK
Target: banyak kandidat → validasi → pilih beberapa → produksi beberapa → listing → ukur. Kandidat yang pernah muncul: budget planner, financial planner/tracker, spreadsheet keuangan, pembukuan UMKM, inventory tracker, life planner, social media content planner, Canva template, digital calendar, worksheet, educational material, tutorial, template administrasi/bisnis, template rumah/desain, wedding planner, baby journal, ebook/tutorial praktis. Ini kandidat, bukan keputusan final.

## 3. WORKFLOW UTAMA
1. AKUN SELLER — verifikasi Seller Centre, status seller, identitas, kontak, rekening/pencairan, dan kemampuan mengelola toko.
2. JALUR PRODUK DIGITAL — verifikasi langsung apakah akun dapat menjual produk digital; kategori, PDF, template, XLSX/spreadsheet, Canva template, program khusus, virtual/digital goods, dan delivery mechanism.
3. CARI PRODUK — setelah channel terbukti, riset banyak produk dan catat Product, Seller, Price, Sales, Rating, Review, Format, Category, Problem, Competition, Gap, Source, Status.
4. PILIH BEBERAPA PRODUK — gunakan demand, competition, production difficulty, cost, problem value, differentiation, marketplace eligibility.
5. CARI TEMPAT MEMBUAT — Canva, spreadsheet, AI, dan tool gratis lain sesuai kebutuhan; periksa lisensi.
6. PRODUKSI — produk utama, preview, informasi listing, dan quality control.
7. BUKA/LENGKAPI TOKO — profil, seller settings, rekening, kategori, dan delivery mechanism yang benar-benar tersedia.
8. LISTING — judul, thumbnail, preview, deskripsi, harga, kategori, format, isi paket, penggunaan, ketentuan, delivery, publish.
9. JUAL & UKUR — impression, view, click, add to cart bila tersedia, order, conversion, revenue, refund/complaint, review, pertanyaan pembeli.

## 4. MARKET RESEARCH RULES
Bedakan FAKTA, SIGNAL, INFERENCE, dan ASSUMPTION. Listing seller lain adalah market signal, bukan bukti bahwa akun user mendapat izin yang sama dan bukan jaminan produk laku.

## 5. MARKET SIGNAL SEBELUMNYA
Riset sebelumnya pernah menunjukkan antara lain: Budget Planner 3RB+; Template Keuangan UMKM sekitar 593–605; Pembukuan Spreadsheet sekitar 212–221; Life Planner 10-in-1 sekitar 574–583; Financial Tracker Spreadsheet sekitar 432; Template Canva 3RB+; Planner 2026–2027 2RB+; Financial Planner 3RB+; Baby Journal 1RB+; Wedding Planner 1RB+; Tutorial BIM/Revit sekitar 254; ebook membuat/menjual ebook sekitar 249; template desain rumah sekitar 148; digital calendar sticker sekitar 151.
PENTING: angka tersebut adalah market signals dari riset sebelumnya, bukan kondisi terkini yang terverifikasi dan bukan jaminan penjualan. Verifikasi ulang sebelum keputusan produksi.

## 6. SHOPEE — STATUS
Shopee adalah salah satu channel utama yang sedang dieksplorasi. Bedakan marketplace, Seller Centre, Official Open Platform/Partner App, dan connector ChatGPT.
Connector Shopee yang telah diperiksa terutama menyediakan search/browse item dan tracking tertentu. Belum terbukti sebagai Seller Management API penuh.
Jangan menyatakan MR.ONE dapat membuat/edit/delete listing, mengelola order/toko/inventory, kecuali endpoint dan authorization tersedia serta berhasil diuji.

## 7. SHOPEE API / AUTOMATION
Jalur prioritas: MR.ONE → Official Shopee API → Shopee Authorization → Seller Store.
Bukan MR.ONE → tool tidak dikenal → login/password Shopee.
Jangan memberikan credential toko kepada tool yang tidak jelas.

## 8. SECURITY
Gunakan OAuth bila tersedia dan least privilege. Secret/API key tidak masuk source code. Jangan mengirim credential melalui chat bila tidak diperlukan. Jangan memakai automation tidak resmi untuk melewati batasan platform. Semua koneksi harus dapat diaudit.

## 9. MR.ONE SHOP MANAGER
Nama komponen yang dikunci: MR.ONE Shop Manager.
Konsep utama: Arsitektur Dua Jalur. Store/channel dapat berbeda; jangan menganggap semua toko otomatis satu repository/pipeline.

## 10. REPOSITORY YANG SUDAH ADA
Repository: iwansb27/mr-one-shop-manager
Environment yang disebut user: Poe.new.
Repository ini HARUS dibaca sebelum menentukan apakah Shopee reuse repository, module baru, branch, atau repository terpisah. Jangan mengklaim telah membaca source code tanpa akses repository aktual.

## 11. MASTER REPOSITORY BARU
Repository: iwansb27/mr-one-digital-product-business
Fungsi: master repository bisnis produk digital, terpisah dari MR.ONE Shop Manager, Home MR.ONE, dan repo/channel implementasi spesifik.
Struktur awal:
mr-one-digital-product-business/
├── MASTER_HANDOFF.md
├── README.md
├── market-research/
├── product-ideas/
├── products/
├── production/
├── marketplace/
├── listings/
├── sales-data/
├── automation/
└── checkpoints/

## 12. ATURAN REPOSITORY
Sebelum membuat repo/module baru, periksa struktur, fungsi, store/channel, posting manager, backend, API, authentication, database/storage, deployment, workflow, multi-store architecture, dan apakah Shopee hanya channel baru.
Opsi A — Reuse repository jika architecture multi-store. Opsi B — Module/channel baru jika core manager sama. Opsi C — Repository baru jika lifecycle/architecture benar-benar berbeda. Tidak boleh menentukan A/B/C sebelum membaca repository aktual.

## 13. HUBUNGAN DENGAN MR.ONE HOME
Home MR.ONE adalah pusat orkestrasi. Fondasi yang dikunci: Workspace Agent, Lead Work Orchestrator, Task State, Approval Gateway, Registry, Audit/History.
Architecture final mengikuti repository dan tool yang benar-benar tersedia.

## 14. MR.ONE DIGITAL PRODUCT FACTORY
Pipeline: IDE → RISET KEBUTUHAN → CONTENT MASTER → STRUCTURE → FLOW / DIAGRAM → VISUAL → TEMPLATE / CHECKLIST → DESIGN → FINAL FILE → PRODUCT LIBRARY → READY FOR SALE → PUBLISH / SELL → MEASURE → ITERATE.

## 15. TOOL PRINCIPLE
Tools bukan tujuan. ChatGPT = reasoning/content/orchestration; Canva = design; Spreadsheet = business tools; Cloudinary = storage bila diperlukan; GitHub = source/version control; AppDeploy = application/workspace; Poe.new = environment yang sebelumnya digunakan; Shopee = marketplace; Official Shopee API = automation jika benar-benar tersedia.
Audit tool dengan: AVAILABLE → CONNECTED → READ → WRITE → VERIFIED.

## 16. CONNECTOR STATUS RULE
CONNECTED + READ = bisa membaca. CONNECTED + READ-WRITE = bisa membaca dan mengubah. AVAILABLE NOT CONNECTED = tersedia tetapi belum tersambung. NOT AVAILABLE = tidak tersedia. UNVERIFIED = secara teori mungkin tetapi belum diuji.

## 17. KERJA, BUKAN OMONG
Setiap fase harus menghasilkan output nyata: riset → tabel kandidat; validasi → daftar lolos/tidak; produksi → file nyata; listing → data siap publish; automation → koneksi/API/workflow yang benar-benar diuji.
Jangan mengganti pekerjaan bisnis dengan pembangunan architecture.

## 18. ANTI-RISET TANPA AKHIR
Gunakan Minimum Viable Evidence. Setelah bukti minimum: STOP RESEARCH → START BUILD.
Bukti minimum: ada kebutuhan, ada channel, produk dapat dibuat, dan produk allowed/legal pada channel tersebut.

## 19. ATURAN PRODUKSI
Jangan membuat produk hanya karena AI bisa membuatnya. Buat karena ada masalah nyata + channel + buyer signal + dapat dibuat secara ekonomis.

## 20. STRATEGI PORTFOLIO
20 kandidat → 5–10 divalidasi → 3–5 diproduksi → listing → ukur → produk yang menunjukkan bukti pasar dikembangkan. Jumlah final menyesuaikan kemampuan dan bukti.

## 21. KATEGORI PRIORITAS RISET
Keuangan pribadi; UMKM; productivity; content creator; education; business; niche-specific. Contoh niche: UMKM makanan, reseller, affiliate, freelancer, guru, mahasiswa, pemilik toko, content creator, wedding organizer, small business.

## 22. DIFFERENTIATION
Jika pasar ramai, cari narrower niche. Contoh Financial Planner → Financial Planner untuk UMKM makanan rumahan; Inventory spreadsheet → Inventory spreadsheet untuk reseller Shopee.
Nilai dapat berasal dari spesifik, mudah digunakan, bahasa Indonesia, instruksi, formula otomatis, bundle, contoh data, dashboard, checklist, tutorial.

## 23. KUALITAS MINIMUM PRODUK DIGITAL
Mudah digunakan, tidak membingungkan, bahasa jelas, minim typo, visual cukup profesional, asset berlisensi digunakan sesuai aturan, ada instruksi, preview, dan value jelas.

## 24. HARGA
Pertimbangkan harga kompetitor, kompleksitas, value, jumlah template, fitur, bundle, target buyer, dan bukti demand. Harga final diuji melalui pasar.

## 25. DEFINISI PRODUK JADI
File final tersedia; sudah diperiksa; preview tersedia; nama dan deskripsi tersedia; harga ditentukan; kategori diketahui; delivery mechanism diketahui; listing siap; channel memperbolehkan produk.

## 26. DEFINISI TOKO SIAP
Seller account aktif; verifikasi selesai; rekening tersedia; store profile tersedia; kategori tersedia; digital product route terbukti; delivery mechanism terbukti; listing dapat dibuat; produk siap publish.

## 27. DEFINISI AUTOMATION SIAP
API tersedia; authentication dan scope tersedia; credential aman; endpoint diketahui; request/response berhasil; error handling tersedia; rate limit dipahami; test berhasil; tidak melanggar kebijakan platform.

## 28. CHECKPOINT 30 SEPTEMBER 2026
MR.ONE membangun bisnis produk digital dengan Free/Zero Rupiah First, multi-product, market validation wajib, production setelah channel terbukti. Shopee sedang dieksplorasi. Seller account dan digital-product eligibility harus diverifikasi. Official Shopee Open Platform/Partner App adalah jalur yang perlu diperiksa untuk automation. Connector Shopee saat ini bukan bukti seller management API. mr-one-shop-manager harus dibaca sebelum keputusan arsitektur Shopee. MR.ONE Shop Manager menggunakan Arsitektur Dua Jalur. Home MR.ONE tetap pusat orkestrasi.

## 29. BELUM TERBUKTI
Belum boleh dianggap selesai: akun dapat menjual semua digital products; PDF/Canva/XLSX tertentu allowed; delivery otomatis semua digital goods; Seller API tersedia di connector; MR.ONE dapat create/edit/delete listing; automation penuh toko aktif; mr-one-shop-manager cocok langsung; produk tertentu pasti laku atau menghasilkan pendapatan.

## 30. NEXT ACTION — URUTAN WAJIB
1. Verifikasi Seller Centre / akun Shopee: seller status, verification, bank, store, category, digital product route.
2. Verifikasi jalur Produk Digital melalui Seller Centre, dokumentasi Shopee resmi, dan Official Open Platform bila relevan.
3. Jika terbukti, riset banyak produk dengan tabel PRODUCT | SELLER | PRICE | SALES | FORMAT | CATEGORY | DEMAND SIGNAL | COMPETITION | GAP | SOURCE.
4. Pilih beberapa kandidat.
5. Cari tool produksi gratis.
6. Produksi produk pertama, kedua, ketiga, dan seterusnya berdasarkan validasi.
7. Siapkan toko.
8. Listing.
9. Ukur transaksi.
10. Kembangkan produk yang menunjukkan bukti pasar.

## 31. ATURAN PENTING UNTUK GPT BERIKUTNYA
Jangan mengulang teori jika checkpoint jelas; jangan mengatakan akan mengecek tanpa benar-benar mengecek; jangan klaim connector/API aktif tanpa test; jangan klaim telah membaca repository tanpa membacanya; jangan membuat repo baru tanpa memeriksa repo yang ada; jangan menganggap seller lain sebagai bukti izin akun; jangan menjanjikan produk pasti laku; jangan membangun architecture besar sebelum pekerjaan bisnis; jangan membakar free quota tanpa alasan; jangan menggunakan tool berbayar sebelum alasan bisnis kuat; jangan meminta user mengulang informasi yang sudah ada.

## 32. BACA DULU, BARU BERTINDAK
Untuk pekerjaan teknis: READ → VERIFY → DECIDE → ACT.
Bukan ASSUME → BUILD → DISCOVER PROBLEM.
Terutama untuk repository, API, connector, existing application, existing architecture, existing deployment, dan existing credentials.

## 33. STATUS LABEL WAJIB
✅ SUDAH — sudah dilakukan dan ada bukti.
🟡 BELUM — belum dilakukan.
🔵 TERBUKTI — sudah diuji dan berhasil.
⚠️ BELUM TERBUKTI — secara teori mungkin tetapi belum diuji.
❌ TIDAK TERSEDIA — tool/API/fitur memang tidak tersedia.

## 34. MASTER BUSINESS LOOP
MARKET SIGNAL → IDE → VALIDATION → PRODUCT → LISTING → TRAFFIC → ORDER → REVENUE → DATA → IMPROVEMENT → NEW PRODUCT → MORE REVENUE.
Bukan IDE → BUILD APP → BUILD APP → BUILD APP → BELUM ADA PRODUK.

## 35. FINAL OBJECTIVE
Menemukan kebutuhan pasar nyata, mengubahnya menjadi produk digital yang dapat dibuat dengan biaya sangat rendah, menjual melalui channel yang benar-benar tersedia, mengukur hasil, lalu membuat sistem semakin otomatis berdasarkan bukti transaksi.
Urutan prioritas: PASAR → PRODUK → PENJUALAN → DATA → AUTOMATION.
Bukan TOOL → APP → ARCHITECTURE → AUTOMATION → baru mencari pasar.

## 36. CURRENT MASTER CHECKPOINT
PROJECT: MR.ONE DIGITAL PRODUCT BUSINESS & MARKETPLACE
CHANNEL: SHOPEE
MODEL: DIGITAL PRODUCT
MODAL: FREE / ZERO RUPIAH FIRST
STRATEGI: MULTI-PRODUCT, BUKAN SATU PRODUK
MARKET VALIDATION: WAJIB
PRODUCTION: SETELAH CHANNEL TERBUKTI
MASTER REPOSITORY: iwansb27/mr-one-digital-product-business
REPOSITORY SHOP MANAGER: iwansb27/mr-one-shop-manager
REPOSITORY ENVIRONMENT: Poe.new
STATUS REPOSITORY SHOPEE: BELUM DIPUTUSKAN — HARUS DIBACA DAHULU
MR.ONE SHOP MANAGER: ARSITEKTUR DUA JALUR
HOME MR.ONE: CENTRAL ORCHESTRATOR
SHOPEE SELLER API: BELUM TERBUKTI TERSEDIA DI CONNECTOR SAAT INI
DIGITAL PRODUCT ELIGIBILITY: HARUS DIVERIFIKASI PADA SELLER ACCOUNT
NEXT ACTION: VERIFIKASI CHANNEL → BACA REPO → RISET PRODUK → PRODUKSI → LISTING

## 37. PERINTAH LANJUTAN
Pekerjaan tidak dimulai dari nol. Mulai dari checkpoint terakhir.
1. Verifikasi apa yang sudah terbukti.
2. Jangan mengulang yang sudah selesai.
3. Jika membutuhkan repository, baca repository aktual.
4. Jika membutuhkan API/connector, audit koneksi aktual.
5. Setelah minimum evidence tersedia, langsung bekerja.
6. Setiap pekerjaan menghasilkan output nyata.

# MASTER PRINCIPLE
JANGAN TERUS BERBICARA TENTANG MEMBANGUN BISNIS.
BANGUN BISNISNYA.

END OF MASTER HANDOFF