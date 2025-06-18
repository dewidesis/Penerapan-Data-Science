# Proyek Akhir: Menyelesaikan Permasalahan Jaya Jaya Institut

## Business Understanding

Jaya Jaya Institut adalah lembaga pendidikan ternama yang telah berdiri sejak tahun 2000 dan dikenal luas karena menghasilkan lulusan berkualitas. Namun, saat ini institusi tersebut menghadapi tantangan besar berupa tingginya angka putus kuliah, yang berisiko menurunkan reputasi dan mengganggu efisiensi operasional. Dengan mendeteksi lebih awal siswa yang berisiko dropout, Jaya Jaya Institut dapat memberikan intervensi berupa bimbingan dan dukungan yang dibutuhkan, sehingga mampu meningkatkan tingkat kelulusan, menjaga reputasi institusi, dan mendorong kepuasan serta kesuksesan mahasiswa.

### Permasalahan Bisnis

Jaya Jaya Institut tengah menghadapi tantangan besar akibat tingginya angka mahasiswa yang mengundurkan diri sebelum lulus. Tingginya angka dropout ini tidak hanya berdampak negatif terhadap reputasi dan kondisi finansial institusi, tetapi juga merugikan mahasiswa yang tidak dapat menyelesaikan pendidikan mereka. Fenomena ini berisiko menurunkan tingkat kepercayaan calon mahasiswa beserta orang tua terhadap mutu pendidikan yang disediakan oleh Jaya Jaya Institut. Berikut ini adalah sejumlah permasalahan bisnis utama yang timbul akibat situasi tersebut:
1. **Reputasi Institusi**: Tingkat dropout yang tinggi dapat mencoreng citra institusi sebagai lembaga pendidikan yang kredibel dan berkualitas.
2. **Kehilangan Sumber Pendapatan**: Mahasiswa dropout menyebabkan institusi kehilangan potensi pendapatan dari biaya pendidikan dan sumber pendapatan lainnya.
3. **Dampak terhadap Akreditasi**: Rendahnya tingkat kelulusan dapat menjadi faktor yang menurunkan nilai akreditasi institusi secara keseluruhan.
4. **Kekecewaan Stakeholder**: Kepercayaan mahasiswa, orang tua, serta masyarakat luas terhadap kemampuan institusi dalam membina dan mendampingi mahasiswa hingga lulus dapat menurun.

### Cakupan Proyek

1. Mengumpulkan dan memproses data mahasiswa.
2. Menganalisis data untuk menemukan pola dan faktor-faktor yang mempengaruhi dropoutnya mahasiswa.
3. Membangun model prediktif menggunakan algoritma Random Forest Classifier.
4. Membuat dashboard bisnis untuk memvisualisasikan temuan dan prediksi.
5. Memberikan rekomendasi tindakan berdasarkan hasil analisis.

### Persiapan

Sumber data: https://github.com/dicodingacademy/dicoding_dataset/tree/main/students_performance

Setup environment:

Proyek ini dikembangkan menggunakan Python dan disarankan untuk dijalankan dalam lingkungan virtual (virtual environment) untuk mengelola dependensi secara terisolasi.
1.  **Membuat dan Mengaktifkan Virtual Environment (venv)**
    Buka terminal atau command prompt, lalu ikuti langkah-langkah berikut:
    ```bash
    # Membuat virtual environment baru bernama 'venv'
    python -m venv venv

    # Mengaktifkan virtual environment:
    # Untuk macOS/Linux:
    source venv/bin/activate
    # Untuk Windows (Command Prompt):
    venv\Scripts\activate.bat
    # Untuk Windows (PowerShell):
    venv\Scripts\Activate.ps1
    ```
    Setelah diaktifkan, akan terlihat `(venv)` di awal baris perintah yang menandakan bahwa sudah berada di lingkungan virtual.

2.  **Menginstal Dependensi dari `requirements.txt`**
    Pastikan  telah mengaktifkan virtual environment (langkah 1). Kemudian, install semua pustaka Python yang dibutuhkan dari berkas `requirements.txt` menggunakan pip:
    ```bash
    pip install -r requirements.txt
    ```
    Ini akan menginstal semua *library* yang diperlukan.

Dengan langkah-langkah di atas, Anda telah siap untuk memulai proyek dengan lingkungan yang bersih dan terisolasi.

3. Buka jupyter-notebook dengan menjalankan perintah berikut.
    ```
    jupyter-notebook
    ```

4. Buka file python `prediction.py`.

5. Jalankan Streamlit
   - Jalankan perintah `streamlit run app.py` di terminal atau command prompt, di mana `app.py` adalah nama file Python yang berisi kode Streamlit.
     ```bash
     streamlit run app.py
     ```
   - Deploy Aplikasi Streamlit
     Aplikasi Streamlit telah di-deploy dan dapat diakses melalui tautan berikut: https://penerapan-data-science-dewi.streamlit.app/

## Business Dashboard

Dashboard ini dibuat untuk memberikan pemahaman yang komprehensif terkait tingkat dropout mahasiswa. Melalui visualisasi metrik penting, tren, serta perbandingan berdasarkan berbagai faktor penyebab yang ditemukan dari hasil analisis, dashboard ini bertujuan mendukung institusi dalam menentukan fokus strategi yang tepat guna meningkatkan motivasi serta keberhasilan akademik mahasiswa.

URL: https://lookerstudio.google.com/reporting/8a3b91d8-a06c-4c9e-b634-9b6c7364d2b3

## Menjalankan Prototype Sistem Machine Learning

Untuk menjalankan aplikasi ini, Anda perlu mengikuti langkah-langkah berikut:

1. **Persyaratan Awal**:

   - Pastikan Anda telah menginstal Python di sistem Anda.
   - Instal Streamlit dan Pandas dengan menggunakan pip. Anda dapat melakukannya dengan menjalankan perintah berikut di terminal:
     ```bash
     pip install streamlit pandas
     ```

2. **Model yang Dilatih**:

   - Pastikan Anda memiliki model yang telah dilatih dan disimpan dalam format pickle (`model.pkl`). Model ini harus berada di direktori yang sama dengan berkas `app.py`.

3. **Menjalankan Aplikasi**:

   - Buka terminal dan navigasikan ke direktori tempat berkas `app.py` berada.
   - Jalankan aplikasi dengan perintah berikut:
     ```bash
     streamlit run app.py
     ```
   - Setelah menjalankan perintah tersebut, aplikasi akan terbuka di browser Anda secara otomatis. Jika tidak, Anda dapat mengaksesnya melalui alamat `http://localhost:8501`.

4. **Menggunakan Aplikasi**:

   - Setelah aplikasi terbuka, Anda akan melihat antarmuka untuk memasukkan data mahasiswa.
   - Isi kolom-kolom yang tersedia dengan informasi yang relevan.
   - Klik tombol "Prediksi" untuk mendapatkan hasil prediksi apakah mahasiswa tersebut berpotensi dropout atau tidak.

5. **Hasil Prediksi**:
   - Hasil prediksi akan ditampilkan di bawah tombol prediksi.

## Streamlit

Local URL: http://localhost:8501
Network URL: http://192.168.1.6:850
Link Deployment streamlit : https://penerapan-data-science-dewi.streamlit.app/

## Conclusion

Tingkat dropout mahasiswa di Jaya Jaya Institut dipengaruhi oleh beragam aspek yang mencakup karakteristik demografis, latar belakang pendidikan sebelumnya, kondisi ekonomi, situasi keluarga dan sosial, serta performa akademik.

1. **Tingkat Dropout Tinggi**: Dari total 4.424 mahasiswa, sekitar 32,1% di antaranya mengalami dropout, angka yang cukup signifikan dan memerlukan perhatian khusus dari pihak institusi.

2. **Faktor-Faktor Sosial Demografis**:
   - Jenis Kelamin: Mahasiswa perempuan lebih banyak mengalami dropout dibandingkan laki-laki.
   - Status Perkawinan: Dropout paling tinggi terjadi pada mahasiswa yang belum menikah (single).
   - Status Tempat Tinggal (Displaced): Mahasiswa yang tinggal jauh dari rumah (displaced) memiliki tingkat dropout lebih tinggi.
   - Penerima Beasiswa: Mahasiswa yang tidak menerima beasiswa memiliki tingkat dropout yang lebih tinggi.

3. **Waktu Perkuliahan**: Mahasiswa program daytime (kelas pagi/siang) memiliki angka dropout yang jauh lebih tinggi dibandingkan program evening.

4. **Faktor Akademik**: Mahasiswa dengan nilai rata-rata masuk sebesar 126,64 dan usia masuk rata-rata 23,27 tahun menunjukkan bahwa dropout bukan hanya masalah akademik, tetapi bisa dipengaruhi oleh faktor lain seperti motivasi atau tekanan sosial.

5. **Mode Pendaftaran dan Jenis Kursus**: Beberapa jalur masuk dan jurusan tertentu seperti Nursing dan Social Service menunjukkan tingkat dropout yang tinggi.

6. **Latar Belakang Orang Tua**: Mahasiswa dengan orang tua (baik ayah maupun ibu) yang memiliki pendidikan dan pekerjaan di kategori rendah (misalnya tidak bekerja atau hanya tamatan pendidikan dasar) cenderung memiliki angka dropout lebih tinggi.

7. **GDP**: Dropout lebih tinggi terjadi pada mahasiswa dengan tingkat GDP yang lebih rendah.

### Rekomendasi Action Items (Optional)

1. Berikut sejumlah strategi yang dapat diterapkan oleh Jaya Jaya Institut untuk menurunkan angka mahasiswa yang tidak menyelesaikan studi:
2. Berikan dukungan akademik tambahan, seperti kelas pendamping dan bimbingan belajar, khususnya bagi mahasiswa di program manajemen malam hari dan teknik informatika yang menunjukkan tingkat dropout tinggi.
3. Laksanakan program remedial guna membantu mahasiswa dengan nilai masuk rendah agar dapat mengejar ketertinggalan dan memperbaiki performa akademik mereka.
4. Perluas cakupan beasiswa bagi mahasiswa yang memiliki risiko tinggi mengalami dropout, serta sediakan informasi yang lebih jelas dan mudah diakses mengenai opsi bantuan keuangan.
5. Tingkatkan layanan konseling dan dukungan psikologis, terutama bagi mahasiswa yang berasal dari keluarga dengan latar belakang pendidikan orang tua yang rendah atau tidak tercatat.
6. Rancang program bantuan khusus bagi mahasiswa dari keluarga dengan latar belakang pekerjaan orang tua yang secara sosial atau ekonomi kurang mendukung kelangsungan studi.
7. Terapkan sistem pemantauan akademik secara rutin, sehingga institusi dapat melakukan tindakan preventif lebih awal terhadap mahasiswa yang mengalami penurunan prestasi.
8. Tingkatkan kualitas fasilitas kampus, seperti perpustakaan, ruang belajar, dan layanan mahasiswa, guna menciptakan suasana belajar yang lebih nyaman dan mendukung.
9. Dorong partisipasi mahasiswa dalam kegiatan yang mendukung keseimbangan hidup, seperti program ekstrakurikuler dan layanan kesehatan mental, untuk menjaga kesehatan fisik dan emosional mereka.
10. Bangun komunikasi aktif dengan orang tua, melalui program sosialisasi dan pelibatan keluarga, agar mereka dapat lebih mendukung proses pendidikan anak-anak mereka.
