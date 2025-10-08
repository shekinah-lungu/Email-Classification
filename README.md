📧 Email Classification — Ham vs Spam
🔗 Try it live here: https://shekinah-lungu.github.io/Email-Classification/

This project started as a small experiment to keep my machine learning skills sharp and learn how different techniques perform on the same task.
It turned into a complete mini AI project — from classical ML to deep learning, training, evaluation, and deployment.

The goal: build a system that can tell if an email is “ham” (normal) or “spam” (junk).

🌱 My Learning Journey

I started simple — with a Logistic Regression model.
I cleaned and vectorized the dataset using TF-IDF, trained the model, and visualized the results with a confusion matrix.

Then, I tried a transformer model (DistilBERT) using Hugging Face.
I fine-tuned it on the same dataset, compared both models, and found that the transformer learned the patterns in spam messages much better.
That difference inspired me to build a simple web interface so anyone could test the model themselves.

🧠 How It Works

The model reads your text and turns words into numbers it understands (tokenization).

It uses attention to focus on the most important words in the email (like “win”, “free”, or “urgent”).

It predicts whether the message is ham or spam, along with a confidence score.

⚙️ Models Compared
Approach	Tools	Notes
Logistic Regression	TF-IDF + scikit-learn	Simple, fast, but struggled with subtle spam wording.
DistilBERT	Hugging Face Transformers	Captured context and performed much better overall.

Both were evaluated using confusion matrices — DistilBERT’s showed fewer false positives and negatives, confirming it was the better fit.

🧩 Tech Stack

Data: SMS Spam Dataset (UCI via Hugging Face)

Classical ML: Logistic Regression + TF-IDF Vectorizer

Transformer Model: Fine-tuned DistilBERT (binary classification)

Libraries: scikit-learn, PyTorch, Hugging Face Transformers

Deployment:

Model hosted on Hugging Face Spaces
 using Gradio

Interface embedded via GitHub Pages

💻 Try It Yourself

Visit the live app: https://shekinah-lungu.github.io/Email-Classification/

Paste an email (real or fake).

Click Classify to see the result.

💬 Lessons Learned

Start simple — classical ML builds intuition before using large models.

Understanding tokenization and attention made transformers less of a “black box.”

Evaluating with confusion matrices helped me see where each model struggled.

Deployment doesn’t need to be complex — one model, one simple interface, and it works.

🧡 Built By

Agness Lungu
Master’s student in Intelligent Systems Engineering at Indiana University.
Passionate about building AI tools that are practical, human-centered, and easy to understand.

 • LinkedIn: https://www.linkedin.com/in/agness-lungu-709168196/
