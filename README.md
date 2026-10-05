# Multi-Platform AI Content Distribution Pipeline

An automated content publishing engine built in **Zapier** that triggers on video file uploads in **Google Drive**, leverages **AI by Zapier** to generate dynamic promotional copy, and distributes posts seamlessly across **Buffer**, **LinkedIn**, and **YouTube**.

---

## 📌 Workflow Architecture


```
[Google Drive: New File in Folder]
│
▼
[AI by Zapier: Promote KOSLICH Academy...]
│
▼
[Buffer: Add to Queue (Primary Social Schedule)]
│
▼
[LinkedIn: Create Share Update]
│
▼
[Buffer: Add to Queue (Secondary Channel Schedule)]
│
▼
[YouTube: Upload Video]
```

---

## ⚡ Workflow Breakdown & Trigger Execution

1. **Trigger — Google Drive (New File in Folder)**  
   * **Action:** Listens in real-time for newly uploaded MP4/video media assets within a designated Google Drive input folder.
   * **Payload:** Extracts the media download URL, file name, creation timestamp, and raw metadata.

2. **Action — AI by Zapier (Promote KOSLICH Academy...)**  
   * **Action:** Passes raw metadata to an AI prompt step.
   * **Function:** Dynamically drafts platform-optimized social media captions, hashtag groups, and video titles tailored for marketing campaigns.

3. **Action — Buffer (Add to Queue)**  
   * **Action:** Enqueues the video asset and AI-generated social post into Buffer's primary scheduled queue for multi-platform distribution (e.g., TikTok / X).

4. **Action — LinkedIn (Create Share Update)**  
   * **Action:** Posts a native video update directly to the target LinkedIn profile/page complete with AI-tailored professional copy.

5. **Action — Buffer (Add to Queue)**  
   * **Action:** Adds a secondary queued dispatch tailored for additional connected social channels.

6. **Action — YouTube (Upload Video)**  
   * **Action:** Performs a direct native API video upload to YouTube, applying generated video titles, descriptions, and tags.

---

## 🚀 Key Benefits

* **Zero Manual Publishing Overhead:** Uploading a raw file to Google Drive automatically handles scheduling, copying, and cross-platform uploads.
* **Consistent Brand Presence:** Keeps social media channels continuously active without manual intervention.
* **Dynamic AI Copywriting:** Utilizes AI to transform raw filenames/metadata into contextual social captions.

---

## 🛠️️ Tech Stack & Integrations

* **Orchestration:** Zapier
* **Trigger Storage:** Google Drive API
* **AI Engine:** AI by Zapier (LLM Prompting)
* **Social Scheduling & Direct Distribution:** 
