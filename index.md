---
layout: home
title: MMU-RAG
subtitle: NeurIPS 2025 Competition
---

Welcome to the official website of **MMU-RAG**: the *Massive Multi-Modal User-Centric Retrieval-Augmented Generation* Benchmark. This competition invites researchers and developers to build RAG systems that perform in real-world conditions.


---
# **2025 MMU-RAGent Competition — Official Winners Announcement**

We are excited to announce the results of the 2025 MMU-RAGent Competition, which brought together teams from around the world to tackle challenging problems in multimodal Retrieval-Augmented Generation (RAG). This year’s competition featured two tracks: (1) Text-to-Text and (2) Text-to-Video. Both tracks were evaluated through a combination of automatic metrics, LLM-as-a-judge, human annotation, and our real-time RAG-Arena live evaluation.

Across both tracks, participants demonstrated creative system designs, robust retrieval pipelines, and thoughtful approaches to grounding generative models in multimodal evidence.

------



## **Participation Overview**

This year’s competition received:

- **8 full-system submissions** to the Text-to-Text track
- **2 additional validation-only submissions**, and
- **1 full-system submission** to the Text-to-Video track

To support development, we released development, validation, and held-out test sets totalling nearly **1,000 queries**.
Human evaluation played a central role in our assessment: across both tracks, we collected **2,315 annotations** from **1,197 annotators**, ensuring broad and reliable feedback on relevance, factuality, and utility.

------



# **Text-to-Text Track Winners**

Final rankings were determined using a robustness-aware aggregation of normalized automatic metrics and human Likert evaluations, with LLM-as-a-judge analysis informing, but not directly contributing, to the final scores.

Winners were recognized in two evaluation modes:

- **Static Evaluation:** Teams distinguished themselves through strong semantic alignment, factual grounding, and robustness across automatic and human Likert evaluation modalities.
- **Dynamic Evaluation (RAG-Arena):** In real-time interactive comparisons, these winners were preferred most frequently by users, highlighting the importance of evaluating not just correctness, but also clarity, usefulness, and overall preference.

---

<table class="no-stripe">
<thead>
<tr>
<th style="text-align: center;"><strong>🏆 Open Source</strong></th>
<th style="text-align: center;"><strong>🏆 Closed Source</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td style="vertical-align: top; padding: 1.5rem;">
<h3 style="margin-top: 0; color: #2c3e50;">🥇 Best Static Evaluation</h3>
<p style="font-size: 1.3em; font-weight: bold; margin: 0.5rem 0; color: #1a73e8;"><strong>Efficient-Deep-Research</strong></p>
<br>
<h3 style="margin-top: 1rem; color: #2c3e50;">🥇 Best Dynamic Evaluation</h3>
<p style="font-size: 1.3em; font-weight: bold; margin: 0.5rem 0; color: #1a73e8;"><strong>RMIT-ADMS IR</strong></p>
</td>
<td style="vertical-align: top; padding: 1.5rem;">
<h3 style="margin-top: 0; color: #2c3e50;">🥇 Best Static Evaluation</h3>
<p style="font-size: 1.3em; font-weight: bold; margin: 0.5rem 0; color: #1a73e8;"><strong>Cattalyya</strong></p>
<br>
<h3 style="margin-top: 1rem; color: #2c3e50;">🥇 Best Dynamic Evaluation</h3>
<p style="font-size: 1.3em; font-weight: bold; margin: 0.5rem 0; color: #1a73e8;"><strong>Nightfeats</strong></p>
</td>
</tr>
</tbody>
</table>

------



# **Text-to-Video Track Winner**

The Text-to-Video track received one full submission, DeepVideoResearcher, We evaluated the system against a strong baseline (Nova-Reel) using both VBench automatic metrics and human utility assessments.

Although the baseline demonstrated higher visual-quality metrics, human evaluators preferred deepvideo-researcher for relevance, precision, and overall utility to the query. This highlights the gap between traditional visual metrics and user-oriented evaluation of RAG-generated videos.

---

<table class="no-stripe">
<tbody>
<tr>
<td style="vertical-align: top; padding: 1.5rem; text-align: center;">
<h3 style="margin-top: 0; color: #2c3e50;">🏆 Best Human Likert Rating</h3>
<p style="font-size: 1.3em; font-weight: bold; margin: 0.5rem 0; color: #1a73e8;"><strong>Deepvideoresearcher</strong></p>
<p style="margin-top: 0.5rem; color: #666;">Outperformed the baseline text-to-video model in Human Likert Rating</p>
</td>
</tr>
</tbody>
</table>

------



# **Key Insights From This Year’s Evaluation**

- **Human and LLM-as-a-judge ratings align strongly** (correlations ≈ 0.93), validating the use of LLMs for diagnostic evaluation while reinforcing that human ratings should remain the final authority.
- **Live evaluation matters:** Arena preferences revealed qualitative distinctions not captured by static metrics.
- **Multimodal video evaluation remains challenging:** Existing automatic metrics emphasize visual fidelity, while human evaluators prioritize task relevance and procedural clarity.

------



We extend our warmest congratulations to the winning teams, and our sincere appreciation to every participant who contributed to this year’s competition. Your work pushes the boundaries of retrieval-augmented generation and helps shape the future of multimodal reasoning systems.

___

<!-- ### Update 06 Oct 2025
As we approach the competition deadline, we’d like to share a few important updates and reminders to help you prepare your final submissions.

#### 🗓️ Submission Deadline
The submission will close on October 15 (23:59 AoE). Please make sure all materials are uploaded before the deadline.

#### 📂 Test Dataset for Static Evaluation
For participants taking part only in the static evaluation, the test-release dataset is now available at the following links: 
1. [Text-to-Text Test Set (For static evaluation) ](https://drive.google.com/file/d/1D_lbDseQIf-_f2ebTiEv1ebOoSN9PgeQ/view?usp=sharing)
2. [Text-to-Video Test Set (For static evaluation)](https://drive.google.com/file/d/1fTbAhdqfMVUj1vrbBUUdVZz2H9Wtj-WM/view?usp=sharing)

Please follow the submission instructions in the documentation and generate responses only for the queries in this list. 

#### 📝 Short System Paper
We ask each participating team to prepare a short paper describing your system and methodology.
Please use the NeurIPS short-paper format (2–4 pages).

This write-up will serve as part of the competition record and allow others to learn from your approach.

Submission details for the paper will be shared shortly after the system submission deadline.

#### 🗣️ Workshop & Presentations
We’re excited to announce that the MMU-RAG Workshop will take place at NeurIPS 2025 on
 📅 Sunday, December 7, from 3–6 PM PDT.
Selected teams will be invited to present their work during the session.
 If you are interested in presenting (accommodating both in-person or virtually), please indicate your interest when submitting your final materials.

Thank you again for being part of MMU-RAG! We’re looking forward to seeing your submissions and showcasing your work at NeurIPS.

------

Participants will tackle real-user queries, retrieve from web-scale corpora, and generate high-quality responses in both text and/or video formats.

**MMU-RAG** features two tracks:

1. **Text-to-Text**
2. **Text-to-Video**

Submissions are evaluated using a blend of:

- Automatic metrics
- LLM-as-a-judge evaluations
- Real-time human feedback through our interactive RAG-Arena platform

### Evaluation Methods and Metrics

**Illustration of our static evaluation methods and their corresponding metrics.**

<table class="no-stripe">
<thead>
<tr>
<th><strong>Track</strong></th>
<th><strong>Evaluation Method</strong></th>
<th><strong>Evaluation Metric</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="3"><strong>Text-to-text</strong></td>
<td>Automatic</td>
<td>Rouge-L, BERTScore</td>
</tr>
<tr>
<td>LLM-as-a-Judge</td>
<td rowspan="2">Semantic Similarity, Coverage, Factuality, Citation Quality</td>
</tr>
<tr>
<td>Human Likert Ratings</td>
</tr>
<tr>
<td rowspan="2"><strong>Text-to-video</strong></td>
<td>Automatic</td>
<td>Subject Consistency, Background Consistency, Motion Smoothness, Dynamic Degree, Aesthetic Quality, Imaging Quality (from <a href="https://vchitect.github.io/VBench-project/">VBench</a>)</td>
</tr>
<tr>
<td>Human Likert Ratings</td>
<td>Relevance, Precision, Recall, Usefulness</td>
</tr>
</tbody>
</table>

Whether you're advancing retrieval strategies, generation quality, or multimodal outputs, this is your opportunity to benchmark your system in a setting that reflects actual user needs.

------

## Timeline

### Aug 1: **Competition launch & dataset release**

Two exciting tracks, both with provided corpora, APIs, and starter codes. You are also allowed to use external resources or APIs for retrieval as long as they are clearly documented in submission.

| **Text-to-Text** ([details](/MMU-RAGent/text-to-text)) | **Text-to-Video** ([details](/MMU-RAGent/text-to-video)) |
|---|---|
| **Standard text-to-text RAG:** Create systems that retrieve from a text corpus and generate text responses from text queries<br><br>**Deep Research Systems welcome!** e.g. Multi-hop retrieval, Structured reasoning, Integration with external tools or knowledge bases, etc. | **More novel task!** Given text queries that benefit from video outputs ("how to peel banana"), Retrieve from a text corpus and generate video responses. |

### Aug 1 - Oct 24: **ACTION REQUIRED**: Register to get necessary resources

- Go to [Getting Started page](/MMU-RAGent/getting-started) to see:
  - Our competition rules
  - Instructions on registration (required)
  - Detailed instructions for the two tracks

### Aug 1 - Oct 24: **ACTION REQUIRED**: Competition Submission

**Deadline extended to October 24, 2025 (23:59 AoE)** for both Text-to-Text and Text-to-Video tracks.

- Step-by-step instructions for the [text-to-text](/MMU-RAGent/text-to-text) and [text-to-video](/MMU-RAGent/text-to-video) tracks.
- Submission options preview (applicable for both tracks):

| **Static Evaluation (Non-Cash Prizes)** | **Full System Submission (Cash Prizes)** |
|---|---|
| Run your system on the public validation set<br><br>Submit outputs (.jsonl or video folder) via Google Drive<br><br>Eligible for honorable mentions and website features | Package your RAG system as a Docker image<br><br>Submit via AWS ECR for live + static evaluation<br><br>Eligible for leaderboard rankings and cash prizes |

### Oct 24 - Nov: **Organizers Running Evaluations**

- Submissions will be evaluated using a blend of:
  - Automatic metrics
  - LLM-as-a-judge evaluations
  - Real-time user feedback from our RAG-Arena

**Action required:** All participants are required to submit a report detailing their system, methods, and results. The system report should be 2–4 page short paper following the NeurIPS short-paper format. Top-performing and innovative teams will be invited to present their work at our associated NeurIPS 2025 workshop.

### Dec 6-7: **MMU-RAG Workshop at NeurIPS 2025**

- Presentations by selected teams
- Winners and runner(s)-up announced

---

## Prizes

We're excited to offer both **monetary prizes** and **academic exposure opportunities** to recognize outstanding submissions.

### 💰 Prize Pool

Thanks to the support of Amazon, MMU-RAG offers a **$10,000 prize pool in AWS credits**. Prizes will be awarded to top-performing teams across both tracks.

### 🎤 Present at NeurIPS

Top teams will also be invited to **present their systems** during the **MMU-RAG competition session at NeurIPS 2025**. This is a unique opportunity to share your work with the community.

### 🥇 Eligibility

Prize eligibility requires full system reproducibility and clear documentation of all components. Only participants in the **Full System Submission** option are eligible for cash prizes.

---

# Contact Us

For any questions or clarifications, email the organizers directly at: mmu-rag@andrew.cmu.edu -->

## Organizers

- [Luo Qi Chan](https://luoqichan.github.io), DSO National Laboratories / Carnegie Mellon University  
- [Tevin Wang](https://tevinwang.com), Carnegie Mellon University  
- [Shuting Wang](https://shootingwong.github.io), Renmin University of China / Carnegie Mellon University  
- Zhihan Zhang, Carnegie Mellon University  
- Alfredo Gomez, Carnegie Mellon University  
- [Prahaladh Chandrahasan](https://prahaladhchandrahasan.github.io), Carnegie Mellon University  
- Lan Yan, Carnegie Mellon University  
- Andy Tang, Carnegie Mellon University  
- Zimeng (Chris) Qiu, Amazon AGI  
- Morteza Ziyadi, Amazon AGI  
- [Sherry Wu](https://www.cs.cmu.edu/~sherryw/), Carnegie Mellon University  
- Mona Diab, Carnegie Mellon University  
- [Akari Asai](https://akariasai.github.io), University of Washington
- [Chenyan Xiong](https://www.cs.cmu.edu/~cx/), Carnegie Mellon University  
