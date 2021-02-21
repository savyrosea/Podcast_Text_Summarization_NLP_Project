# Podcast_Text_Summarization_NLP_Project

# Overview
I spend countless hours a week absorbing podcasts, and I am also passionate about exploring new NLP techniques. In this project I wanted to explored the new PEGASUS text abstraction model and comparare it the T5 abstractive text summarization from the transformers library. I am comparing these two text summarization models while summarizing some top 2021 podcast descriptions. Hopefully I discover a new podcast to listen to along the way!

# Data
The podcast descriptions and photos used in this project were scraped from a goodhousekeeping article that can be found here:

https://www.goodhousekeeping.com/life/entertainment/g28353940/best-podcasts/

# Text Summarization Using Pegasus
The first method of text summarization that I wanted to explore was PEGASUS. PEGASUS is the latest state-of-the-art model for abstractive summarization open-sourced by Google. I am using a Pegasus model that has been pre-trained on the XSUM dataset as well as using this huggingface page as a basis for my Pegasus model.

https://huggingface.co/google/pegasus-xsum

I also looked at the distribution of the length of the original podcast description compared to the new summary that PEGASUS created.
![](https://github.com/savyrosea/Podcast_Text_Summarization_NLP_Project/blob/main/images/InputOutputDistribution.PNG)

Read more about Pegasus here: 

https://ai.googleblog.com/2020/06/pegasus-state-of-art-model-for.html


# Text Summarization Using T5
In this model, I am using the T5 model to summerize text by using the Google T5 encoder-decoder model. 
The basis for this method of summerization can be found here:

https://huggingface.co/transformers/task_summary.html

# Example Outputs
![](https://github.com/savyrosea/Podcast_Text_Summarization_NLP_Project/blob/main/images/99Invisible.PNG)

![](https://github.com/savyrosea/Podcast_Text_Summarization_NLP_Project/blob/main/images/EarHustle.PNG)

# My Findings
In general, Pegasus is more casual, fun, and grammatically correct, but sometimes takes too big of leaps and draws conclusions that are not true. 
The T5 model is more accurate summarization but uses poor grammar, often leaving sentences hanging even if the summary hasn't met the max word requirement.

There were examples when the Pegasus preformed better than the T5 model:
![](https://github.com/savyrosea/Podcast_Text_Summarization_NLP_Project/blob/main/images/RadioCherryBombe.PNG)

And vice versa:
![](https://github.com/savyrosea/Podcast_Text_Summarization_NLP_Project/blob/main/images/EveryLittleThing.PNG)
