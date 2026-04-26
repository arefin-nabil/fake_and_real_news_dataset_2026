# 📰 Bangla Fake News Dataset

## 📌 Overview

This repository contains Bangla news data for **fake news detection**.
Total dataset size: **~5355 rows, 7 columns**

---

## 📂 Files

### `fake_raw.csv`

Fake news dataset
Columns: `title`, `text`, `source`, `publish_date`, `category`, `url`, `label`

---

### `real_raw.csv`

Real news dataset
Columns: `title`, `text`, `source`, `publish_date`, `category`, `url`, `label`

---

### `full_dataset.csv`

Merged (real + fake) dataset
Columns: `title`, `text`, `source`, `publish_date`, `category`, `url`, `label`

---

### `dl_dataset.csv`

Processed dataset for deep learning
Columns: `title`, `text`, `label`

---

## 🏷 Label Info

- `0 = real`
- `1 = fake`

---

## 🧹 Notes

- Bangla text (UTF-8 encoded)
- Basic cleaning applied (empty rows, duplicates, noise removed)
- Dataset is shuffled

---

## 📊 Usage

- Fake news detection
- NLP / text classification

---

⭐ Use for learning and research
