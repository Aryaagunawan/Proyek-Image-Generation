# Text-to-Image Generation (Stable Diffusion)

## 📖 Deskripsi Proyek
Proyek ini merupakan *submission* untuk program BFGAI yang berfokus pada pengembangan dan implementasi model Generative AI. Proyek ini mengimplementasikan model **Text-to-Image** menggunakan pustaka Hugging Face `diffusers` dan model dasar `runwayml/stable-diffusion-v1-5`. 

Selain itu, proyek ini juga dilengkapi dengan antarmuka web interaktif yang dibangun menggunakan **Streamlit** untuk memudahkan pengguna dalam berinteraksi dengan model secara langsung. Antarmuka ini dirancang agar dapat diakses secara publik melalui Google Colab menggunakan fitur *tunneling* dari **Ngrok**.

## ✨ Fitur Utama
1. **Text-to-Image Generation:** Menghasilkan gambar beresolusi tinggi (512x512) dari instruksi teks (prompt) menggunakan model Stable Diffusion v1.5 dengan optimasi `DPMSolverMultistepScheduler`.
2. **Interactive UI:** Web interface interaktif yang dibangun menggunakan Streamlit.
3. **Public Deployment:** Integrasi dengan Ngrok untuk mengekspos port aplikasi lokal dari Google Colab menjadi URL publik yang dapat diakses di mana saja.

## 🛠️ Teknologi & Dependensi
Proyek ini memanfaatkan berbagai *library* dan *framework*, antara lain:
- **Bahasa Pemrograman:** Python
- **AI / ML Framework:** PyTorch, Hugging Face `diffusers`, `transformers`
- **Web Framework:** Streamlit
- **Computer Vision & Visualisasi:** OpenCV (`opencv-python`), Pillow (`PIL`), Matplotlib
- **Deployment / Tunneling:** Ngrok
- **Optimasi & Utilitas:** `accelerate`, `safetensors`, `xformers` (opsional untuk efisiensi memori)

## 🚀 Cara Menjalankan Proyek

### 1. Uji Coba Model Pipeline (Eksplorasi)
1. Unggah dan buka file `Pipeline_submission_BFGAI_ARYA GUNAWAN.ipynb` di **Google Colab**.
2. Ubah tipe Runtime ke **GPU** (direkomendasikan menggunakan *Tesla T4*).
3. Jalankan sel-sel awal untuk melakukan instalasi dependensi.
4. Ikuti instruksi yang ada di dalam notebook untuk memuat *Base Pipeline Model* dan uji coba melakukan inferensi teks ke gambar.

### 2. Menjalankan Antarmuka Web (Streamlit)
1. Unggah file `Streamlit_submission_BFGAI_ARYA GUNAWAN.ipynb` beserta file `app.py` dan `logic.py` ke dalam *file explorer* di Google Colab.
2. Buka notebook tersebut dan pastikan Anda sudah melengkapi logika kode yang rumpang pada `logic.py`.
3. Jalankan sel persiapan untuk setup Streamlit dan Ngrok.
4. Saat menjalankan sel koneksi Ngrok, sebuah *Public URL* akan muncul di output (misalnya `https://xxxx.ngrok-free.app`). 
5. Klik URL tersebut untuk membuka aplikasi web Streamlit Anda.
