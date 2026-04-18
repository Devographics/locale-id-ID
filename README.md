# locale-id-ID

Repo ini berisi berkas-berkas bahasa Indonesia untuk survei State of JS/CSS/dll.

## Cara berkontribusi

### 1. Menjadi penerjemah

Untuk memulai menerjemahkan survei, anda harus bergabung ke dalam server Discord
dan DM saya (`sachaG`) username GitHub anda, bersama dengan kode locale (id-ID, fr-Fr,
dll.) untuk bahasa yang ingin anda terjemahkan.

Saya akan memberikan anda hak pengelola atas sebuah repo yang berisikan berkas-berkas
`yaml` untuk penerjemahan, dan setelah itu anda dapat mengelolanya sendiri
bersaama dengan anggota tim penerjemah lainnya.

### 2. Menemukan hal-hal untuk diterjemahkan

Anda bisa menjelajahi aplikasi untuk mengisi survei, situs hasil survei, dll.
dan menemukan string yang belum diterjemahkan, atau menggunakan API kami untuk
mendapatkan data lebih misalnya persentasi penyelesaian untuk sebuah locale tertentu
atau sebuah daftar dari semua string yang belum diterjemahkan:

[https://graphiql.devographics.com/]

Contoh sampel survei:

```graphql
query GetLocaleData {
  locale(localeId: ru_RU) {
    completion
    totalCount
    translatedCount
    translators
    untranslatedKeys
  }
}
```

### 3. Mendapatkan penghargaan

Setiap penerjemah akan mendapatkan penghargaan dalam situs manapun yang menggunakan terjemahannya, dimulai dari aplikasi pengambilan surveinya. Untuk mendapatkan penghargaan, tambahkan username Github Anda di dalam array `translators` dalam file `config.yml`.

Nama dapat ditambahkan di sini:

- https://github.com/Devographics/locale-id-ID/blob/main/config.yml#L3

### 4. Membuat perubahan anda terlihat

Untuk saat ini tidak ada hook terotomasi untuk memperbarui aplikasi produksi
ketika sudah selesai menerjemahkan, jadi untuk sekarang cara terbaik adalah untuk
mengirimkan pesan pribadi kepada saya (`sachaG`) di Discord untuk memberitahu saya ketika
Anda sudah selesai.

## Berkas-berkas penerjemahan

### Aplikasi survei

String-string berikut berkaitan dengan aplikasi yang dipakai untuk mengisi survei:

- `surveys.yml`
- `accounts.yml`
- `state_of_js_2020_survey.yml`

### Aplikasi hasil

String-string hanya muncul dalam situs web statis yang menampilkan hasil dan
statistik survei.

- `results.yml`
- `state_of_css_2020.yml`
- `state_of_js_2020.yml`

### Dua-duanya

String-string berikut muncul dalam keduanya.

- `common.yml`
- `state_of_css.yml`
- `state_of_js.yml`

### Lainnya

- `homepage.yml`

## Dapatkan bantuan

Bergabung dengan [Discord kami](https://discord.gg/zRDb35jfrt).
