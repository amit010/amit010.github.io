---
layout: page
title: LLM Personalization
description: LLM, Huggingface, Scikit Learn, Python, Probabilistic and Neural Retrievers.
img: assets/img/clustering-ir.jpg
importance: 1
category: Graduate
related_publications: true
---

<a href="https://amit010.github.io/assets/pdf/LLM_Personalization.pdf">[Report]</a> <a href='https://github.com/amit-sarker/LLM_Personalization'>[Code]</a>

<strong>Project Title:</strong> Improving Retrieval Accuracy Using Clustering to Personalize Large Language Models.

<p style="text-align:justify">
<strong>Project Overview:</strong> This project focuses on improving the personalization capabilities of Large Language Models (LLMs) by advancing the retrieval of user profile information. By using novel retrieval strategies, including clustering and reranking methods, this project aims to optimize LLM outputs to be more user-specific and contextually relevant.
</p>
The project focuses on the following research questions (RQs):
<ul>
    <li> RQ1: How can relevant information be extracted from a user profile to personalize the output of a Large Language Model (LLM)? </li>
    <li> RQ2: How can the prompt to personalize an LLM output be optimized when the relevant user information is large? </li>
</ul>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/clustering-ir.jpg" title="project structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This figure shows our clustering approach for retrieval. In our approach, we first cluster the documents using KMeans. We then sample a data point or document from a cluster. Finally, we rerank the documents using contriever.
</div>


<p style="text-align:justify"><strong>Challenges:</strong> This project addresses a suite of challenges related to enhancing the personalization capabilities of Large Language Models (LLMs) through advanced information retrieval strategies.</p>
<ul>
    <li> <p style="text-align:justify">The core challenge is to extract relevant and significant data efficiently from voluminous and diverse user profiles. This is crucial to ensure that the LLM outputs are both contextually relevant and accurate.</p> </li>
    <li> <p style="text-align:justify">The project explores ways to manage large datasets efficiently. It aims to optimize the input sequences for LLMs, making it feasible to process large volumes of data without compromising the quality of the outputs.</p> </li>
    <li> <p style="text-align:justify">One of the significant hurdles is enhancing personalization while operating within the bounds of limited computational resources. The project develops retrieval strategies like clustering and reranking that aim to reduce computational demands while maintaining or enhancing performance.</p> </li>
    <li> <p style="text-align:justify">Achieving a delicate balance between the accuracy of retrieved information and its relevance to the user's context is challenging. Different models are tested to identify methods that can optimize both aspects effectively.</p> </li>
    <li> <p style="text-align:justify">Another challenge is conducting experiments that closely mirror real-world conditions. Using realistic datasets, such as those from the LaMP benchmark, the project validates the effectiveness of different retrieval models in practical scenarios.</p> </li>
</ul>

<p style="text-align:justify"><strong>Methods:</strong> The project used a comprehensive approach to tackle the challenges of personalizing outputs from Large Language Models (LLMs) through information retrieval strategies. Here are the specific solution methods used:</p>
<ol>
    <ul>
        <li> BM25 Baseline: Used as a baseline to set a standard for performance comparison with more advanced methods. </li>
        <li> Topic-Model Based Retrieval: This method uses BM25 to first rank the data points and then incorporates topic modeling to streamline and shorten the input by focusing on key topics rather than full texts. </li>
        <li> Reranking with Contriever: After initial ranking with BM25, this method uses the Contriever model to rerank the results, aiming to improve relevance by refining the selection of user profile data. </li>
        <li> </li>
    </ul>
</ol>



You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
