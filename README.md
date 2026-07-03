# TinyGPT

Implementasi sederhana dari arsitektur GPT (Generative Pre-trained Transformer) menggunakan PyTorch. Project ini dibuat untuk mempelajari konsep dasar Transformer, Self-Attention, dan proses generasi teks.

## Deskripsi

Model dilatih menggunakan dataset teks sederhana yang berisi materi tentang Machine Learning dan Artificial Intelligence. Setelah proses training selesai, model dapat menghasilkan teks baru berdasarkan input awal (prompt) yang diberikan.

Project ini tidak bertujuan untuk membuat model sekompleks ChatGPT, tetapi lebih berfokus pada pemahaman cara kerja dasar GPT.

## Fitur

- Tokenisasi teks menggunakan SentencePiece
- Implementasi Transformer Block dari awal
- Multi-Head Self Attention
- Training model bahasa sederhana
- Generasi teks berdasarkan prompt
- Dukungan GPU menggunakan CUDA

## Struktur Project

```bash
tinyGPT-main/
│
├── corpus.txt
├── tinygpt.py
├── transformer_blocks.py
├── tokenizer.model
├── tokenizer.vocab
├── LICENSE
└── README.md
```

## Requirements

- Python 3.10+
- PyTorch
- SentencePiece

Install dependency:

```bash
pip install torch sentencepiece
```

## Cara Menjalankan

Jalankan perintah berikut pada terminal:

```bash
python tinygpt.py
```

Jika GPU NVIDIA tersedia, model akan otomatis menggunakan CUDA.

## Dataset

Dataset yang digunakan berupa kumpulan teks sederhana mengenai topik Machine Learning dan Artificial Intelligence yang disimpan pada file `corpus.txt`.

## Hasil

Contoh hasil generasi teks:

```text
machine learning menggunakan data Reinforcement learning memiliki label Metode ini banyak data yang dihasilkan pembelajaran
```

Karena dataset yang digunakan masih sangat kecil, hasil generasi teks belum sepenuhnya sempurna. Namun model sudah mampu mempelajari pola dasar dari data pelatihan.

## Tujuan Project

Project ini dibuat sebagai media pembelajaran untuk memahami:

- Tokenization
- Embedding
- Self-Attention
- Transformer Block
- Language Modeling
- Text Generation

## Author

Muhammad Noer Attalah Dzahkwan
