
# **Sentiment Analysis on a Military-Style Boot Camp Program for Troubled Students in West Java**

##  **Background**

In May 2025, a military-style boot camp program for troubled students in West Java—initiated by **Dedi Mulyadi**—sparked intense public debate. The program was designed to instill discipline and improve student behavior through militaristic training.

While some supported the program as a strict and effective approach to youth delinquency, others criticized it for being too harsh and potentially violating children's rights.

Social media, especially **YouTube**, became the primary platform where the public expressed their opinions. Conducting sentiment analysis on these conversations provides valuable insight into public perception and helps policymakers better understand how society views the program.

---

##  **Research Questions**

1. What major issues arise regarding the military-style boot camp program?
2. What is the overall public sentiment toward the program?
3. How do online discussions evolve over time, especially on YouTube?
4. How do netizens respond to **Dedi Mulyadi** as the initiator of the program?

---

##  **Data Collection Period**

**May 2 – May 27, 2025**

##  **Data Source**

**YouTube Comments** collected via YouTube Data API.

##  **Keywords Used**

* Program barak militer
* Barak Militer Dedi Mulyadi
* Barak militer anak
* Barak militer siswa
* Siswa nakal Jawa Barat

---

#  **Data Preparation**

### **1. YouTube Data Collection**

We collected comments from multiple YouTube videos using five keywords. To avoid overlap, comments from different keywords were merged and deduplicated.

### **2. Preprocessing Steps**

* Remove duplicates
* Add sentiment labels (1 = Positive, 2 = Neutral, 3 = Negative)
* Clean text
* Normalize text
* Remove stopwords
* Lemmatization
* Tokenization

No missing values were found.

---

# **Visualization & Interpretation**

### **1. Daily Comment Trends**

Two major comment spikes occurred:

* **May 4** (549 comments)
* **May 23** (627 comments)

These increases likely followed viral discussions, public statements, or responses by key figures.

---

### **2. Sentiment Distribution**

* **Neutral (53.5%)** – mostly informational or critical without emotional tone
* **Positive (44.5%)** – support for discipline-building and controlling youth delinquency
* **Negative (2.0%)** – concerns about harshness, authoritarianism, or ineffective policy

---

### **3. Sentiment Insights**

* Positive comments focus on discipline, national values, and moral improvement.
* Negative comments highlight concerns about militarization, child psychology, and authoritarian tendencies.
* Neutral comments contain critiques, suggestions, or debates without strong emotional markers.

---

#  **Topic Modeling (Positive Sentiment)**

### **Cluster 1: Religious Expressions**

Keywords: *masyallah, subhanallah, amin, berkat, amanah*
→ Public displays of admiration, spirituality, and moral support.

### **Cluster 2: Nationalism & Politics**

Keywords: *nasionalisme, demokrasi, kritik, leadership*
→ Program viewed in the context of national identity and political discourse.

### **Cluster 3: Education & Physical Training**

Keywords: *latih, fisik, guru, kurikulum, proses*
→ Focus on discipline building, training, and educational comparisons.

### **Cluster 4: Motivation & Program Sustainability**

Keywords: *pindah, pantang, lanjutkan, langkah*
→ Support for the continuation and long-term impact of the program.

---

#  **Tools & Libraries**

* Python
* YouTube Data API
* Pandas
* NLTK / spaCy
* Scikit-learn
* Matplotlib / Seaborn
* BERTopic (if applicable)

---

#  **Conclusion**

This sentiment analysis highlights the complexity of public perception regarding the military-style boot camp program. While many support it for its disciplinary purpose, others express concerns about child welfare, ideology, and implementation methods.

The analysis also shows that:

* Neutral comments dominate due to critical but emotionless discussions.
* Debate peaks follow content that is emotional, controversial, or politically charged.
* Public discussion forms clusters tied to religion, nationalism, education, and social critique.

---
