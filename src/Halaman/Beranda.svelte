<script>
  import Gerbang from "../library/kunci-terbaru/src/Gerbang.svelte";

  let angka = 0;
  // Fungsi untuk mengambil angka acak antara 1 dan 604
  function getRandomNumber() {
    // Menggunakan Math.random() untuk mendapatkan nilai acak antara 0 (inklusif) dan 1 (eksklusif)
    // Kemudian dikalikan dengan 603 untuk mendapatkan rentang antara 0 dan 603
    // Setelah itu, ditambahkan 1 untuk memindahkan rentang ke 1 hingga 604
    return Math.floor(Math.random() * 604) + 1;
  }

  // Menggunakan fungsi untuk mendapatkan angka acak
  angka = getRandomNumber();

  // Menampilkan angka acak di konsol
  // console.log("Angka acak antara 1 dan 604:", angkaAcak);
</script>

<Gerbang namaAplikasi="Ngaji">
  <div class="p-5 min-h-screen flex justify-center items-center">
    <div class="text-5xl">{angka}</div>
  </div>
</Gerbang>
