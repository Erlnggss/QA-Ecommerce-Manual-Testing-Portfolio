TC-LOGIN-001 — Login dengan credential valid
Field	Isi
Test Case ID	TC-LOGIN-001
Scenario ID	TS-LOGIN-001
Title	Login with valid credentials
Module	Login
Type	Positive
Priority	High
Preconditions	User berada di halaman Login
Test Data	Username: standard_user / Password: secret_sauce

Step	Test Steps	Expected Result
1	Buka SauceDemo	Halaman Login ditampilkan
2	Input username standard_user	Username terisi
3	Input password secret_sauce	Password terisi
4	Klik Login	Login berhasil
5	Verifikasi halaman Inventory	Inventory dan daftar produk ditampilkan

TC-LOGIN-002 — Login dengan password salah
Field	Isi
Test Case ID	TC-LOGIN-002
Scenario ID	TS-LOGIN-002
Title	Login with invalid password
Module	Login
Type	Negative
Priority	High
Preconditions	User berada di halaman Login
Test Data	Username: standard_user / Password: wrong_password

Step	Test Steps	Expected Result
1	Buka SauceDemo	Halaman Login ditampilkan
2	Input username valid	Username terisi
3	Input password salah	Password terisi
4	Klik Login	Login ditolak
5	Verifikasi response	Pesan error ditampilkan dan user tidak masuk Inventory

TC-LOGIN-003 — Login dengan username salah
Field	Isi
Test Case ID	TC-LOGIN-003
Scenario ID	TS-LOGIN-003
Title	Login with invalid username
Module	Login
Type	Negative
Priority	High
Preconditions	User berada di halaman Login
Test Data	Username: wrong_user / Password: secret_sauce

Step	Test Steps	Expected Result
1	Buka SauceDemo	Halaman Login ditampilkan
2	Input username wrong_user	Username terisi
3	Input password valid	Password terisi
4	Klik Login	Login ditolak
5	Verifikasi halaman	User tetap berada di Login dan error ditampilkan

TC-LOGIN-004 — Login tanpa username
Field	Isi
Test Case ID	TC-LOGIN-004
Scenario ID	TS-LOGIN-004
Title	Login without username
Module	Login
Type	Negative
Priority	High
Preconditions	User berada di halaman Login
Test Data	Username: kosong / Password: secret_sauce

Step	Test Steps	Expected Result
1	Buka SauceDemo	Halaman Login ditampilkan
2	Kosongkan username	Username tidak terisi
3	Input password valid	Password terisi
4	Klik Login	Login ditolak
5	Verifikasi error	Validasi username wajib diisi ditampilkan

TC-LOGIN-005 — Login tanpa password
Field	Isi
Test Case ID	TC-LOGIN-005
Scenario ID	TS-LOGIN-005
Title	Login without password
Module	Login
Type	Negative
Priority	High
Preconditions	User berada di halaman Login
Test Data	Username: standard_user / Password: kosong

Step	Test Steps	Expected Result
1	Buka SauceDemo	Halaman Login ditampilkan
2	Input username valid	Username terisi
3	Kosongkan password	Password tidak terisi
4	Klik Login	Login ditolak
5	Verifikasi error	Validasi password wajib diisi ditampilkan

TC-LOGIN-006 — Login menggunakan akun locked
Field	Isi
Test Case ID	TC-LOGIN-006
Scenario ID	TS-LOGIN-006
Title	Login with locked user
Module	Login
Type	Negative
Priority	High
Preconditions	User berada di halaman Login
Test Data	Username: locked_out_user / Password: secret_sauce

Step	Test Steps	Expected Result
1	Buka SauceDemo	Halaman Login ditampilkan
2	Input username locked_out_user	Username terisi
3	Input password valid	Password terisi
4	Klik Login	Login ditolak
5	Verifikasi response	Pesan akun terkunci ditampilkan dan user tidak dapat masuk


2. Inventory Test Cases — 5 Test Cases
Requirement: RQ-002 · Scenario: TS-INV-001 sampai TS-INV-005
TC-INV-001 — Inventory ditampilkan setelah login
Field	Isi
Test Case ID	TC-INV-001
Scenario ID	TS-INV-001
Title	Inventory page displayed after login
Module	Inventory
Type	Positive
Priority	High
Preconditions	User belum login
Test Data	standard_user / secret_sauce

Step	Test Steps	Expected Result
1	Login menggunakan credential valid	Login berhasil
2	Verifikasi halaman tujuan	User diarahkan ke halaman Inventory
3	Verifikasi judul halaman	Product / Inventory page ditampilkan
4	Verifikasi daftar produk	Produk ditampilkan tanpa error

TC-INV-002 — Seluruh produk ditampilkan
Field	Isi
Test Case ID	TC-INV-002
Scenario ID	TS-INV-002
Title	Verify all products displayed
Module	Inventory
Type	Positive
Priority	High
Preconditions	User berhasil login dan berada di Inventory
Test Data	Daftar produk SauceDemo

Step	Test Steps	Expected Result
1	Buka halaman Inventory	Inventory ditampilkan
2	Periksa seluruh item produk	Seluruh produk yang tersedia ditampilkan
3	Hitung jumlah produk	Jumlah sesuai katalog aplikasi
4	Periksa tampilan daftar	Tidak ada item hilang atau duplikat yang tidak semestinya

TC-INV-003 — Nama dan harga produk
Field	Isi
Test Case ID	TC-INV-003
Scenario ID	TS-INV-003
Title	Verify product name and price
Module	Inventory
Type	Positive
Priority	High
Preconditions	User berada di halaman Inventory
Test Data	Semua produk yang ditampilkan

Step	Test Steps	Expected Result
1	Buka Inventory	Daftar produk ditampilkan
2	Periksa nama setiap produk	Nama produk ditampilkan dengan benar
3	Periksa harga setiap produk	Harga ditampilkan
4	Bandingkan nama dan harga	Informasi sesuai dengan produk yang ditampilkan

TC-INV-004 — Gambar produk
Field	Isi
Test Case ID	TC-INV-004
Scenario ID	TS-INV-004
Title	Verify product images
Module	Inventory
Type	Positive
Priority	Medium
Preconditions	User berada di halaman Inventory
Test Data	Seluruh gambar produk

Step	Test Steps	Expected Result
1	Buka Inventory	Daftar produk ditampilkan
2	Periksa gambar setiap produk	Gambar muncul
3	Bandingkan gambar dengan nama produk	Gambar sesuai produk
4	Periksa gambar rusak / kosong	Tidak terdapat gambar yang gagal dimuat

TC-INV-005 — Product detail
Field	Isi
Test Case ID	TC-INV-005
Scenario ID	TS-INV-005
Title	Verify product detail
Module	Inventory
Type	Positive
Priority	Medium
Preconditions	User berada di halaman Inventory
Test Data	Sauce Labs Backpack

Step	Test Steps	Expected Result
1	Pilih Sauce Labs Backpack	Produk dapat dipilih
2	Klik nama atau gambar produk	Halaman detail dibuka
3	Periksa nama produk	Nama sesuai produk yang dipilih
4	Periksa harga dan deskripsi	Data sesuai produk
5	Periksa gambar	Gambar produk sesuai


3. Sorting Test Cases — 4 Test Cases
Requirement: RQ-003 · Scenario: TS-SORT-001 sampai TS-SORT-004
TC-SORT-001 — Sorting Name A to Z
Field	Isi
Test Case ID	TC-SORT-001
Scenario ID	TS-SORT-001
Title	Sort product name ascending
Module	Sorting
Type	Positive
Priority	Medium
Preconditions	User sudah login dan berada di Inventory
Test Data	Sort option: Name (A to Z)

Step	Test Steps	Expected Result
1	Buka Inventory	Produk ditampilkan
2	Klik dropdown sorting	Sorting option ditampilkan
3	Pilih Name (A to Z)	Sorting diterapkan
4	Periksa urutan nama produk	Nama produk urut alfabetis dari A ke Z

TC-SORT-002 — Sorting Name Z to A
Field	Isi
Test Case ID	TC-SORT-002
Scenario ID	TS-SORT-002
Title	Sort product name descending
Module	Sorting
Type	Positive
Priority	Medium
Preconditions	User berada di Inventory
Test Data	Sort option: Name (Z to A)

Step	Test Steps	Expected Result
1	Buka Inventory	Produk ditampilkan
2	Klik dropdown sorting	Sorting option ditampilkan
3	Pilih Name (Z to A)	Sorting diterapkan
4	Periksa urutan nama produk	Nama produk urut alfabetis terbalik Z ke A

TC-SORT-003 — Sorting Price Low to High
Field	Isi
Test Case ID	TC-SORT-003
Scenario ID	TS-SORT-003
Title	Sort price low to high
Module	Sorting
Type	Positive
Priority	High
Preconditions	User berada di Inventory
Test Data	Sort option: Price (low to high)

Step	Test Steps	Expected Result
1	Buka Inventory	Produk ditampilkan
2	Klik dropdown sorting	Sorting option ditampilkan
3	Pilih Price (low to high)	Sorting diterapkan
4	Periksa harga produk	Harga terurut dari terendah ke tertinggi

TC-SORT-004 — Sorting Price High to Low
Field	Isi
Test Case ID	TC-SORT-004
Scenario ID	TS-SORT-004
Title	Sort price high to low
Module	Sorting
Type	Positive
Priority	High
Preconditions	User berada di Inventory
Test Data	Sort option: Price (high to low)

Step	Test Steps	Expected Result
1	Buka Inventory	Produk ditampilkan
2	Klik dropdown sorting	Sorting option ditampilkan
3	Pilih Price (high to low)	Sorting diterapkan
4	Periksa harga produk	Harga terurut dari tertinggi ke terendah


4. Shopping Cart Test Cases — 6 Test Cases
Requirement: RQ-004 · Scenario: TS-CART-001 sampai TS-CART-006
TC-CART-001 — Add Single Product
Field	Isi
Test Case ID	TC-CART-001
Scenario ID	TS-CART-001
Title	Add single product to cart
Module	Cart
Type	Positive
Priority	High
Preconditions	User login dan berada di Inventory
Test Data	Sauce Labs Backpack

Step	Test Steps	Expected Result
1	Buka Inventory	Produk ditampilkan
2	Klik Add to Cart pada Backpack	Produk ditambahkan
3	Periksa cart badge	Badge menunjukkan angka 1
4	Buka Cart	Backpack muncul di Cart
5	Periksa nama dan harga	Data sesuai produk

TC-CART-002 — Add Multiple Products
Field	Isi
Test Case ID	TC-CART-002
Scenario ID	TS-CART-002
Title	Add multiple products to cart
Module	Cart
Type	Positive
Priority	High
Preconditions	User login dan berada di Inventory
Test Data	Sauce Labs Backpack, Sauce Labs Bike Light

Step	Test Steps	Expected Result
1	Klik Add to Cart pada Backpack	Backpack berhasil ditambahkan
2	Klik Add to Cart pada Bike Light	Bike Light berhasil ditambahkan
3	Periksa cart badge	Badge menunjukkan 2
4	Buka Cart	Kedua produk muncul
5	Verifikasi produk	Nama dan harga kedua produk sesuai

TC-CART-003 — Remove Selected Product
Field	Isi
Test Case ID	TC-CART-003
Scenario ID	TS-CART-003
Title	Remove selected product from cart
Module	Cart
Type	Positive
Priority	High
Preconditions	User login dan 2 produk sudah ditambahkan ke Cart
Test Data	Backpack dan Bike Light

Step	Test Steps	Expected Result
1	Buka Cart	2 produk ditampilkan
2	Klik Remove pada Backpack	Backpack dihapus
3	Periksa Cart	Backpack tidak ditampilkan
4	Periksa Bike Light	Bike Light tetap ada
5	Periksa cart badge	Jumlah item berkurang menjadi 1

TC-CART-004 — Cart Count Validation
Field	Isi
Test Case ID	TC-CART-004
Scenario ID	TS-CART-004
Title	Validate cart item count
Module	Cart
Type	Validation
Priority	Medium
Preconditions	User login dan berada di Inventory
Test Data	3 produk berbeda

Step	Test Steps	Expected Result
1	Periksa Cart awal	Cart badge tidak menampilkan item
2	Tambahkan produk pertama	Badge menunjukkan 1
3	Tambahkan produk kedua	Badge menunjukkan 2
4	Tambahkan produk ketiga	Badge menunjukkan 3
5	Hapus satu produk	Badge menunjukkan 2

TC-CART-005 — Cart Data Consistency
Field	Isi
Test Case ID	TC-CART-005
Scenario ID	TS-CART-005
Title	Validate cart product data consistency
Module	Cart
Type	Positive
Priority	High
Preconditions	User login dan berada di Inventory
Test Data	Backpack dan Bike Light

Step	Test Steps	Expected Result
1	Tambahkan Backpack ke Cart	Backpack berhasil ditambahkan
2	Tambahkan Bike Light ke Cart	Bike Light berhasil ditambahkan
3	Buka Cart	Kedua produk ditampilkan
4	Periksa nama produk	Nama sesuai produk yang ditambahkan
5	Periksa harga produk	Harga sesuai Inventory
6	Periksa item di Cart	Tidak ada produk tambahan atau tertukar

TC-CART-006 — Empty Cart Edge Case
Field	Isi
Test Case ID	TC-CART-006
Scenario ID	TS-CART-006
Title	Remove all products from cart
Module	Cart
Type	Edge Case
Priority	Medium
Preconditions	User login dan Cart berisi beberapa produk
Test Data	2 produk atau lebih

Step	Test Steps	Expected Result
1	Buka Cart	Produk yang ditambahkan ditampilkan
2	Klik Remove pada produk pertama	Produk berhasil dihapus
3	Klik Remove pada seluruh produk tersisa	Semua produk dihapus
4	Periksa halaman Cart	Tidak ada produk yang tersisa
5	Periksa cart badge	Badge hilang atau menunjukkan 0 sesuai behavior aplikasi


5. Checkout Test Cases — 5 Test Cases
Requirement: RQ-005 · Scenario: TS-CHK-001 sampai TS-CHK-005
TC-CHK-001 — Checkout with Valid Information
Field	Isi
Test Case ID	TC-CHK-001
Scenario ID	TS-CHK-001
Title	Checkout with valid customer information
Module	Checkout
Type	Positive
Priority	High
Preconditions	User login, Cart berisi produk
Test Data	First Name: Budi / Last Name: Santoso / Postal Code: 15157

Step	Test Steps	Expected Result
1	Tambahkan produk ke Cart	Produk berhasil ditambahkan
2	Buka Cart	Produk ditampilkan
3	Klik Checkout	Halaman informasi customer ditampilkan
4	Input First Name	Data terisi
5	Input Last Name	Data terisi
6	Input Postal Code	Data terisi
7	Klik Continue	User berhasil lanjut ke Checkout Overview

TC-CHK-002 — Checkout Without First Name
Field	Isi
Test Case ID	TC-CHK-002
Scenario ID	TS-CHK-002
Title	Checkout without first name
Module	Checkout
Type	Negative
Priority	High
Preconditions	User login, Cart berisi produk, berada di halaman Your Information
Test Data	First Name: kosong / Last Name: Santoso / Postal Code: 15157

Step	Test Steps	Expected Result
1	Kosongkan First Name	First Name kosong
2	Isi Last Name	Last Name terisi
3	Isi Postal Code	Postal Code terisi
4	Klik Continue	Sistem menolak melanjutkan
5	Periksa pesan error	Pesan First Name required ditampilkan

TC-CHK-003 — Checkout Without Last Name
Field	Isi
Test Case ID	TC-CHK-003
Scenario ID	TS-CHK-003
Title	Checkout without last name
Module	Checkout
Type	Negative
Priority	High
Preconditions	User login, Cart berisi produk, berada di halaman Your Information
Test Data	First Name: Budi / Last Name: kosong / Postal Code: 15157

Step	Test Steps	Expected Result
1	Isi First Name	First Name terisi
2	Kosongkan Last Name	Last Name kosong
3	Isi Postal Code	Postal Code terisi
4	Klik Continue	Sistem menolak melanjutkan
5	Periksa pesan error	Pesan Last Name required ditampilkan

TC-CHK-004 — Checkout Without Postal Code
Field	Isi
Test Case ID	TC-CHK-004
Scenario ID	TS-CHK-004
Title	Checkout without postal code
Module	Checkout
Type	Negative
Priority	High
Preconditions	User login, Cart berisi produk, berada di halaman Your Information
Test Data	First Name: Budi / Last Name: Santoso / Postal Code: kosong

Step	Test Steps	Expected Result
1	Isi First Name	First Name terisi
2	Isi Last Name	Last Name terisi
3	Kosongkan Postal Code	Postal Code kosong
4	Klik Continue	Sistem menolak melanjutkan
5	Periksa pesan error	Pesan Postal Code required ditampilkan

TC-CHK-005 — Product and Price Validation
Field	Isi
Test Case ID	TC-CHK-005
Scenario ID	TS-CHK-005
Title	Validate product and order price in checkout overview
Module	Checkout
Type	Validation
Priority	High
Preconditions	User login dan berada di Inventory
Test Data	Backpack $29.99 dan Bike Light $9.99

Step	Test Steps	Expected Result
1	Tambahkan Backpack ke Cart	Backpack ditambahkan
2	Tambahkan Bike Light ke Cart	Bike Light ditambahkan
3	Buka Cart	2 produk ditampilkan
4	Klik Checkout dan isi data valid	User lanjut ke Overview
5	Periksa nama dan harga produk	Nama dan harga sesuai Cart
6	Periksa subtotal	Subtotal = $39.98
7	Periksa tax	Tax sesuai perhitungan sistem
8	Periksa total	Total = Subtotal + Tax

Catatan: Tax dan Total harus dicocokkan dengan hasil perhitungan aplikasi. Jangan mengasumsikan tax sebelum melihat hasil aktual.

6. Order Completion Test Cases — 4 Test Cases
Requirement: RQ-006 · Scenario: TS-ORD-001 sampai TS-ORD-004
TC-ORD-001 — Complete Order Successfully
Field	Isi
Test Case ID	TC-ORD-001
Scenario ID	TS-ORD-001
Title	Complete order successfully
Module	Order
Type	Positive
Priority	High
Preconditions	User sudah sampai di Checkout Overview
Test Data	Produk dan customer information valid

Step	Test Steps	Expected Result
1	Periksa halaman Checkout Overview	Produk dan informasi order ditampilkan
2	Klik Finish	Order berhasil diproses
3	Verifikasi halaman selanjutnya	User diarahkan ke halaman Order Complete
4	Periksa status halaman	Tidak ada error saat order diselesaikan

TC-ORD-002 — Order Confirmation Validation
Field	Isi
Test Case ID	TC-ORD-002
Scenario ID	TS-ORD-002
Title	Verify order confirmation message
Module	Order
Type	Validation
Priority	High
Preconditions	User berhasil menyelesaikan order
Test Data	Order yang sudah berhasil di-Finish

Step	Test Steps	Expected Result
1	Selesaikan checkout hingga halaman Overview	Overview ditampilkan
2	Klik Finish	Order selesai diproses
3	Periksa halaman konfirmasi	Halaman order confirmation ditampilkan
4	Periksa pesan konfirmasi	Pesan Thank You for Your Order ditampilkan
5	Periksa informasi order	Informasi bahwa order berhasil diselesaikan ditampilkan

TC-ORD-003 — Back Home Navigation
Field	Isi
Test Case ID	TC-ORD-003
Scenario ID	TS-ORD-003
Title	Navigate back to inventory after order completion
Module	Order
Type	Positive
Priority	Medium
Preconditions	User berada di halaman Order Complete
Test Data	Order yang telah selesai

Step	Test Steps	Expected Result
1	Periksa halaman Order Complete	Halaman konfirmasi ditampilkan
2	Klik Back Home	User diarahkan kembali
3	Periksa halaman tujuan	Inventory ditampilkan
4	Periksa daftar produk	Produk dapat ditampilkan kembali

TC-ORD-004 — Cart Data Consistency After Order
Field	Isi
Test Case ID	TC-ORD-004
Scenario ID	TS-ORD-004
Title	Verify cart is empty after completed order
Module	Order
Type	Data Consistency
Priority	High
Preconditions	User login dan Cart berisi produk
Test Data	Sauce Labs Backpack dan Sauce Labs Bike Light

Step	Test Steps	Expected Result
1	Tambahkan 2 produk ke Cart	2 produk berhasil ditambahkan
2	Buka Cart	Kedua produk ditampilkan
3	Klik Checkout	Halaman informasi customer ditampilkan
4	Isi First Name, Last Name, dan Postal Code	Seluruh informasi terisi
5	Klik Continue	Checkout Overview ditampilkan
6	Klik Finish	Order berhasil diselesaikan
7	Klik Back Home	User kembali ke Inventory
8	Buka Cart	Cart kosong, tidak ada produk dari transaksi sebelumnyaTest cases document for E-Commerce Manual QA Project.
