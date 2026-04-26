# 📰 Bangla Fake News Dataset

## 📌 Overview

This repository contains a Bangla-language dataset designed for **fake news detection** tasks.
The data has been collected from various online sources, including news websites and YouTube, and includes both **authentic and misleading content**.

Each row represents a single news instance with its associated metadata and label.

---

## 🧱 Dataset Structure

| Column Name    | Description                                                        |
| -------------- | ------------------------------------------------------------------ |
| `title`        | Headline of the news article                                       |
| `text`         | Full news content or video description (Bangla text)               |
| `source`       | Source platform or publisher (e.g., website, YouTube channel)      |
| `publish_date` | Publication date (format: MM/DD/YYYY; may be generated if missing) |
| `category`     | News category (e.g., politics, entertainment, etc.)                |
| `url`          | Original link to the content                                       |
| `label`        | Target label (`fake` / `real` or `0` / `1`)                        |

---

## 📥 Data Collection

- Data was collected using web scraping techniques from:
  - Bangla news websites
  - YouTube video titles and descriptions

- The dataset includes:
  - Real news content
  - Fake, misleading, or satire-style content

---

## 🧹 Raw Data Characteristics

Since the data is scraped from real-world sources, it may contain:

- Duplicate or near-duplicate entries
- Hashtags and promotional content
- Mixed language (Bangla with English phrases)
- Missing or synthetic `publish_date` values

All text is encoded in **UTF-8**, ensuring Bangla text remains fully readable.

---

## ⚙️ Preprocessing

Typical preprocessing steps include:

- Removing empty or invalid rows
- Cleaning hashtags and boilerplate/disclaimer text
- Normalizing whitespace and formatting
- Deduplicating based on `title`, `text`, or `url`
- Generating missing `publish_date` values
- Shuffling the dataset to eliminate ordering bias

---

## 📊 Use Cases

- Fake news detection (binary classification)
- Bangla NLP research
- Training deep learning models (e.g., transformer-based models, RNNs)

---

## ⚠️ Limitations

- Possible class imbalance
- Source bias across labels
- Noise from scraped content
- Generated dates are not suitable for temporal analysis

---

## 📈 Dataset Size

- ~2600+ samples (may vary after cleaning)

---

## 📜 License

This dataset is intended for **research and educational purposes only**.

---

## 🤝 Contribution

Contributions are welcome! You can:

- Improve data quality
- Add new labeled samples
- Enhance preprocessing

---

⭐ If you find this dataset useful, consider starring the repository!
