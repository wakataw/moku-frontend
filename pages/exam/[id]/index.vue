<template>
  <div class="mx-auto w-full flex-1 flex justify-center">
    <div class="w-1/2 m-8 ml-4 border rounded-md bg-white shadow-md overflow-auto">
      <div class="p-4 border-b bg-[url('~/assets/images/blue-abstract.svg')] text-white font-semibold sticky top-0 bg-cover text-center">Deskripsi dan Ketentuan</div>
      <div class="p-8 space-y-6 items-start">
        <div class="space-y-4">
          <h2 class="text-2xl font-semibold underline decoration-yellow-400 decoration-4">Jadwal & Waktu</h2>
          <table class="[&_tr>th]:text-left [&_tr>th]:font-semibold [&_tr>th]:pr-4 [&_tr>*]:py-1">
            <tr>
              <th>Mulai</th>
              <td>7 Desember 2022 10:33</td>
            </tr>
            <tr>
              <th>Selesai</th>
              <td>7 Desember 2022 11:33</td>
            </tr>
            <tr>
              <th>Durasi</th>
              <td>60 menit</td>
            </tr>
            <tr>
              <th>Jumlah Soal</th>
              <td>90 soal</td>
            </tr>
            <tr>
              <th>Kesempatan</th>
              <td>1 kali</td>
            </tr>
          </table>
        </div>
        <div class="space-y-4">
          <h2 class="text-2xl font-semibold underline decoration-yellow-400 decoration-4">Ketentuan Pelaksanaan</h2>
          <ol class="list-decimal p-4">
            <li>Kesempatan yang diberikan untuk menyelesaikan uji kompetensi ini hanya 1 (satu) kali;</li>
            <li>Batas waktu maksimal pengerjaan soal adalah 60 menit;</li>
            <li>Dalam pengerjaan soal ini jawaban benar mendapat nilai +1, sedangkan jawaban salah dan tidak menjawab mendapat nilai 0.</li>
            <li>Jika memilih untuk tidak menjawab, pastikan untuk tidak mengklik pilihan jawaban dikarenakan pilihan jawaban tidak dapat dihapus, tetapi pilihan jawaban masih dapat diubah selama belum melakukan klik "Submit All and Finish";</li>
            <li>Pastikan telah menekan tombol "Submit All and Finish" setelah selesai mengerjakan soal;</li>
            <li>Dengan menekan tombol klik "Attempt quiz now" dengan ini saya menyatakan telah membaca dan akan mematuhi tata tertib peserta assessment;</li>
            <li>Peserta dilarang menggunakan Kalkulator/Handphone/Microsoft Excel dalam melakukan perhitungan.</li>
            <li>Setelah selesai mengerjakan soal pilihan ganda, harap mengisi formulir Critical Incident dan Self Assesment yang telah dikirim ke e-mail pajak peserta</li>
          </ol>
        </div>
        <div>
          <NuxtLink :to="`/exam/${route.params.id}/answers`" class="bg-emerald-500 text-emerald-50 font-semibold text-xl py-2 px-4 rounded-md">
            Mulai Ujian
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  definePageMeta({
    layout: "exam"
  });

  const route = useRoute();
</script>

<style scoped>

</style>