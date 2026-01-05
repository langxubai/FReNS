# Fundamental Research in Natural Sciences (FReNS) Seminar

This repository hosts the official website for the **Fundamental Research in Natural Sciences Seminar**.

The seminar is dedicated to exploring cutting-edge developments across physics, mathematics, computer science, and interdisciplinary approaches. We bring together researchers and graduate students to discuss foundational questions and emerging methodologies.

🔗 **Live Website:** [https://langxubai.github.io/FReNS/](langxubai.github.io/FReNS/)

## 📅 Features
- **Schedule Management**: Lists upcoming and past talks with speaker details.
- **Modern Design**: Clean, responsive interface optimized for both desktop and mobile.
- **RSS Feed**: Supports subscription for seminar updates via `feed.xml`.

## 🛠 Maintenance Guide

To add a new seminar or update information, you need to modify two files: `index.html` and `feed.xml`.

### 1. Update the Schedule (`index.html`)
Open `index.html` and locate the `<tbody>` section inside `<section id="schedule">`. Add a new row (`<tr>`) at the top of the list:

```html
<tr>
  <td>Date</td>
  <td>Speaker Name</td>
  <td>Affiliation</td>
  <td>Talk Title</td>
  <td>Type (Talk/Lecture)</td>
  <td>Collection/Topic</td>
</tr>
```
### 2. Update the RSS Feed (feed.xml)
- To notify subscribers of a new event, open feed.xml.

- Update the <lastBuildDate> tag with the current date.

- Add a new <item> block inside the <channel> tag (place it at the top of the items list):

```XML

<item>
  <title>Talk: Speaker Name - Talk Title</title>
  <link>[https://langxubai.github.io/FReNS/#schedule](https://langxubai.github.io/FReNS/#schedule)</link>
  <guid>[https://langxubai.github.io/FReNS/talks/YYYY-MM-DD](https://langxubai.github.io/FReNS/talks/YYYY-MM-DD)</guid>
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
