## Membuat Aplikasi Lempar Dadu di Android Studio Menggunakan Jetpack Compose

#### Aplikasi yang dibuat kali ini memungkinkan pengguna untuk melempar dadu secara acak dengan tampilan yang menarik dan animasi yang responsif.

1️⃣ Buat Proyek → New Project → Pilih Empty Activity (Jetpack Compose)
2️⃣ Tampilan Dasar
- Buka MainActivity.kt dan ubah setContent {} agar memanggil DiceRollerApp()
- Tambahkan fungsi DiceRollerApp()
3️⃣ Modifikasi UI dengan Compose
- Buat fungsi DiceWithButtonAndImage()
- Gunakan Column, Button, Image, Text untuk UI, lalu tambahkan Modifier untuk spacing & styling
4️⃣ Import Gambar Dadu
- Import gambar dadu ke res/drawable melalui Resource Manager
- Gunakan Image(painterResource(id = R.drawable.dice_1), contentDescription = "Dice")
5️⃣ Logika Random Dice
- Buat var result by remember { mutableIntStateOf(1) }
- Gunakan when(result) {} untuk menampilkan gambar sesuai angka dadu
- Tambahkan aksi onClick pada Button → result = (1..6).random()
6️⃣ Menyimpan teks
- Buka res/values/strings.xml
- Tambahkan <string name="roll">Roll</string>
7️⃣ Jalankan Aplikasi
Klik Run (Shift + F10) dan coba tekan tombol Roll
🎲 Selesai! Aplikasi Dice Roller sudah berfungsi! 🚀


Tampilan Output
Ketika aplikasi dijalankan, tampilan yang dihasilkan adalah sebagai berikut:

![Screenshot_20250325_231801](https://github.com/user-attachments/assets/58e45a9d-9a3d-469f-a20f-dcd1be2f1953)

