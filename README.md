

📑 Strategic Legal Preparation Tool — Top-10 Argument Extractor

This project implements an AI/ML pipeline that processes a legal brief PDF and automatically extracts the Top-10 most significant arguments. Each key item includes:
	•	✅ Concise summary (via transformer summarizer)
	•	✅ Excerpt from the document
	•	✅ Page & line references for easy lookup
	•	✅ Stance classification (for / against / neutral)
	•	✅ Exported results in both JSON and PowerPoint

⸻

🎯 Problem Statement

Attorneys often deal with lengthy legal briefs that are difficult to digest quickly.
Our solution automatically extracts the Top-10 pivotal arguments from an amicus brief to help attorneys prepare strategically with clear evidence references.

⸻

⚙️ Pipeline Overview
	1.	PDF Extraction (PyMuPDF + OCR fallback via Tesseract)
	2.	Sentence Tokenization (NLTK)
	3.	Embeddings (Sentence-BERT: all-MiniLM-L6-v2)
	4.	Importance Ranking (TextRank over cosine similarity graph)
	5.	Stance Detection (zero-shot classification using facebook/bart-large-mnli)
	6.	Clustering (Agglomerative Clustering to group arguments)
	7.	Summarization (sshleifer/distilbart-cnn-12-6)
	8.	Export results → JSON + PowerPoint

⸻
