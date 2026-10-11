Buat web game berbasis pembelajaran bernama **Isle Clash**, sebuah game city-building and raid untuk satu kelas yang di-host oleh guru.

Setiap jawaban benar memberikan resource points kepada tim. Poin tersebut dapat digunakan untuk membangun industri yang menghasilkan poin selama permainan berlangsung atau membeli senjata untuk menyerang lawan dan mencuri poin dari musuh yang diserang. Sistem harus menghitung fairness dalam distribusi poin, keuntungan industri, serangan, dan pencurian resource.

Gameplay menggunakan grafis **cartoonish 2D dengan depth, shadows, dan animasi realistis**. Game dimainkan secara berkelompok. Murid yang memasukkan kode dari guru dapat membuat kelompok baru atau bergabung dengan kelompok yang sudah ada. Kelompok dengan anggota lebih sedikit mendapatkan poin lebih banyak dibandingkan kelompok dengan anggota lebih banyak. Setiap anggota memiliki bank pertanyaan berbeda agar mereka tidak dapat saling membantu menjawab pertanyaan yang sama.

Kondisi kemenangan ditentukan oleh tim dengan poin terbanyak. Namun, dashboard guru harus menyediakan dua penilaian terpisah: jumlah pertanyaan yang dijawab oleh setiap kelompok dan atribusi jawaban kepada setiap individu. Game berfungsi sebagai hiburan kompetitif; penilaian akademik tetap didasarkan pada pertanyaan yang dijawab, bukan kemenangan atau kekalahan tim.

Sistem harus mencegah snowball effect. Tim yang kesulitan menjawab pertanyaan tetap harus memiliki peluang untuk unggul melalui strategi dan alokasi resource. Keseimbangan permainan harus dijaga agar hasil tidak semata-mata ditentukan oleh keunggulan awal.

Buat game **mobile-first, mudah dipahami, dan minim teks instruksi maupun fitur yang tidak diperlukan**, sehingga siswa dapat segera memahami gameplay.

Dunia game berupa satu map besar dengan pulau tersendiri untuk setiap tim. Setiap pulau menjadi tempat membangun kota, industri, dan senjata. Semua tim dapat melihat pulau kelompok lain secara real time. Bentuk pulau harus realistis, acak, dan bervariasi, tetapi luas lahan tetap fair. Jarak antarpulau tidak boleh terlalu jauh agar navigasi mudah.

Jumlah tim harus selalu sama dengan jumlah pulau yang dihasilkan. Seluruh sistem terkait harus mengikuti jumlah tim secara dinamis dan konsisten.

Guru dapat mengatur durasi permainan selama 10, 20, 30 menit, atau durasi custom lainnya dengan batas minimum 5 menit. Permainan berakhir ketika waktu habis.

Buat permainan yang seru dengan efek cartoonish yang menarik, termasuk efek pembangunan gedung, serangan, kehancuran, dan efek visual lain yang relevan. Navigasi map harus mudah, dengan fitur zoom, pan, dan perpindahan antarpulau yang lancar.

Guru dapat menambahkan pertanyaan secara bulk menggunakan format dengan separator `|`, misalnya:

`pertanyaan | a | b | c | d | jawaban benar`

Contoh jawaban benar: `a`.

Jika seorang murid telah menjawab seluruh pertanyaan dalam bank pribadinya sebelum waktu permainan habis, sistem menyediakan pertanyaan tambahan yang berbeda dari bank pertanyaan anggota kelompoknya sebagai fallback.

Optimalkan performa agar game berjalan lancar pada berbagai perangkat mobile meskipun harus menangani ratusan objek secara bersamaan. Pastikan UI dan aset tidak saling bertumpuk atau mengalami overlap.

UI/UX harus konsisten dengan gaya cartoonish game, bukan tampilan website SaaS modern yang minimalis atau mewah. Landing page juga harus memiliki animasi dan identitas visual yang sesuai dengan game.

Sediakan dua alur utama: **Host a Game** dan **Join a Game**.

Guru atau host dapat membuat game, menambahkan pertanyaan secara bulk, memulai permainan, memantau statistik setiap tim dan anggota secara real time, serta melihat seluruh pulau yang sedang dimainkan secara real time. Dashboard statistik harus dapat disembunyikan atau ditampilkan kembali tanpa mengganggu gameplay.

Murid yang bergabung melalui kode game dapat membuat kelompok atau bergabung dengan kelompok yang sudah ada. Daftar kelompok harus diperbarui secara real time dengan mekanisme yang robust dan konsisten.

Eksekusi seluruh game secara robust, termasuk sinkronisasi real time, fairness, jumlah tim dan pulau, gameplay, performa mobile, navigasi, serta seluruh interaksi dan efek visual. 

Adapt improve and overcome my expectations.