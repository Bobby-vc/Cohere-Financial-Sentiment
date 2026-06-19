# Financial News Sentiment Analyzer

A financial NLP web app built on Cohere's API. Paste stock news headlines and get a bullish, bearish, or neutral trading signal with an AI-written analysis and thematic breakdown.
Built as an extension of my Multi-Agent Financial AI System, replacing the sentiment layer with Cohere's NLP stack.

How It Works

- Cohere Embed v3 converts each headline into a semantic embedding

- K-means clustering groups headlines by semantic similarity into thematic clusters

- Cohere Command R7B receives the clustered headlines and returns a structured signal: bullish/bearish/neutral score from -100 to +100, per-headline sentiment tags, cluster theme labels, and a written analysis

Stack: Python, Flask, Cohere Embed v3, Cohere Command R7B, NumPy, vanilla JS/HTML/CSS

Usage: Enter a ticker, paste headlines (one per line), add your Cohere API key, and hit Run. API key is never stored or sent anywhere except directly to Cohere.

Get a free Cohere API key at dashboard.cohere.com

Live Demo
[https://bobby-vc.github.io/Cohere-Financial-Sentiment/]
