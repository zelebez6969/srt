Cara penggunaan:
1. Simpan script sebagai `srt_translator.py`
2. Install dependensi yang diperlukan:
```bash
pip install googletrans==4.0.0-rc1
```
3. Jalankan script melalui command line:
```bash
python srt_translator.py -i input.srt -o output.srt -d id
```

Penjelasan parameter:
- `-i/--input`: File SRT input yang akan diterjemahkan
- `-o/--output`: File SRT hasil terjemahan
- `-d/--dest`: Kode bahasa target (default: 'en' untuk Inggris)
- `-e/--encoding`: Encoding file (default: 'utf-8')

Fitur:
1. Mempertahankan format waktu dan urutan subtitle
2. Menangani multi-line text dalam subtitle
3. Mempertahankan formatting asli (italic, bold, dll) selama ada di teks
4. Error handling dasar untuk proses terjemahan

Catatan:
1. Google Translate API memiliki limitasi penggunaan, mungkin tidak bekerja untuk file yang sangat besar
2. Hasil terjemahan mungkin tidak sempurna, disarankan untuk melakukan proofreading setelah terjemahan
3. Untuk bahasa sumber (source language), script akan mendeteksi otomatis

Untuk daftar kode bahasa yang tersedia, bisa merujuk ke:
https://py-googletrans.readthedocs.io/en/latest/#googletrans-languages

Beberapa contoh kode bahasa populer:
- id: Indonesia
- en: Inggris
- es: Spanyol
- fr: Prancis
- ja: Jepang
- ko: Korea
- zh-cn: Mandarin (Simplified)
