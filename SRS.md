<ol>
<b>1.1	Tujuan</b>
	<ol>
	Dokumen ini berisi Spesifikasi Kebutuhan Perangkat Lunak (SKPL) atau Software Requirement Spesification (SRS)  untuk Sistem Penjualan Aksesoris dan Sparepart Handphone.Tujuan dari penulisan dokumen ini adalah untuk memberikan penjelasan mengenai perangkat lunak yang akan dibangun baik berupa gambaran umum maupun penjelasan detil dan menyeluruh.<br>
	Pengguna dari dokumen ini adalah pengembang perangkat lunak sistem Penjualan Aksesoris dan Sparepart Handphone pengguna (user) dari perangkat lunak atau personil-personil yang terlibat dalam sistem.Dokumen ini akan digunakan sebagai bahan acuan dalam proses pengembangan dan sebagai bahan evaluasi pada saat proses pengembangan  perangkat lunak maupun di akhir pengembangannya. Dengan adanya dokumen SKPL ini diharapkan pengembangan perangkat lunak akan lebih terarah dan lebih terfokus serta tidak menimbulkan ambiguitas terutama bagi pengembang perangkat lunak Penjualan Aksesoris dan Sparepart Handphone.
	</ol><br>
<b>1.2	Lingkup Masalah<br></b>
	<ol>Perangkat lunak yang akan dikembangkan adalah perangkat lunak Penjualan Aksesoris dan Sparepart Handphone, yaitu merupakan perangkat lunak yang digunakan untuk mempermudah proses administrasi dan penjualan Aksesoris dan Sparepart Handphone.<br>
	Aplikasi Aksesoris dan Sparepart Handphone ini dapat melakukan hal-hal berikut ini : <br>
		<ol>
		1.2.1 Fasilitas Login untuk admin, dan karyawan/kasir untuk menghindari penyalahgunaan hak akses.<br>
		1.2.2 Menampilkan daftar Aksesoris dan Sparepart Handphone yang tersedia.<br>
		1.2.3 Melayani penjualan Aksesoris dan Sparepart Handphone secara onlineberbasis web dan wap, dan  juga  transaksi dapat dilakukan dari manapun dan kapanpun.<br>
		1.2.4 Admin dan karyawan dapat melihat rekapitulasi hasil penjualan Dengan adanya Aplikasi ini.<br>
		</ol>
	</ol><br>
<b>1.3	Definisi, Akronim dan Singkatan</b>
   <ol>Istilah, Akronim dan Singkatan beserta Keterangannya : <br>
	 	<ol>
	 	1. Admin Merupakan seseorang yang bertanggungjawab untuk perawatan sistem dan  serta bertanggungjawab terhadap operasional sistem.<br>
	 	2. User merupakan Karyawan/kasir.<br>
	 	3. Pembeli Merupakan orang yang akan membeli. <br>
	 	4. web adalah halaman informasi yang disediakan melalui jalur internet sehingga bisa diakses di seluruh dunia selama terkoneksi dengan internet.<br>
	 	5. wap adalah standar internasional terbuka untuk aplikasi yang menggunakan komunikasi nirkabel. Tujuan utamanya untuk membangun aplikasi yang dapat mengakses internet dari telepon genggam atau PDA.<br>
	 	6. Transaction report merupakan Laporan rekapitulasi transaksi per satu transaksi.<br>
	 	7. Monthly report merupakan Laporan rekapitulasi transaksi per satu bulan.<br>
	 	</ol>
 </ol></br>
<b>1.4	Referensi</b><br>
	<ol>Dokumen-dokumen yang digunakan sebagai referensi dalam pembuatan SKPL ini adalah sebagai berikut: <br>
		<ol>
	    1.4.1 DOKUMEN1: menjelaskan tentang database system dan database pelanggan.<br> 
	    1.4.2 DOKUMEN2: daftar barang, deskripsi barang, Jumlah barang.<br>
	    1.4.3 DOKUMEN3: format keluhan standar.<br>
		</ol>
    </ol><br>
<b>1.5	Deskripsi Umum Dokumen</b><br>
	<ol>Dokumen ini secara garis besar terdiri dari tiga bab dengan perincian sebagai berikut: <br>
		<ol>
		1.5.1 Bab 1 Pendahuluan, merupakan pengantar dokumen  SKPL yang brisi tujuan penulisan dokumen, lingkup masalah pengembangan perangkat lunak, juga memuat definisi, akronim dan istilah yang digunakan  serta deskripsi umum dokumen yang merupakan ikhtisar dokumen SKPL.<br>
		1.5.2 Bab 2 Deskripsi Global Perangkat Lunak, mendefinisikan perspektif produk perangkat lunak serta asumsi dan ketergantungan yang digunakan dalam pengembangan aplikasi penjualan Aksesoris dan Sparepart Handphone.<br>
		</ol>
	</ol>
</ol><br>
 <b><li>Gambaran Umum</li><br></b>
<ol>
	<b>2.1 Perspektif produk</b> 
	<ol>Produk ini akan dijalankan oleh admin, pemilik, pegawai dan user yang
	memiliki koneksi ke internet. Penggunaan sistem terbagi tiga yaitu antar
	muka untuk user individu, antar muka untuk admin, dan antar muka untuk
	Pegawai. Produk ini dapat berjalan pada platform atau sistem operasi 
	apa saja yang mendukung aplikasi berbasis web.<br> 
		<ol>
		2.1.1 Antarmuka sistem  
			  <ol>Dalam penggunaan, pengguna berinteraksi langsung dengan aplikasi melalui PC / Laptop.</ol>
		2.1.2 Antarmuka pengguna 
			  <ol>Perangkat lunak untuk aplikasi ini dibuat dengan menggunkan aplikasi flash.Dimana tampilan didesain dengan menggunakan template yang ada. Perangkat lunak untuk layanan dalam Aplikasi ini dilengkapi dengan menu untuk pengaksesan berbagai fungsi yang disediakan.</ol>
		2.1.3 Antarmuka perangkat keras
			  <ol>
			  Perangkat keras yang dapat digunakan dalam perangkat lunak yang dibuat:<br>
				1.	PC<br>
				2.	Monitor VGA mempunyai resolusi minimal 8800 x 1200 pixel.<br>
				3.	Keyboard dan mouse untuk kegiatan user.<br>
				4.	Semua perangkat keras yang digunakan merupakan perangkat standar dalam sistem komputer.
			</ol>
		2.1.4 Antarmuka perangkat lunak
			  <ol>Perangkat lunak yang dibutuhkan untuk perpustakaan antara lain:<br>
				1. Sistem Operasi Windows (XP,Vista,7,Server 2008) dll<br>
				2. Untuk pengolahan database : MYSQL<br>
				3. ntuk koneksi Database digunakan XAMPP
			</ol>
		2.1.5 Antarmuka komunikasi
			  <ol>
			  Proses komunikasi dalam sistem ini menggunakan jaringan lokal, dimana dikontrol oleh komputer server.
			  </ol>
		2.1.6 Batasan-batasan memori
			  <ol>Perangkat lunak hanya dijalankan di Windows (XP,vista, 7, 8, server 2008 dll).
			  Waktu pengembangan perangkat lunak yang singkat membuat adanya kemungkinan tidak semua fungsi yang ada dapat dilaksanakan. Pengembangan perangkat lunak tidak akan merubah file-file ataupun database yang ada pada saat ini tanpa adanya user.</ol>
		2.1.7 Operasi-operasi
			  <ol>Perangkat lunak dapat dijalankan di PC atau Laptop manapun.</ol>
		2.1.8 Kebutuhan-kebutuhan dalam tahapan adaptasi
		</ol>
	</ol><br>
	<b>2.2 Fungsi-fungsi produk<br></b>
	<ol>Perangkat Lunak Sistem penjualan sparepart dan aksesoris online berbasis website responsife ini mempunyai beberapa fungsi utama, 
	antara lain: <br>
	<ol>
		1. Memudahkan proses jual beli barang.<br>
		2. Memudahkan user untuk menawarkan barang baru atau bekas yang dimiliki.<br>
		3. Menyediakan informasi mengenai data barang secara akurat.<br>
		4. Dapat memberikan penawaran khusus untuk user sesuai minat dan    kebutuhan user.<br>
		5. Memberikan alternatif pembayaran yang lebih banyak.<br></ol>
	</ol><br>
	<b>2.3 Karakteristik pengguna<br></b>
	<ol>
	Dalam sistem informasi ini, users yang terlibat adalah sebagai berikut:
		<ol>
		2.3.2 Pemilik
			  <ol>
			  Pemilik bisa memiliki banyak fungsi, sebagai pengelola stok barang,pengelola keuangan, Melihat Data Transaksi harian, dan pengelola sistem.
			  </ol>
		2.3.2 Admin
			  <ol>
			  Admin bisa memiliki banyak fungsi, sebagai pengelola stok barang,pengelola keuangan, pengelola user, dan pengelola sistem.
			  </ol>
		2.3.3 User Individu
			  <ol>
			  User Individu memiliki hak akses ke katalog yang disediakan
			  admin dan hak akses katalog yang dimiliki User Pegawai. User
			  Individu dapat memilih barang dan membeli barang. 
			  </ol>
		2.3.4 Pegawai
		      <ol>
			  Pegawai mendapat suatu halaman dinamis dan halaman
			  administrasi untuk mengelola katalog barang yang dimiliki, dan
			  mengelola Pembelian terhadap barang yang dimilikinya oleh User Individu
			  </ol>
		</ol>
	</ol><br>
	<b>2.4 Batasan-batasan<br></b>
		<ol>
		1. Untuk masalah pembayaran ditangani oleh pihak ketiga seperti,
		   perusahaan kartu kredit, paypal dan bank.<br>
		2. User yang berhak untuk mengakses sistem ini antara lain adalah admin,
		   user individu,pegawai dan pemilik.<br>
		</ol>