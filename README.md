# Informerd_Search

Untuk tugas Praktikum ke 3

# Penjellasan

1. Greedy Best First Search
   Kode di atas adalah implementasi algoritma Greedy Best-First Search (GBFS), yang digunakan untuk mencari jalur dari simpul awal ke simpul tujuan dalam sebuah graf. Algoritma ini memilih simpul berdasarkan nilai heuristiknya, yaitu perkiraan jarak ke tujuan tanpa mempertimbangkan biaya sebenarnya.

Prosesnya dimulai dengan memasukkan simpul awal ke dalam Priority Queue, lalu terus mengeksplorasi simpul dengan nilai heuristik terkecil. Jika simpul tujuan ditemukan, maka jalur menuju tujuan akan direkonstruksi menggunakan dictionary came_from, yang menyimpan dari mana setiap simpul berasal. Jika simpul tujuan tidak ditemukan setelah semua kemungkinan dicoba, maka algoritma akan mengembalikan bahwa pencarian gagal.

Perbedaannya dengan A Search\* adalah bahwa Greedy Best-First Search hanya mempertimbangkan heuristik tanpa memperhitungkan biaya perjalanan yang telah ditempuh, sehingga sering kali lebih cepat tetapi tidak selalu menemukan jalur terpendek.

2. A Star Search
   Kode di atas adalah implementasi algoritma A* Search, yang digunakan untuk mencari jalur terpendek dari titik awal ke tujuan dalam sebuah graf berbobot. Algoritma ini bekerja dengan menggunakan Priority Queue untuk menentukan simpul (node) mana yang akan dieksplorasi berdasarkan total biaya perjalanan sejauh ini dan perkiraan biaya menuju tujuan (heuristik). Setiap kali algoritma mengambil simpul dengan prioritas tertinggi, ia memeriksa apakah simpul tersebut adalah tujuan. Jika ya, maka jalur yang ditempuh dan total biaya akan ditampilkan. Jika belum, algoritma akan mengeksplorasi semua tetangga dari simpul tersebut, menghitung total biaya baru, dan memasukkan jalur yang diperbarui ke dalam antrean untuk diperiksa lebih lanjut. Dengan pendekatan ini, A* Search dapat menemukan jalur terpendek secara efisien dengan mempertimbangkan baik biaya aktual maupun estimasi ke tujuan.
