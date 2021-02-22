function piketmj() {
  var token = '1231278846:AAHBdL8QkHHFQupdQvTplRjQIfm8tFiPU2E';
  var tg = new telegram.daftar(token);
  var chatid = -498115106; // ID Telegram tujuan remindernya
  
  var now = new Date();
  var waktu = Utilities.formatDate(now, 'Asia/Jakarta', 'HH:mm:ss');
  var teks = "🗣Pengingat Piket MJ !!"
  
  teks = teks + "\n\nbot pengingat piket harian";
  teks = teks + "\n Menyapu = Syahrul";
  teks = teks + "\n Mengepel = Riyan  ";
  teks = teks + "\n Membersihkan teras dan outlet = Erfa";
  teks = teks + "\n Desinfektan = Iqbal";
  teks = teks + "\n Membersihkan sampah dan got = Idham  ";
  teks = teks + "\n Menata dokumen dan peralatan publik = Zuli  ";
  teks = teks + "\n Masak nasi, bersih area dapur dan cuci = Irfan";
  teks = teks + "\noiya , ini untuk menampilkan jam ya ,  ⏱ `" + waktu + "` ";
  
  teks = teks + "\n\nSemangat :) ";
  teks = teks + "\nTerima kasih telah menjaga sekre tercinta, Semoga senantiasa dilimpahkan keberkahan  ";
  
  var ret = tg.kirimPesan(chatid, teks, 'markdown');
  Logger.log(ret); // simpan hasil return kirimPesan ke log
}
