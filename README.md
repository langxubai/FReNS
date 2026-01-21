# Fundamental Research in Natural Sciences (FReNS) Seminar

This repository hosts the official website for the **Fundamental Research in Natural Sciences Seminar**.

The seminar is dedicated to exploring cutting-edge developments across physics, mathematics, computer science, and interdisciplinary approaches. We bring together researchers and graduate students to discuss foundational questions and emerging methodologies.

🔗 **Live Website:** [https://langxubai.github.io/FReNS/](langxubai.github.io/FReNS/)

## 📅 Features
- **Data-Driven Schedule**: Talks are managed easily via a YAML data file (`_data/talks.yml`), with no HTML editing required.
- **Automatic Archiving**: Past seminars are automatically folded by year to keep the page clean.
- **Responsive Design**: Clean interface optimized for both desktop and mobile.
- **RSS Feed**: Supports subscription for seminar updates via `feed.xml`.

## 🛠 Maintenance Guide

To add a new seminar, you primarily work with the data file. To notify subscribers, you also update the RSS feed.

### 1. Update the Schedule (`_data/talks.yml`)
Open `_data/talks.yml` and add a new entry block at the **top** of the file.

**Format:**
```yaml
- date: "Month DD, YYYY"
  speaker: "Speaker Name"
  affiliation: "Affiliation"
  title: "Talk Title"
  type: "Talk"       # or "Lecture"
  collection: "Topic/Collection Name"
  link: ""           # Speaker's website URL (leave as "" if none)
```

### 2. Update the RSS Feed (feed.xml)
- To notify subscribers of a new event, open feed.xml.

- Update the <lastBuildDate> tag with the current date.

- Add a new <item> block inside the <channel> tag (place it at the top of the items list):

```XML
<item>
  <title>Talk: Speaker Name - Talk Title</title>
  <link>https://langxubai.github.io/FReNS/#schedule</link>
  <guid>https://langxubai.github.io/FReNS/talks/YYYY-MM-DD</guid>
  <pubDate>Fri, 21 Nov 2025 14:00:00 +0800</pubDate>
  <description>Speaker: Name (Affiliation). Topic: Title.</description>
</item>
```

## 👥 Organizers
Langxu Bai (Nankai University)

Siyuan He (Tsung-Dao Lee Institute, SJTU)

Lingyu Ren (Nankai University)

## 📝 License
This project is open source and available under the MIT License.
