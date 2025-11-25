# 🎯 AI Resume Matcher

The **AI Resume Matcher** is a powerful, single-page web application designed to help recruiters and job seekers quickly determine the best resume fit for a given job description (JD). It uses the **Gemini API's multimodal capabilities** to analyze PDF resumes and rank them based on both keyword presence and contextual relevance.

---

## ✨ Features

- **Multimodal Analysis:** Uploads and reads the content from multiple PDF resumes against a single job description.
- **Contextual Ranking:** Ranks resumes not just by keyword count, but by prioritizing deeper contextual relevance (e.g., demonstrated experience, leadership, progression) to handle cases where scores are close.
- **Match Scoring:** Generates a match percentage and a detailed justification for the ranking of each resume.
- **Detailed Comparison:** Provides a side-by-side view of the Job Description and the top-ranked resume, with key matching terms highlighted using the `<mark>` tag.
- **Single-File Simplicity:** The entire application is self-contained within a single **ResumeMatcher.html** file (HTML, Tailwind CSS, and JavaScript).

---

## 🚀 Setup and Prerequisites

To run this application, you only need **one** thing:

### Gemini API Key

1. **Get a Key:** Obtain your personal API key from **Google AI Studio**.
2. **Insert Key:** Open the `ResumeMatcher.html` file and locate the following line near the top of the `<script>` tag:

    ```javascript
    const apiKey = ""; // <-- PASTE YOUR API KEY HERE
    ```

3. Replace the placeholder value with your actual Gemini API key.

---

## 🛠️ Usage

1. **Open the File:** Load the `ResumeMatcher.html` file directly in your web browser or use a live preview environment (like the Canvas editor).
2. **Paste Job Description:** Enter the full text of the job description into the first text area.
3. **Upload Resumes:** Click the upload box to select one or more PDF resume files.
4. **Analyze:** Click the **"Analyze & Rank Resumes"** button. The application will send the JD and the PDF files to the Gemini API for analysis.
5. **Review Results:** The ranked list will appear below. Click **"View Detailed Match"** on the Rank #1 resume to see the side-by-side highlighted comparison.

---

## 🔒 Privacy and Data Handling

The resume files you select are converted to **Base64 format** in your browser and are sent directly to the Gemini API as part of the analysis request. They are **not stored or saved** persistently by this local HTML application.
