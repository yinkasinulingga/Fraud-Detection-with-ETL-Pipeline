
---

# **Fraud Detection with ETL Pipeline**  

## **Deskripsi Proyek**  
Proyek ini mengembangkan sistem **deteksi fraud berbasis ETL dan Machine Learning** untuk mengidentifikasi transaksi mencurigakan secara otomatis. Menggunakan **Apache Airflow**, pipeline ini mengekstrak data transaksi dari database, melakukan transformasi dan validasi, kemudian menerapkan model Machine Learning untuk mendeteksi aktivitas penipuan. Jika ditemukan transaksi mencurigakan, sistem akan mengirimkan notifikasi email untuk investigasi lebih lanjut.  

## **Alur Proses ETL**  
1. **Extract**: Mengambil data transaksi dari PostgreSQL menggunakan Airflow.  
2. **Load**: Menyimpan data yang telah diproses ke database untuk analisis lebih lanjut.  
3. **Predict**: Menggunakan model Machine Learning untuk mengklasifikasikan transaksi sebagai fraud atau non-fraud.  
4. **Alert**: Jika ditemukan fraud, sistem mengirimkan notifikasi email kepada tim terkait.  

## **Teknologi yang Digunakan**  
- **Orkestrasi ETL**: Apache Airflow  
- **Database**: PostgreSQL  
- **Pemrograman**: Python, Pandas, NumPy  
- **Machine Learning**: Scikit-learn, XGBoost, Random Forest, Isolation Forest  
- **Deployment**: Pickle (model serialization), JSON  
- **Automasi & Notifikasi**: EmailOperator (Airflow)  

## **Struktur File**  
`Fraud_DAG.py` → Skrip DAG Airflow untuk pipeline ETL dan prediksi fraud  
`Modeling.ipynb` → Eksplorasi dan pemrosesan data transaksi  
`model.pkl` → Model Machine Learning yang digunakan untuk prediksi  

## **Cara Menjalankan Proyek**  
1. **Jalankan Apache Airflow** dan pastikan PostgreSQL sudah terkoneksi.  
2. **Tambahkan DAG ke dalam Airflow** dengan menyimpan `Fraud_DAG.py` di folder DAG.  
3. **Aktifkan DAG** melalui UI Airflow untuk memproses data dan melakukan prediksi.  
4. **Periksa email notifikasi** jika terdapat transaksi yang terdeteksi sebagai fraud.  

## Kontak  
Jika ada pertanyaan atau saran terkait proyek ini, silakan hubungi **Saya** di Email : yinkasinulingga@gmail.com  

---

