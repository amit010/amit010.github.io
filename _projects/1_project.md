---
layout: page
title: LLM Personalization
description: LLM, Huggingface, Scikit Learn, Python, Probabilistic and Neural Retrievers.
img: assets/img/clustering-ir.pdf
importance: 1
category: Graduate
related_publications: true
---

<strong>Project Title:</strong> Improving Retrieval Accuracy Using Clustering to Personalize Large Language Models.

<p style="text-align:justify">
Project Overview: This project focuses on improving the personalization capabilities of Large Language Models (LLMs) by advancing the retrieval of user profile information. By using novel retrieval strategies, including clustering and reranking methods, this project aims to optimize LLM outputs to be more user-specific and contextually relevant.
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
