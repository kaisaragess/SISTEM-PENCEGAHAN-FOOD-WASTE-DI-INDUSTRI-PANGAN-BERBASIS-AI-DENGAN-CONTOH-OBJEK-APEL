SISTEM PENCEGAHAN FOOD WASTE DI INDUSTRI PANGAN BERBASIS AI DENGAN CONTOH OBJEK APEL

![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Roboflow](https://img.shields.io/badge/Roboflow-101010?style=for-the-badge&logo=roboflow&logoColor=white)

Aplikasi *mobile* cerdas yang dirancang untuk mendeteksi tingkat kematangan buah apel menggunakan kamera *smartphone*.

Proyek ini dibangun untuk mendukung inisiatif **SDG 2: Zero Hunger** dan mengurangi angka *food waste* di Indonesia dengan membantu konsumen dan pedagang memilah buah yang masih layak konsumsi atau yang harus segera diolah.

---

## 📸 Layout UI/UX & Alur Aplikasi

*(Catatan: Ganti placeholder ini dengan screenshot asli aplikasimu)*

| 1. Prediksi Apel Mentah | 2. Prediksi Apel Matang  | 3. Prediksi Apel Busuk |
| :---: | :---: | :---: |
| <img width="714" height="1599" alt="WhatsApp Image 2026-06-19 at 15 25 58" src="https://github.com/user-attachments/assets/54495b62-5754-4f7d-ae28-4b0aac3d93c5" />
 | <img width="714" height="1599" alt="WhatsApp Image 2026-06-19 at 15 25 58 (1)" src="https://github.com/user-attachments/assets/c9a9605c-478b-4bd8-b2d5-a9f7d4af5502" />
 | <img width="714" height="1599" alt="WhatsApp Image 2026-06-19 at 15 25 58 (2)" src="https://github.com/user-attachments/assets/a0513910-d537-4ebc-8742-a972e8c536ed" />
 |
| Penjelasan misi *Zero Hunger* dan tombol mulai scan. | *Bounding box* mendeteksi apel secara *real-time*. | Menampilkan status (Mentah, Matang, Busuk) & persentase akurasi. |

---

## 🛠️ Arsitektur & Teknologi

Aplikasi ini dipisahkan menjadi *client-side* dan *server-side* untuk memastikan inferensi AI berjalan cepat dan ringan di *mobile*:

* **Frontend:** Flutter (Dart) - Mengambil gambar dan merender UI.
* **Backend API:** FastAPI (Python) - Menangani *request* gambar dan melakukan inferensi.
* **AI / Computer Vision:** Model deteksi objek (dilatih menggunakan dataset *custom* via Roboflow).
* **Database (Opsional):** MongoDB - Untuk menyimpan riwayat *scan* pengguna.

## 🚀 Cara Instalasi & Menjalankan Aplikasi

### Opsi 1: Instalasi Langsung (APK)
Bagi pengguna yang hanya ingin mencoba aplikasi, silakan unduh versi *compiled* terbaru:
👉 **LinkDrive**

### Opsi 2: Build dari Source Code (Untuk Developer)

**1. Clone Repositori:**
```bash
git clone 
