# dVote App by F3rwell

## Anggota

1. Fabiansyah Raam Pontoh (185150200111088)
2. Mohammad Zulfikar (185150207111014)
3. Muhammad Fikri Ashari (185150200111017)
4. Muhammad Rafi Fauzan Fathin (185150200111018)

## Deskripsi

Pada negara yang memiliki bentuk pemerintahan demokrasi dan menjunjung tinggi demokrasi, pasti sudah tidak asing dengan sistem voting atau pemungutan suara. Sering kita temui bahwa pemungutan suara secara tradisional (seseorang datang langsung ke tempat pemilihan dan memilih pada kotak suara) berlangsung secara lama dalam proses perhitungannya. Adapun, solusi voting dengan menggunakan app menjadi alternatif di beberapa negara atau daerah, terlebih di era pandemi seperti ini. Akan tetapi, dengan menggunakan aplikasi yang menggunakan database tradisional adalah bisa saja beberapa pihak tertentu yang memiliki power, mencoba mengubah database baik secara langsung ataupun semisal dengan memberikan ancaman terhadap pengelola database. Hal ini tentu dapat membuat proses demokrasi menjadi cacat dan tidak berdasarkan asas luberjurdil yang diharapkan. Dengan menggunakan teknologi blockchain, kita bisa mengatasi hal tersebut karena nantinya setiap transaksi (ketika seseorang melakukan voting) akan tercatat dan bersifat *immutable*. Dengan begitu kecacatan yang dapat muncul dari segi teknologi dapat dikecilkan atau dihindari,

Atas dasar tersebut kami membuat aplikasi decentralized voting yang dapat melakukan pencatatan voting. Beberapa fungsionalitas utama yang kami hadirkan diantaranya,

1. Melakukan voting terhadap calon yang telah dibuat
2. Mencatat siapa saja "akun" (wallet) yang telah melakukan voting
3. Menampilkan grafik perolehan suara secara *real-time*

## Implementasi

Kami membuat aplikasi dVote dengan tech stack sebagai berikut,

- Frontend: HTML, CSS, JS
- Backend: Ethereum (Solidity)
- Blockchain Network: Geth

## Pengujian

Kami melakukan pengujian dengan skenario pembatasan voter atau pemungut suara menjadi 3. Ketika total yang melakukan pemungutan suara sudah berjumlah total 3, maka tidak ada yang bisa melakukan vote. Jumlah maksimal pemungut suara dapat diganti nantinya sesuai jumlah yang diinginkan.

## Menjalankan Aplikasi

### Install Dependensi

```bash
npm install
```

### Buat Jaringan Ethereum

Buat jaringan private ethereum menggunakan geth atau hyperledger besu, atau jika ingin hanya mencoba di lokal bisa menggunakan [Ganache](https://www.trufflesuite.com/ganache).

### Kompilasi dan Deploy Smart Contract

Lakukan migrasi untuk membuat koneksi ke jaringan ethereum.

```bash
truffle migrate --reset
```

### Konfigurasi Metamask

Pastikan [metamask](https://metamask.io/) telah terpasang di browser. Buatlah koneksi dengan jaringan ethereum anda (private atau local) dan lakukan import akun dengan informasi yang di dapat dari jaringan ethereum.

### Jalankan Aplikasi

Gunakan command `npm` untuk menjalankan aplikasi

```bash
npm run dev
```

Aplikasi akan berjalan di http://localhost:3000
