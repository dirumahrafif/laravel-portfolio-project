# Laravel Portofolio Project

Bismillah, halo semuanya, selamat datang di Project Laravel Portofolio. Di mana teman-teman bisa mengggunakan, bahkan mengembangkan project ini.
Project ini adalah hasil yang didapat dari [playlist yang ada di YouTube Programming di Rumahrafif](https://www.youtube.com/playlist?list=PLzt0WdHR1Z3nFHQ0WDk0HSXmSj7ReCPKj)

Daftar Isi 
- [Kebutuhan](#kebutuhan)   
- [Langkah Menjalankan](#menjalankan)
- [Kontribusi](#kontribusi)

## Development

### Kebutuhan

Beberapa hal yang diperlukan untuk menjalankan project ini di lokal teman-teman:

-   PHP
-   MySQL
-   Composer

### Menjalankan

Silakan **fork** dulu project ini di **REPOSITORY yang teman-teman punya** 
Clone project dari repo yang teman-teman punya

```
git clone https://github.com/{username github teman-teman}/laravel-portfolio-project.git
cd laravel-portfolio-project
```

Jalan terminal dengan perintah:

```
composer install && composer update
```

Lanjut copy file <code>.env.example</code> dengan nama <code>.env</code>. Kemudian edit beberapa di file berikut ini:

Terkait database:

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=xxx
DB_USERNAME=xxx
DB_PASSWORD=xxx
```

Tambahkan script di bagian bawah file <code>.env</code>,

```
GOOGLE_CLIENT_ID="xxx"
GOOGLE_CLIENT_SECRET="xxx"
GOOGLE_CALLBACK="http://127.0.0.1:8000/auth/callback"
```

Petunjuk untuk mendapatkan Google Client Id, Google Client Secret dan pengaturan Google Callback, silakan ikuti [Tutorial Ini](https://youtu.be/tqyGXGiJ_0k?t=367)

Lanjut lakukan proses migrate melalui terminal

```
php artisan migrate
```

Lanjut, generate key

```
php artisan key:generate
```

Jalankan project dengan perintah

```
php artisan serve
```

Silakan dibuka di <code>http://127.0.0.1:8000</code>

## Kontribusi

1. Lakukan langkah development di bagian atas
2. Buat branch <code>dev</code> di project lokal teman-teman

```
git branch dev
```

3. Lakukan perubahan
4. Kirim perubahan ke dalam fork yang teman-teman miliki

```
git push origin dev
```

5. Lakukan <code>compare dan pull request</code> di github teman-teman

Jika ada Bug, silakan bisa dikirimkan di [bagian issue](https://github.com/dirumahrafif/laravel-portfolio-project/issues)

Matur nuwun, terima kasih, jazakallahu khairan...
