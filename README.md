# repositoriNurita

# PENGEMBANGAN OPEN SOURCE
# TEKNOLOGI OPEN SOURCE DAN TERBARU
# KELOMPOK 2

## The Cathedral & The Bazaar
### Sejarah
* Essay tentang metode Software Engineering dari Eric S. Raymond dipresentasikan di Linux Kongress pada May 27, 1997.
* Diterbitkan sebagai buku “The Cathedral and the Bazaar: Musings on Linux and Open Source by an Accidental Revolutionary” (CatB) pada 1999

### Definisi
Model pengembangan suatu sistem bisa mengambil pendekatan salah satu model, yakni model Cathedral atau model Bazaar. Ada istilah lain untuk kedua model tersebut, yakni Top Down dan Bottom Up.

### The Cathedral Model
Pada model Cathedral, hanya kaum elit yang bisa mengembangkan sistem. Setelah sistem tersebut jadi, merekalah yang mempunyai hak untuk menyebarkan sistem tersebut kepada para pengguna sistem.  
Pada model pertama (Cathedral), proses peer review terjadi di dalam khalayak elit (para pengembang sistem saja).
Model Cathedral biasanya lebih lambat dalam mengikuti keinginan pemakai.

### The Bazaar Model
Pada model Bazaar, orang yang merasa mampu mengembangkan sistem akan diberikan kesempatan untuk menyajikan sistem rancangannya ke khalayak ramai dan secara terbuka menerima saran/feedback bila ada bug atau kekurangan. Hasil revisinya pun bisa disajikan ke khalayak ramai kembali.  
Pada proses kedua, peer review terjadi lebih luas, baik dari kalangan pengguna sistem maupun para peer reviewer (pemberi feedback tadi).

### Kelebihan The Bazaar
1. Dapat menemukan dan memperbaiki bug atau kekurangan dengan cepat
2. Lebih cepat dan lebih terbuka
3. Proses peer review dapat dilakukan oleh siapa saja yang mampu mengembangkan sistem

### Kekurangan The Bazaar
1. GUI dari software yang dibuat dengan model the bazaar biasanya kurang memuaskan untuk pengguna yang awam.
2. Kesulitan dalam mengenakan biaya untuk sesuatu yang bisa didapatkan secara gratis.
3. Rilis terlalu sering sehingga beberapa diantaranya masih belum stabil

### Contoh Software Open Source The Bazaar
1. Linux
2. Apache
3. GNU Image Manipulation Program (GIMP)
4. Wikipedia

## Versioning
Sebuah proses untuk memberikan nama atau nomor yang unik untuk sebuah software. Dalam kategori nomor, angka ini diberikan dalam rangka peningkatan dan perkembangan yang lebih baru dari sebuah pengembangan software

### Versioning: Semantic Version
Pada umumnya sebuah software yang rilis memiliki versi. Versi Software adalah sebuah pemberian nomor atau angka yang bersifat unik kepada sebuah software untuk menerangkan status software tersebut.  
Nomor versi software diberikan secara berurut dan meningkat mengikuti Rilis software tersebut.  
Dengan memberikan versi pada sebuah software akan memudahkan dalam meng-organisir source code sebuah software yang bermanfaat bagi developer maupun pengguna sofware. Dan dapat berfungsi sebagai history perkembangan sebuah software.

![Semantic Version Rule](https://muut.com/help/img/semantic.png)

**Aturan Pertama**  
Sebuah nomor versi software berpola X.Y.Z di mana X, Y, dan Z adalah bilangan bulat.  
X adalah versi mayor  
Y adalah versi minor  
Z versi patch  
Setiap rilis maka elemen versi sofware HARUS meningkat, Sebagai contoh seperti dibawah ini  
Rilis ke 1 >> 1.0.0  
Rilis ke 2 >> 1.0.1  
Rilis ke 3 >> 1.1.1  
Rilis ke 4 >> 2.0.0  

**Aturan Kedua**  
Untuk versi software dalam fase Release Life Cycle Software dapat ditambahkan dengan AlphaNumerics [0-9A-Za-z] & simbol strip dan serta diawali karakter alpha [A-Za-z], Sebagai contoh adalah sebagai berikut.  
Versi 1.0.0 Alpha ke 1 >> 1.0.0alpha1  
Versi 1.0.0 Alpha ke 2 >> 1.0.0alpha2  
Versi 1.0.0 Beta ke 1 >> 1.0.0beta1  
Versi 1.0.0 Beta ke 2 >> 1.0.0beta2  

**Aturan ketiga**  
Setelah sebuah versi software rilis maka setiap ada modifikasi dari source code software tersebut akan melahirkan rilis versi yang baru.

**Aturan Keempat**  
Angka pada versi patch harus bertambah apabila terjadi perbaikan bug/error dari sebuah versi software, sebagai contoh.  
Perbaikan bug/error di Versi 1.0 ke 1 >> 1.0.1  
Perbaikan bug/error di Versi 1.0 ke 2 >> 1.0.2  
Perbaikan bug/error di Versi 1.0 ke 3 >> 1.0.3  
Perbaikan bug/error di Versi 1.0 ke 4 >> 1.0.4  

**Aturan kelima**  
Versi minor pada versi software harus bertambah jika terdapat modul/fungsional baru yang kompatibel dengan versi mayor atau terjadi perbaikan yang besar pada versi software tersebut.  
Penambahan fungsional di Versi 1 ke 1 >> 1.1.0  
Penambahan fungsional di Versi 1 ke 2 >> 1.2.0  
Penambahan fungsional di Versi 1 ke 3 >> 1.3.0  
Penambahan fungsional di Versi 1 ke 4 >> 1.4.0  

**Aturan keenam**  
Versi mayor pada versi software harus bertambah apabila terjadi perubahan yang menyebabkan modul/fungsional yang telah ada sebelumnya menjadi tidak kompatibel, hal ini biasa terjadi apabila ada  perubahan pada kode program yang bersifat core/inti atau fundamental dari sofware tersebut.  
Perubahan core software ke 1 >> 2.0.0  
Perubahan core software ke 2 >> 3.0.0  
Perubahan core software ke 3 >> 4.0.0  

**Contoh Semver Software**  
GO-JEK  
Versi terbaru: 2.6.1  
Instagram  
Versi terbaru: 9.4.0  
Line  
Versi terbaru: 6.6.2  
WhatsApp Messenger  
Versi terbaru: 2.16.275  
Youtube  
Versi terbaru: 11.35.60  

### Versioning: Sequential
**Penjelasan**
Skema berbasis urutan adalah skema yang paling umum digunakan, di mana setiap versi adalah urutan nilai-nilai numerik biasanya dipisahkan dengan titik (.):  
1.0  
1.1  
1.0.1  
1.3.4  
Skema berbasis sequence yang paling sering adalah:  
MAJOR.MINOR[.MICRO]  
**Contoh software:**  
Internet Explorer 5 dari 5.1 - 5.5  

### Versioning: Tanggal
**Penjelasan**  
Skema versioning tanggal yaitu penggunaan format tanggal, bulan, dan atau tahun untuk pengkodean rilis suatu perangkat lunak sesuai dengan waktu rilis perangkat lunak tersebut.  
**Contoh software:**  
Wine: "Wine 20040505".  
Ubuntu Linux: 11.10, artinya, dirilis Oktober 2011.  
Microsoft Office: 3419, dua angka pertama adalah jumlah bulan berlalu dari proyek dimulai (dengan setiap rilis Office utama adalah proyek yang berbeda), dan dua angka terakhir adalah hari. Jadi 3419 adalah hari ke-19 bulan ke-34 setelah bulan Januari tahun proyek dimulai.

### Versioning: Bebas
**Penjelasan**  
Skema versioning tidak memiliki format atau ketentuan khusus dan biasanya versioning ini digunakan untuk branding terhadap perangkat lunak yang telah dirilis oleh pengembang.  
**Contoh software:**  
Microsoft Windows XP  
Microsoft Windows 10  
Microsoft Windows Vista  

## Github
Github adalah layanan hosting repository git berbasis web. Web ini menawarkan semua distribusi untuk mengontrol versi dan manajemen source code (SCM) dari git. Web ini menyediakan control akses dan beberapa fitur kolaborasi misalnya, pelacakan bug, fitur permintaan, manajemen tugas dan wiki untuk setiap project.

### Repository
* Repository baru  
`git init [project-name]`  
* Menambah file  
`git add [file]`  
* Commit & Push  
`git commit -m "[descriptive message]" && git push`  
* Remote Origin  
`git remote add origin https://github.com/username/myproject.git`

### Rilis
* Buat akun github terlebih dahulu di github.com  
* Install git ( https://git-scm.com/downloads ) atau “_sudo apt-get install git_” bagi pengguna linux.
* Buat repositori baru di github.com kemudian clone di komputer  
`git clone https://github.com/usermu/repositorinya.git`
* Add, commit & push  
`git add *`  
`git commit -m "Describe Your Work Here"`  
`git push`  

### Branch
* Membuat branch baru  
`git checkout -b dev`  
* Melihat list branch  
`git branch`  
* Pindah antar branch  
`git checkout dev`

### Merge Patch
* Pindah ke branch dev  
`git checkout dev`  
* Buat file baru, add, commit & push di branch dev.  
`git add *`  
`git commit -m  "Describe Your Work Here"`  
`git push origin dev`  
* Pindah ke branch utama  
`git checkout master`  
* Periksa perubahan baru yang baru dibuat dengan branch utama  
`git diff master dev`  
* Merge branch dev dengan branch utama (master)  
`git merge dev`  
* Push perubahan di branch utama  
`git push origin master`  
* Periksa status di branch utama  
`git status`  

### Markdown
Markdown adalah cara untuk memformat teks pada website. Kita dapat mengontrol tampilan dari dokumen dengan memformat kata atau huruf menjadi tebal atau miring, menambahkan gambar, membuat list dan masih banyak lagi yang bisa dilakukan dengan Markdown. Markdown umumnya hanya berisi teks biasa dengan beberapa karakter non alfabet seperti # atau *.

## Daftar Pustaka
* [http://gemabuj.github.io/post-the-cathedral/index.html](http://gemabuj.github.io/post-the-cathedral/index.html)
* [http://the-hitchhikers-guide-to-packaging.readthedocs.io/en/latest/specification.html](http://the-hitchhikers-guide-to-packaging.readthedocs.io/en/latest/specification
