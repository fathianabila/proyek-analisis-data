# Proyek Analisis Data: Bike Sharing Dataset

Analisis data penyewaan sepeda Capital Bikeshare (Washington D.C.) tahun 2011-2012 untuk menjawab dua pertanyaan bisnis:

1. Berapa persentase pengguna casual pada hari kerja dibandingkan hari libur/akhir pekan, dan berapa rata-rata penyewaan harian casual dan registered pada masing-masing kelompok hari?
2. Musim apa yang memiliki rata-rata penyewaan harian tertinggi dan terendah, dan berapa persen pertumbuhannya dari 2011 ke 2012 pada tiap musim?

Dataset yang dipakai: `day.csv` (data harian). Berkas `hour.csv` tidak dipakai karena kedua pertanyaan cukup dijawab dengan data harian.

## Struktur Folder
```
submission
├── dashboard
│   ├── main_data.csv
│   └── dashboard.py
├── data
│   └── day.csv
├── notebook.ipynb
├── README.md
├── requirements.txt
└── url.txt
```

## Setup Environment
```
python -m venv venv
venv\Scripts\activate        # Windows (macOS/Linux: source venv/bin/activate)
pip install -r requirements.txt
```

## Menjalankan Notebook
Buka `notebook.ipynb` dari folder utama (`submission`) agar path `data/day.csv` terbaca, lalu jalankan semua sel (Run All).

## Menjalankan Dashboard
Jalankan dari folder utama (`submission`):
```
streamlit run dashboard/dashboard.py
```
Jika perintah `streamlit` tidak dikenali, gunakan:
```
python -m streamlit run dashboard/dashboard.py
```
Dashboard dapat dibuka di `http://localhost:8501`.
