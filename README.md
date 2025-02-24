---

# **Fraud Detection with ETL Pipeline**  

## **Deskripsi Proyek**  
Proyek ini mengembangkan sistem **deteksi fraud berbasis ETL dan Machine Learning** untuk mengidentifikasi transaksi mencurigakan secara otomatis. Menggunakan **Apache Airflow**, pipeline ini mengekstrak data transaksi dari database, memprosesnya, kemudian menerapkan model Machine Learning untuk mendeteksi aktivitas penipuan. Jika ditemukan transaksi mencurigakan, sistem akan mengirimkan notifikasi email kepada tim terkait untuk investigasi lebih lanjut.  

## **Alur Proses ETL**  
1. **Extract** → Mengambil data transaksi dari PostgreSQL menggunakan Airflow.  
2. **Load** → Menyimpan data ke dalam database setelah diproses.  
3. **Predict** → Menggunakan model Machine Learning untuk mengklasifikasikan transaksi sebagai fraud atau non-fraud.  
4. **Alert** → Jika ditemukan transaksi mencurigakan, sistem mengirimkan notifikasi email ke tim terkait.  

## **Teknologi yang Digunakan**  
- **Orkestrasi ETL**: Apache Airflow  
- **Database**: PostgreSQL  
- **Pemrograman**: Python, Pandas, NumPy  
- **Machine Learning**: Scikit-learn, XGBoost, Random Forest, Isolation Forest  
- **Deployment**: Pickle (model serialization), JSON  
- **Automasi & Notifikasi**: EmailOperator (Airflow)  

## **Struktur File**  
- `Fraud_DAG.py` → Skrip DAG Airflow untuk pipeline ETL dan prediksi fraud  
- `Modeling.ipynb` → Eksplorasi dan pemrosesan data transaksi  
- `model.pkl` → Model Machine Learning yang digunakan untuk prediksi  

## **Kesimpulan dan Rekomendasi**  
- **Automasi deteksi fraud meningkatkan efisiensi** → Dengan implementasi Apache Airflow, proses deteksi transaksi mencurigakan dapat dilakukan secara otomatis tanpa intervensi manual.  
- **Notifikasi real-time membantu tim dalam investigasi** → Sistem yang mengirimkan peringatan otomatis memastikan tindakan pencegahan dapat segera diambil untuk mengurangi potensi kerugian akibat penipuan.  
- **Peningkatan akurasi model** → Dengan data yang bersih dan pipeline yang optimal, model dapat lebih akurat dalam mengidentifikasi pola transaksi fraud.  
- **Pengembangan lebih lanjut** → Integrasi dengan dashboard visualisasi (Tableau atau Kibana) dapat memberikan insight lebih mendalam terhadap tren transaksi yang mencurigakan.  

## **Dampak Bisnis**  
- **Mengurangi kerugian akibat penipuan** → Dengan deteksi lebih cepat dan akurat, perusahaan dapat mengurangi transaksi fraud yang berpotensi merugikan finansial.  
- **Meningkatkan kepercayaan pelanggan** → Sistem keamanan yang kuat membuat pelanggan lebih percaya untuk bertransaksi di platform.  
- **Optimasi sumber daya tim keamanan** → Dengan otomatisasi deteksi fraud, tim dapat lebih fokus pada investigasi kasus yang lebih kompleks daripada memproses transaksi secara manual.  
- **Meningkatkan kepatuhan terhadap regulasi** → Sistem deteksi fraud membantu perusahaan dalam memenuhi persyaratan keamanan finansial dan audit transaksi yang lebih transparan.  

## **Cara Menjalankan Proyek**  
1. **Jalankan Apache Airflow** dan pastikan PostgreSQL sudah terkoneksi.  
2. **Tambahkan DAG ke dalam Airflow** dengan menyimpan `Fraud_DAG.py` di folder DAG.  
3. **Aktifkan DAG** melalui UI Airflow untuk memproses data dan melakukan prediksi.  
4. **Periksa email notifikasi** jika terdapat transaksi yang terdeteksi sebagai fraud.  

## **Kontak**  
Jika ada pertanyaan atau saran terkait proyek ini, silakan hubungi:  
**Email**: yinkasinulingga@gmail.com  

---
