# TEST SCENARIOS
## E-Commerce Web Application

Application: SauceDemo
Testing Method: Black Box Testing
Testing Type: Manual Testing

| Scenario ID | Requirement ID | Module | Test Scenario | Type | Priority |
|---|---|---|---|---|---|
| TS-LOGIN-001 | RQ-001 | Login | Memastikan user berhasil login dengan credential valid | Positive | High |
| TS-LOGIN-002 | RQ-001 | Login | Memastikan login ditolak jika password salah dengan username valid | Negative | High |
| TS-LOGIN-003 | RQ-001 | Login |Memastikan login ditolak jika username salah dengan password valid | Negative | High |
| TS-LOGIN-004 | RQ-001 | Login |Memastikan login ditolak apabila tanpa input username valid | Negative | High|
| TS-LOGIN-005 | RQ-001 | Login | Memastikan login ditolak apabila tanpa input password valid | Negative | High |
| TS-LOGIN-006 | RQ-001 | Login | Memastikan login ditolak ketika user menggunakan akun yang terkunci dengan credential yang sesuai | Negative | High |
| TS-INV-001 | RQ-002 | Inventory | Memastikan halaman inventory berhasil ditampilkan setelah user login | Positive | High |
| TS-INV-002 | RQ-002 | Inventory | Memastikan seluruh produk ditampilkan sesuai daftar produk yang tersedia | Positive | High |
| TS-INV-003 | RQ-002 | Inventory | Memastikan setiap produk menampilkan nama dan harga yang sesuai | Positive | High |
| TS-INV-004 | RQ-002 | Inventory | Memastikan gambar setiap produk ditampilkan dengan benar dan sesuai dengan produk terkait | Positive | Medium |
| TS-INV-005 | RQ-002 | Inventory | Memastikan halaman detail menampilkan informasi sesuai produk yang dipilih dari inventory | Positive | Medium |
| TS-SORT-001 | RQ-003 | Sorting | Memastikan produk diurutkan berdasarkan nama secara ascending (A–Z) ketika user memilih opsi Name (A to Z) | Positive | Medium | 
| TS-SORT-002 | RQ-003 | Sorting | Memastikan produk diurutkan berdasarkan nama secara descending (Z–A) ketika user memilih opsi Name (Z to A) | Positive | Medium |
| TS-SORT-003 | RQ-003 | Sorting | Memastikan produk diurutkan berdasarkan harga dari terendah ke tertinggi ketika user memilih Price (low to high) | Positive | High |
| TS-SORT-004 | RQ-003 | Sorting | Memastikan produk diurutkan berdasarkan harga dari tertinggi ke terendah ketika user memilih Price (high to low) | Positive | High |
| TS-CART-001 | RQ-004 | Cart | Memastikan user berhasil menambahkan satu produk ke shopping cart | Positive | High |
| TS-CART-002 | RQ-004 | Cart | Memastikan user berhasil menambahkan beberapa produk ke shopping cart | Positive | High |
| TS-CART-003 | RQ-004 | Cart | Memastikan user berhasil menghapus produk yang dipilih dari shopping cart | Positive | High |
| TS-CART-004 | RQ-004 | Cart | Memastikan jumlah item pada cart bertambah sesuai jumlah produk yang ditambahkan | Validation | Medium |
| TS-CART-005 | RQ-004 | Cart | Memastikan produk dan informasi yang ditampilkan di cart sesuai dengan produk yang dipilih user | Positive | High |
| TS-CART-006 | RQ-004 | Cart | Memastikan seluruh produk dapat dihapus dan cart menampilkan kondisi kosong | Positive | Medium |
| TS-CHK-001 | RQ-005 | Checkout | | | |
| TS-CHK-002 | RQ-005 | Checkout | | | |
| TS-CHK-003 | RQ-005 | Checkout | | | |
| TS-CHK-004 | RQ-005 | Checkout | | | |
| TS-CHK-005 | RQ-005 | Checkout | | | |
| TS-ORD-001 | RQ-006 | Order | | | |
| TS-ORD-002 | RQ-006 | Order | | | |
| TS-ORD-003 | RQ-006 | Order | | | |
| TS-ORD-004 | RQ-006 | Order | | | |


## Requirement Traceability Matrix (RTM)

| Requirement ID | Requirement | Test Scenario IDs | Coverage Status |
|---|---|---|---|
| RQ-001 | Login | | |
| RQ-002 | Inventory | | |
| RQ-003 | Sorting | | |
| RQ-004 | Shopping Cart | | |
| RQ-005 | Checkout | | |
| RQ-006 | Order Completion | | |

## Scenario Summary

- Total Test Scenarios: 30
- Positive Scenarios:
- Negative Scenarios:
- Edge Case Scenarios:

Status: In Progress
