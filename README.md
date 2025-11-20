# 🎧 Spotify Chart Insights

Sebuah proyek eksplorasi data harian **Top 50 Lagu Global Spotify** dari tahun 2023–2024. Proyek ini bertujuan untuk memahami tren musik, pola popularitas, dan dinamika chart Spotify menggunakan data streaming harian.

## 📊 Dataset
Data mencakup:
- **Tanggal pencatatan**
- **Peringkat (1–50)**
- **Judul lagu & artis**
- **Skor popularitas Spotify (0–100)**
- **Jumlah stream harian (perkiraan)**
- **Tipe rilis** (single/album)
- **Durasi lagu**
- **Tanggal rilis asli**
- **Label eksplisit** (`True`/`False`)
- **URL sampul album**

> ⚠️ Catatan: Data berasal dari sumber pihak ketiga dan mungkin mengandung perkiraan atau kesalahan minor.

## Pertanyaan Eksploratif
Beberapa pertanyaan yang dijawab dalam analisis ini:
- Apakah lagu dengan popularitas tinggi selalu berada di puncak chart?
- Siapa artis yang paling sering masuk Top 50?
- Apakah lagu lama masih bisa bertahan di chart?
- Bagaimana pola musiman (misalnya lagu Natal)?
- Apa ciri khas lagu yang sedang *viral*?

## Struktur Proyek
```
spotify-chart-insights/
├── data/
│   └── spotify-streaming-top-50-world.csv  # Dataset mentah
├── spotify_analysis.ipynb   # Analisis eksploratif (Python + Pandas + Matplotlib/Seaborn)
├── README.md
└── requirements.txt
```

## Teknologi yang Digunakan
- **Python** (versi ≥3.8)
- **Pandas** – manipulasi dan pembersihan data
- **Matplotlib / Seaborn** – visualisasi data
- **Jupyter Notebook** – eksplorasi interaktif

## Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone https://github.com/MuhammadPrayoga/spotify-chart-insights.git
   cd spotify-chart-insights
   ```
2. (Opsional) Buat environment virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   # atau
   venv\Scripts\activate     # Windows
   ```
3. Install dependensi:
   ```bash
   pip install -r requirements.txt
   ```
4. Buka notebook:
   ```bash
   jupyter notebook spotify_analysis.ipynb
   ```

---

## 💡 Insight Utama (Preview)
> **Popularitas ≠ Posisi Chart**  
> Skor popularitas Spotify mencerminkan daya tahan dan basis penggemar jangka panjang, sedangkan posisi chart harian didorong oleh **jumlah stream harian**. Karena itu, lagu baru bisa langsung #1 meski popularitasnya belum 100, sementara lagu lama seperti *"Cruel Summer"* (2019) tetap relevan bertahun-tahun kemudian.

