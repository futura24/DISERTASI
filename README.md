# DISERTASI

# Portal Asesmen Diagnostik MCDM

Lima aplikasi asesmen statis (HTML5 + CSS3 + JavaScript murni, Chart.js) untuk penelitian
model diagnostik MCDM matematika SMP. Tanpa backend; data tersimpan di Local Storage dan
dapat diekspor ke JSON.

## Struktur
- `index.html` — portal/landing
- `asesmen-1-diagnostik-kognitif/` — Tes Diagnostik Kognitif (40 butir, mastery A1–A8)
- `asesmen-2-kecemasan-matematika/` — Skala Kecemasan Matematika (28 butir Likert, 4 dimensi)
- `asesmen-3-validasi-materi/` — Lembar Validasi Ahli Materi (CVR)
- `asesmen-4-validasi-psikometri/` — Lembar Validasi Ahli Psikometri (CVR, CVI)
- `asesmen-5-validasi-ai/` — Lembar Validasi Ahli AI/Data Mining (gauge, CVR, CVI)

## Hosting di GitHub Pages
1. Buat repository baru, unggah seluruh isi folder ini ke root.
2. Settings → Pages → Source: branch `main`, folder `/ (root)`.
3. Akses melalui URL yang diberikan; buka `index.html`.

## Catatan metodologis
- Kunci jawaban & pemetaan atribut (Q-matrix) sesuai instrumen MCDM.
- CVR Lawshe = (nₑ − N/2)/(N/2); pada lembar per-validator, N = jumlah indikator dan
  nₑ = jumlah indikator bertanda "Esensial".
- I-CVI/S-CVI: indikator dianggap relevan bila skor 4–5 (skala 1–5).
- Ekspor JSON tiap validator dapat diagregasi untuk CVR/CVI panel lengkap.
