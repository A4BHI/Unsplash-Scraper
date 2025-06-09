# 🖼️ Unsplash Image Scraper

A desktop application built using **Java Swing** that scrapes and downloads high-quality images from [Unsplash](https://unsplash.com) based on user-provided keywords.

## 🚀 Features

- 🔍 Search Unsplash by keyword
- ⬇️ Download images in high resolution
- 🗂️ Saves all images inside a `Scrapper` folder in the system's `Downloads` directory
- 📄 Displays real-time download status
- 📸 Simple and user-friendly GUI built with Java Swing

## 🖼️ UI Preview

![UI Screenshot](screenshot.png) <!-- Replace with your actual screenshot file name -->

## 📦 How It Works

1. Enter a **keyword** (e.g., `sunset`, `car`, `nature`)
2. Enter the **number of images** to download
3. Click **Scrape**
4. App fetches image data from the Unsplash JSON API
5. Downloads images in real-time, 5 per page

## 🧠 Logic Summary

- Sends requests to:  
  `https://unsplash.com/napi/search/photos?page={page}&per_page=20&query={keyword}`
- Parses the JSON to extract `urls.full`
- Downloads in batches of 5 per page

## 🛠️ Requirements

- Java 8 or higher
- `org.json` library

You can download the `org.json` JAR from [here](https://mvnrepository.com/artifact/org.json/json).

## 💾 Output Directory

Downloaded images are saved to: C:\Users<YourUsername>\Downloads\Scrapper\
