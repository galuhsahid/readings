# readings
List of (mostly) data-related books & papers/articles that I've read.

The pdfs that I uploaded here are all annotated - however these are my personal annotations so they might be unreadable. I'll always link to the original post/paper in case you want to check it out yourself (you should!).

## books
- [**Artificial Intelligence: A Guide for Thinking Humans:**](https://www.goodreads.com/book/show/43565360-artificial-intelligence) how did AI come about in the first place? Where are we now with AI? How far away are we from AGI? I read this in the middle of the GPT-3 hype & it was truly a sobering read. 
- [**Build a Career in Data Science:**](https://www.goodreads.com/book/show/52661559-build-a-career-in-data-science) recommended read if you: are looking to break into the data science field or are already in the field but wondering what the possible career path(s) are like.
- [**Feature Engineering and Selection: A Practical Approach for Predictive Models:**](https://www.goodreads.com/book/show/45832399-feature-engineering-and-selection) pretty much covers most of the major feature engineering and selection methods that you need to know in one place. I often find learning resources related to these topics to be scattered all over the internet so it's helpful to have them in one place. Each methodology is also supported with its strength and drawback, as well as a case study (with bonus R code!) to illustrate how it works.
- [**The Effective Engineer:**](https://www.goodreads.com/book/show/25238425-the-effective-engineer) not about data, so not 100% of the examples are probably relatable, but this book really helps me to think about how I can be an effective data scientist.
- [**Thinking with Data:**](https://www.goodreads.com/book/show/20344187-thinking-with-data) This book contains everything you need to know about working on data projects that does not have anything to do with algorithms etc. If you're not yet comfortable with topics like scoping, project management, dealing with stakeholders---this book is for you. I think anyone who wants to be a good data practitioner beyond fitting models should definitely read this book cover-to-cover. You can also read my reading notes [here](https://galuh.me/reading-notes-data/).

## articles/papers
### general
- **150 Successful Machine Learning Models: 6 Lessons Learned at Booking.com [(annotated pdf)](bernardi-booking.pdf) [(paper)](https://www.kdd.org/kdd2019/accepted-papers/view/150-successful-machine-learning-models-6-lessons-learned-at-booking.com):** Lessons learned from ML models deployed at Booking.com. Some of the most memorable examples (to me) are around monitoring & experiment design. The examples are mostly skewed towards features you can find in Booking.com e.g. hotel/destination recommendations.
- **Challenges in Deploying Machine Learning: a Survey of Case Studies [(annotated pdf)](paleyes-challenges_ml.pdf) [(paper)](https://arxiv.org/abs/2011.09926):** This paper covers a lot of aspects related to deploying machine learning; a must-read for those who wish to learn more about what it takes to deploy ML in the real-world (besides the training part!). Some of my favorite takeaways: 1) continuous delivery for ML models is complicated because for ML, there are 3 moving parts: code, data, model (as opposed to just the code). 2) When it comes to end users' trust, there are limits to ML explainability. Most of the time more efforts are required, e.g. engaging with domain experts from very early on, establishing mechanisms for accountability. 3) Data Oriented Approach (DOA) aims to replace microservice architecture with streaming-based architecture. Personally, I've about this idea in passing but never really read up on it.
- **Classifier calibration [(annotated pdf)](poulopoulos-calibration.pdf) [(article)](https://towardsdatascience.com/classifier-calibration-7d0be1e05452):** Classifier calibration 101. What is it, why do we calibrate models, why & when to use it.
- **On Being a Data Skeptic [(annotated pdf)](oneil-data_skeptic.pdf) [(article)](https://www.oreilly.com/content/on-being-a-data-skeptic/):** a timeless read. This is from 2013 but many, if not all points, are still relevant today. A mandatory reading for all data practicioners IMO.
- **Software 2.0 [(annotated pdf)](karpathy-software.pdf) [(article)](https://medium.com/@karpathy/software-2-0-a64152b37c35):** This essay explores what Karpathy names "Software 2.0"; in contrast to Software 1.0, where humans write explicit instructions to the computer, in Software 2.0 we "specify some goal on the behavior of a desirable program". By this definition, things like neural networks are considered as Software 2.0 & not just a tool. This essay also explores the limitations of Software 2.0, including interpretability, bias, & adversarial attack.
- **The End of Moore's Law, CPUs (as we know them), and the Rise of Domain Specific Architectures [(annotated pdf)](hennessy-dsa.pdf) [(slides)](https://www.kisacoresearch.com/sites/default/files/presentations/09.00_-_alphabet_-_john_hennessy.pdf):** I read this to better understand the paper *The Hardware Lottery*. This slide deck explains why we're moving towards Domain Specific Architectures---the downfall of Moore's Law being one of the reasons.
- **The Hardware Lottery [(annotated pdf)](hooker-hw_lottery.pdf) [(paper)](https://arxiv.org/abs/2009.06489):** this paper discusses that throughout history, hardware & software have frequently determined which research ideas succeed. This is even more worrisome when we take into account the fact that we're moving towards Domain Specific Architectures (DSA); the implication would be that some research directions (the ones with DSAs available/DSAs that are commercially viable) will prevail while other research directions that have potential (& can even possibly be better given the chance), yet are not supported by existing DSAs might be left behind.
- **What’s Keeping Women Out of Data Science? [(annotated pdf)](bcg-women_ds.pdf) [(article)](https://www.bcg.com/en-us/publications/2020/what-keeps-women-out-data-science):** findings include a) women seek for clear information of what the day-to-day job is really like; b) women also seek for more opportunities with actual practicioners, because they're looking for a direct feel of the ways of working, degree of collaboration, personalities which cannot be conveyed through corporate slideshows. I think this further emphasizes why representation is very important.


### metrics
- **Categorizing Variants of Goodhart's Law [(annotated pdf)](manheim-garrabrant_goodharts.pdf) [(paper)](https://arxiv.org/abs/1803.04585):** one of the papers/work I can find that touch on the relation between Goodhart's Law & ML/AI. The paper explores 4 types of Goodhart's Law: Regressional Goodhart, Extremal Goodhart, Causal Goodhart, & Adversarial Goodhart. 
- **Designing and evaluating metrics [(annotated pdf)](taylor-design_eval_metrics.pdf) [(article)](https://medium.com/@seanjtaylor/designing-and-evaluating-metrics-5902ad6873bf):** this article explores the five properties of metrics to keep in mind when designing a metric (Cost, Simplicity, Faithfulness, Precision, & Causal Proximity) & lifecycle of a metric.
- **How do you set metrics? [(annotated pdf)](zhuo-how_to_set_metrics.pdf) [(article)](https://medium.com/the-year-of-the-looking-glass/how-do-you-set-metrics-59f78fea7e44):** pretty self-explanatory. One of my key takeaways is: "start with a plain-language statement about what a successful outcome would look like in human terms" & then go from there. Other takeaways include: track counter-metrics, avoid having too many metrics, understand the dynamic between metrics, avoid vanity metrics.
- **Metrics Versus Experience [(annotated pdf)](zhuo-metrics_exp.pdf) [(article)](https://medium.com/the-year-of-the-looking-glass/metrics-versus-experience-a9347d6b80b):** some points overlap with the ones discussed in *How do you set metrics?*. Main takeaway is it's not metrics vs experience. Metrics are helpful, the question is how do we design good metrics?

### NLP
- **Abusive Language Detection in Online User Content [(annotated pdf)](nobata-abusive-lang-detection.pdf) [(paper)](http://www.yichang-cs.com/yahoo/WWW16_Abusivedetection.pdf):** abusive language classification problem. Best result uses character n-grams (also beats deep learning approach.)
- **Deep Learning Based Text Classification: A Comprehensive Review [(annotated pdf)](minaee-text-dl.pdf) [(paper)](https://arxiv.org/abs/2004.03705):** A survey of more than 150 deep learning models & +40 text classification datasets. There's also a quantitative analysis of the performance of these models on several datasets.
- **The Unreasonable Effectiveness of Recurrent Neural Networks [(annotated pdf)](karpathy-rnn.pdf) [(article)](http://karpathy.github.io/2015/05/21/rnn-effectiveness/):** Primer to RNNs & how they work. Recommended reading if you haven't learned RNN before but want to delve into recent NLP surveys; most will definitely talk about RNN & it's helpful to know how RNNs work & their shortcomings.
- **Multilingual Multi-class Sentiment Classification Using Convolutional Neural Networks [(annotated pdf)](attia-sentiment-cnn.pdf) [(paper)](https://research.google/pubs/pub46932/):** language-independent deep learning model for multi-class sentiment analysis. Evaluated on English, German, & Arabic datasets. Uses oversampling to handle the class imbalance.
- **NLP for supervised learning [(annotated pdf)](yan-nlp_for_supervised_learning.pdf) [(article)](https://eugeneyan.com/writing/nlp-supervised-learning-survey/):** Recommended if you need to catch up with all of the progress going on in (supervised learning) NLP so far.
- **The Illustrated Transformer [(annotated pdf)](alammar-transformers.pdf) [(article)](http://jalammar.github.io/illustrated-transformer/):** Have trouble understanding how transformers work? This article (& especially its illustrations) will make it easier for you to understand how it works.
- **Visualizing A Neural Machine Translation Model (Mechanics of Seq2seq Models With Attention) [(annotated pdf)](alammar-attention.pdf) [(article)](https://jalammar.github.io/visualizing-neural-machine-translation-mechanics-of-seq2seq-models-with-attention/):** I found Attention quite difficult to visualize when I'm just reading words on a paper. Recommended if you're a visual learner & want to delve deep into how attentions work.

## videos
I've been watching a lot of videos instead of articles/papers lately, thought I'd list them here as well.
- **Anomaly Detection: Algorithms, Explanations, Applications [(video)](https://www.youtube.com/watch?v=12Xq9OLdQwQ):** Lecture on anomaly detection, specifically using outlier detection approach which is suggested when the number of anomaly points only makes up a small % (< 5%). Highlights for me: 1) based on their benchmarking, isolation forest is pretty robust; 2) anomaly explanation with Sequential Feature Explanations; 3) Application on open category detection.
- **Train, Evaluate, Repeat: Building a Credit Card Fraud Detection System [(video)](https://www.youtube.com/watch?v=rHSpab1Wi9k):** Challenges that Stripe faced when building a fraud detection system & how they overcame them. Three challenges highlighted in the talk: a) defining the label, b) handling class imbalance (fraudulent transactions only make up <1 % of total transactions) by fixing the target rate for the positive class (as opposed to determining a fixed subsampling rate for the negative class), c) model evaluation. Interestingly, the last part of the talk, on model evaluation, is an update from the talk [Counterfactual evaluation of machine learning models](https://www.youtube.com/watch?v=QWCSxAKR-h0) that I watched a while ago. It highlighted some issues with the initial attempt on counterfactual evaluation, namely a) how a misclassified single high-weight transaction can really shift the estimates significantly, b) the initial propensity function assumes that transactions are independent, & they cannot guarantee that the events are indeed independent (e.g. repeated attempts of the same transaction).
