# covid-faq-bert

This is a final project task from our information retrieval class where we built an Indonesian COVID-19 Frequently Asked Questions (FAQ) retrieval system. When a user asks a question related to COVID-19 in Indonesian language, our system will look up the answer on our dataset or corpus, which consists of thousands of question and answer pairs, and then retrieve the answer to the user based on the highest similarity between the question provided by the user and the question-answer pair in the corpus. For our system to be able to do this, we embed the question provided by the user and the corpus using the state-of-the-art pre-trained language model BERT and calculate the similarity using cosine similarity.

## Dataset

We create the corpus by collecting a question-answer pairs in Indonesian related to COVID-19 from indonesian health forum website Alodokter. In this forum, the question was asked by a patient, and the answer was replied by a qualified, registered doctor. From this website, we obtained around 1800 question-answer pairs

## Word Embedding

As mentioned before, we use pre-trained BERT to convert the questions and QA pairs to a dense vector representation. We evaluate several BERT variations and compare which one is better on processing Indonesian language. This variations are:

<ul>
<li>multilingual-BERT (m-BERT)</li>
<li>sentence-BERT (SBERT)</li>
<li>IndoBERT</li>
<li>A lite BERT (ALBERT)</li>
<li>XLM-RoBERTa</li>
</ul>
