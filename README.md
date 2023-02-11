# Pengaturcaraan Rust

![Build Status](https://github.com/rust-lang/book/workflows/CI/badge.svg)

Repositori ini mengandungi sumber kepada buku "Pengaturcaraan Rust".


[Buku ini tersedia dalam format dead-tree dari No Starch Press][nostarch].

[nostarch]: https://nostarch.com/rust-programming-language-2nd-edition

Anda juga boleh membaca buku ini secara percuma dalam talian. Sila rujuk kepada 
buku terbitan terkini [stable], [beta], atau [nightly] Rust. Perlu diingat
bahawa isu-isu di dalam versi-versi tersebut mungkin telah diperbetulkan 
di dalam repositori ini, kerana terbitan tersebut tidak selalu dikemas kini.

[stable]: https://doc.rust-lang.org/stable/book/
[beta]: https://doc.rust-lang.org/beta/book/
[nightly]: https://doc.rust-lang.org/nightly/book/

Sila lihat [releases] untuk muat turun kod sumber yang digunakan dalam buku ini.

[releases]: https://github.com/rust-lang/book/releases

## Syarat-syarat

Pengompilan buku ini memerlukan [mdBook], secara idealnya dengan
menggunakan versi yang sama diguna pakai rust-lang/rust dalam [fail ini][rust-mdbook].
Untuk mendapatkannya:

[mdBook]: https://github.com/rust-lang-nursery/mdBook
[rust-mdbook]: https://github.com/rust-lang/rust/blob/master/src/tools/rustbook/Cargo.toml

```bash
$ cargo install mdbook --version <version_num>
```

## Pengompilan

Untuk mengompil buku ini, taip:

```bash
$ mdbook build
```

Hasil pengompilan akan berada di dalam `book` subdirektori. Sila gunakan 
pelayar untuk memastikan hasil tersebut.


_Firefox:_
```bash
$ firefox book/index.html                       # Linux
$ open -a "Firefox" book/index.html             # OS X
$ Start-Process "firefox.exe" .\book\index.html # Windows (PowerShell)
$ start firefox.exe .\book\index.html           # Windows (Cmd)
```

_Chrome:_
```bash
$ google-chrome book/index.html                 # Linux
$ open -a "Google Chrome" book/index.html       # OS X
$ Start-Process "chrome.exe" .\book\index.html  # Windows (PowerShell)
$ start chrome.exe .\book\index.html            # Windows (Cmd)
```

Untuk melaksanakan ujian:

```bash
$ mdbook test
```

## Menyumbang

Kami mengalu-alukan sumbangan anda! Sila lihat [CONTRIBUTING.md][contrib] untuk mengetahui
tentang jenis-jenis sumbangan yang kami perlukan.

[contrib]: https://github.com/rust-lang/book/blob/main/CONTRIBUTING.md

Disebabkan buku ini di[cetak][nostarch], dan disebabkan kami mahu kekalkan
versi dalam talian hampir sama yang mungkin (dengan cetakan), ianya agak memakan
masa yang lebih lama untuk melayani isu anda atau "pull request".

Setakat ini, kami sedang melaksanakan semakan yang lebih besar bertepatan dengan
[Edisi Rust](https://doc.rust-lang.org/edition-guide/). Diantara revisi besar tersebut, 
hanya pembetulan kepada kesalahan sahaja akan dibuat. Jikalau isu atau "pull request" anda
adalah bukannya pembetulan kesalahan, ianya mungkin akan ditangguhkan sehingga revisi besar
yang berikutnya yang akan mengambil masa beberapa bulan atau tahun. Harap bersabar!

### Terjemahan

Kami mengalu-alukan sumbangan untuk menterjemahkan buku ini!. Rujuk kepada [Translations] label
untuk menyertai usaha-usaha yang sedang berlansung. Untuk terjehamahan yang baharu, sila buka
isu baharu untuk memulakan kerja tersebut! Anda boleh teruskan terjemahan itu sementara kami 
menunggu [mdbook support] untuk pelbagai bahasa sebelum kerja-kerja penggabungan dibuat.

[Translations]: https://github.com/rust-lang/book/issues?q=is%3Aopen+is%3Aissue+label%3ATranslations
[mdbook support]: https://github.com/rust-lang-nursery/mdBook/issues/5

## Penyemakan Ejaan

Untuk mengibas kesalahan ejaan di dalam fail sumber, `spellcheck.sh` skrip 
di dalam `ci` direktori boleh digunakan. Ia memerlukan kamus yang terdiri 
daripada senarai perkataan yang sah, seperti yang disediakan dalam `ci/dictionary.txt`.
Jika skrip tersebut menghasilkan positif palsu (contoh: perkataan `BTreeMap` adalah 
tidak sah bagi imbasan skrip), perkataan tersebut perlulah ditambah kepada 
`ci/dictionary.txt` (susun mengikut aturan supaya kekal konsistent)
