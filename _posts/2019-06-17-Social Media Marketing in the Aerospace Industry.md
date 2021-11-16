---
toc: true
layout: post
description: Social Media Marketing in the Aerospace Industry
image: images/flying_airliner.png
categories: [Marketing,social-media-marketing,  Deep Learning,word-embedding,sentence-embedding]
title: The Use of Social Media Marketing in the Aerospace Industry
---

## Abstract
This report considers the role of social media marketing in the aerospace industry. What is not always obvious from casual readings on this subject is the highly technical underpinnings of the effective use of this marketing approach. Aerospace marketers often outsource the detailed technical analysis to social media marketers which tend to use deep learning to perform this. These service providers seem to operate as custodians of black boxes.

![]({{ site.baseurl }}/images/flying_airliner.png " ")

## Social Media Marketing
The nature of social media conversations span a wide range. At the one extreme, there is gossip around celebrity activities, comments about the breakfast someone just finished, or maybe that her cat had a litter of 5 kittens at midnight. These types of exchanges could be classified as shallow and broad. Some refer to these connection patterns as social networks. The objective of participants is simply to link and have conversations. There are relatively few of these networks but they are large. At the other extreme we find exchanges that can be very focused and deep. These exchanges are made on networks referred to as virtual communities which are smaller in size but much more numerous. The objective of participants is not primarily to communicate, but to accomplish a task or mission. They want guidance from influencers and experts rather than peers on topics they care about. One example is [Engineering 360](https://www.globalspec.com/). In a 2014 news report, Wilinsky, describes it as the world’s largest virtual community for engineers. A few smaller communities are outlined in the article [5 Online Communities About the Aviation Industry You Should Join](https://aviationmaintenance.edu/2014/05/21/5-online-communities-aviation-industry-join/).

### Authority Brands
To target the aerospace industry, marketers continuously identify appropriate communities of aerospace influencers and experts and are positioning themselves to “develop” them. For example, [15 Aerospace Industry Professionals You Should Be Following on Social Media](https://www.cuttingdynamics.com/industry-professionals-you-should-follow-on-social-media/) identifies some influencers to follow on social media. The emphasis is on very relevant content marketing to keep the community members informed on the latest developments in the industry and to address their needs as closely as possible. Marketers are striving to position their companies as *authority brands* rather than engaging in traditional advertising. This leads to relationships founded on *value* rather than purchase transactions. In addition, these relationships connect the company with high value audiences and markets. The members become consumers of this content rather than products and services. Marketers realize that they should support their virtual communities and help them achieve their missions, rather than to engage in traditional advertising. Whenever members are ready to buy, they will come back to the authority brand’s content offerings and tend to seek its advice to initiate purchasing. 

## Social Media Terminology
Social media technology has a number of key terms. The first term is *documents*.


### Documents
Although overloaded, this term has a specific technical meaning in social media. A document is a “post” or entry on a social media site, submitted at a specific time. A good example is a “tweet” on the Twitter platform. Even though such an entry is very short and hardly qualifies as a “document” in the traditional sense of the word, it is referred to as a social media *document*.

### Hashtags
A hashtag serves as a classifier of a document. A document could have more than one hashtag, or it could have none. Hashtags need to start with the “#” character followed by a number of characters excluding spaces and punctuation, for example, `#aerospaceengineering`, or `#AerospaceEngineering` but *not* `#aerospace engineering`. Users of social media platforms are often allowed to invent their own hashtags. 

### Analysis of social media data

It is not possible for humans to manually analyze social media data due to its sheer volume. Automated systems are created to undertake this task. Data, usually in the form of text, is analyzed to discover *named entities*, *categories*, *sentiment*, *topics*, *themes*, and *intentions*.

## The Use of Hashtags
The use of hashtags is important in the analysis of social media data. The short blog, [LESSONS FROM THE AVIATION INDUSTRY: USING HASHTAGS TO HELP BOOST SOCIAL MEDIA MARKETING](https://blog.catmedia.com/lessons-from-the-aviation-industry-using-hashtags-to-help-boost-social-media-marketing), gives some insights into its use. According to the site [best-hashtags.com](http://best-hashtags.com/hashtag/aerospace/) the current top 10 aerospace hashtags are as shown in Figure 1. Some issues with relying on hashtags are immediately obvious. For example, the hashtag #engineering has strong overlaps with other areas of engineering. The same is true for `#manufacturing`, `#robotics`, `#technology`, and `#military`. It is also curious that the hashtag `#aerospaceengineering`, which seems to have the most appropriate name, ranks at only 5%. Issues like these have turned some aerospace marketers away from relying strongly on the use of hashtags for analysis towards the use of *deep learning* and *text embeddings*. This serves as a more robust form of categorization. It also allows the analyst to discover the meaning of social media documents at a more in-depth level. This is the approach taken by, for example, Ben-Lhachemi and Nfaoui (2018). Although they use this approach to recommend more optimal hashtags, the essence of the paper is about using deep learning with embeddings.

![]({{ site.baseurl }}/images/fig1_Top 10 Aerospace Hashtags.png "Figure 1: Top 10 Aerospace Hashtags")

## The use of Deep Learning and Embeddings

The concept of *embeddings* goes hand-in-hand with categorical variables. Individual words in an aerospace related social media document can be considered “values” or categories of a “text” variable. The analyst gets to choose the number of dimensions in semantic space along which the words will be placed. This means each word gets an *embedding vector* of N dimensions and is placed inside an N-dimensional *semantic space*. Figure 2 shows an example of word embeddings (albeit not aerospace words), visualized in a 2-dimensional semantic space. The clustering of words in this space becomes key in identifying, relating, and analyzing the nature of the text.  The usefulness of word embeddings was first described by Collobert and Weston (2008). 


![]({{ site.baseurl }}/images/fig2_Word embeddings in a semantic space.png "Figure 2: Example of word embeddings in a semantic space (visualized in 2 dimenstions)")

Ben-Lhachemi and Nfaoui (2018) realize that using word embeddings as such does not go far enough. The *combined* meaning of all the words in a tweet should somehow be captured in a single tweet embedding. The question is how to combine individual word embeddings. To address this, they made use of the work by Arora, Liang, and Ma (2017). This paper describes a simple but tough-to-beat technique to create *sentence embeddings*. In other words, it shows how to combine individual word embeddings and consolidate them into a single sentence embedding. Ben-Lhachemi and Nfaoui (2018) equated their collection of words (a tweet) to a sentence. Combining word embeddings was not invented by Arora et al. (2017). Similar approaches (that include the combination of word embeddings in terms of phrases, sentences, and even paragraphs) were described by Iyyer, Manjunatha, Boyd-Graber, and Daumé III (2015), Le and Mikolov (2014), Kiros et al. (2015), Socher, Huang, Pennin, Manning, and Ng (2011), Blunsom, Grefenstette, and Kalchbrenner (2014), Tai, Socher, and Manning (2015), and Wang et al. (2016).

The next step for aerospace marketers is to apply the technique described in Ben-Lhachemi and Nfaoui (2018), or described elsewhere in similar papers, to bolster the analysis abilities of their automated systems. 

### Calculate social document embeddings

The first step is to calculate the consolidated embedding of the complete social document, be it a tweet or otherwise. Any of the above-mentioned approaches are used by aerospace marketers to various extents and with varying degrees of success. 

### Place the social document in semantic space
Having the coordinates of the document’s *embedding vector*, allows the document to be placed in semantic space. This action informs how close the semantics of the document is to the semantics of established aerospace hashtags. It also reveals the proximity to centroids of company defined embedding vectors. 

### Compute the distance between the social document and all other relevant cluster centroids
By calculating the distance between the social document and all other relevant cluster centroids a determination can be made of where the document belongs. Company defined centroid clusters are usually most relevant in revealing where the document belongs. It usually works best to identify a ranked list of, say, the top 3 closest centroids. For outward engagement communication, it may be helpful to also add widely recognized hashtags used in the aerospace industry, for example, `#aerospaceengineering`. 

## Execution of social media marketing
Aerospace marketers often do not have the in-house expertise to perform the highly technical analyses referred to above. For this they tend to turn to outsourced solutions. Some of the bigger service providers are [Lexalytics](https://www.lexalytics.com/), Sales Force’s [Radian 6](https://socialstudio.radian6.com/), and [IBM Cloud](https://www.ibm.com/cloud). Sometimes marketers partner at a higher level, for example, [AviationBusinessConsultants.com](https://aviationbusinessconsultants.com/). 

There is also support from trade publications, for example, the paper in 2017 by Knoblich, Martin, Nash, and Stansbie that covers the German market, as well as the Seo and Park (2018) paper. The *Marketing Weekly News* article in 2018, “Studies in the Area of Air Transport Management Reported from Korea Aerospace University” looks at the effects of social marketing in the airline industry in Korea. 

In the end, it does not matter who does the in-depth technical analysis. What is important is how accurately incoming social media data can be analyzed and how accurately outgoing marketing type data can be focused on where it has the most impact.

## Advantages of social media marketing in the aerospace industry
A well-crafted social media marketing plan provides substantial advantages for the aerospace industry. By engaging high value audiences associated with virtual communities related to aerospace, companies that embrace these modern approaches experience significant benefits. It allows marketers to make serious business of engagement marketing and nurture marketing. This includes building long-term relationships as well as one-to-one relationships. 

In the case of engagement marketing the emphasis is on exceptional content and the aim is for marketing to go viral. The objective is to establish a social presence and it allows for relationships to be anonymous. Measurement of success rates are in the form of social metrics (e.g. likes, views, opens, click-throughs, etc.). In the case of nurture marketing, however, content impact is somewhat relaxed although it is required to be relevant. Marketing is now bi-directional and the objective is to establish sales relationships rather than to just have a social presence. At the same time, these relationships are not anonymous anymore but are of the nurture kind. Measurement of success rates are in the form of sales metrics (rather than social metrics).

One of the many success stories in applying social media marketing is the case of [Ansys](https://www.ansys.com/solutions/solutions-by-industry/aerospace) who specializes in advanced engineering simulation software used in the aerospace industry [https://sproutsocial.com/insights/case-studies/ansys/](https://sproutsocial.com/insights/case-studies/). The social engagement of Ansys keeps growing at a 19% year-over-year rate. Against a mostly manufacturing background that sprang from the industrial age, it is encouraging to notice the gradual adoption of social media marketing by aerospace marketers. They may not be as agile as marketers in the food industry, or the retail industry, but they are awakening to the advantages of social media marketing.

## References

Engineering 360 (2019). Retrieved June 17, 2019, from [https://www.globalspec.com/](https://www.globalspec.com/)

Wilinsky, D. (2014, September). IHS Introduces Engineering360, the World’s Largest Online
Destination for Engineers. Retrieved from [https://www.businesswire.com/news/home/20140925005599/en/IHS-Introduces-Engineering360-the-World%E2%80%99s-Largest-Online-Destination-for-Engineers](https://www.businesswire.com/news/home/20140925005599/en/IHS-Introduces-Engineering360-the-World%E2%80%99s-Largest-Online-Destination-for-Engineers) 

5 Online Communities About the Aviation Industry You Should Join. [http://www.aviationmaintenance.edu/blog/aviation-industry/5-online-communities-aviation-industry-join/](https://aviationmaintenance.edu/2014/05/21/5-online-communities-aviation-industry-join/)

15 Aerospace Industry Professionals You Should Be Following on Social Media. [https://www.cuttingdynamics.com/industry-professionals-you-should-follow-on-social-media/](https://www.cuttingdynamics.com/industry-professionals-you-should-follow-on-social-media/)

Knoblich, S., Martin, A., Nash, R., & Stansbie, P. (2017). Keys to success in Social Media Marketing (SMM) – Prospects for the German airline industry. *Tourism and Hospitality Research*, 17(2), 147–164. https://doi.org/10.1177/1467358415610415

Ben-Lhachemi, N. & Nfaoui, E. (2018). Using Tweets Embeddings For Hashtag Recommendation in Twitter. *Procedia Computer Science*, 127(2018), 7–15.

Collobert, R. & Weston, J. (2008). A unified architecture for natural language processing: Deep neural networks with multitask learning.  In *Proceedings of the 25th International Conference on Machine Learning*, Helsinki, Finland, 2008.

Arora, S. Liang, Y., Ma, T. (2017). A SIMPLE BUT TOUGH-TO-BEAT BASELINE FOR SENTENCE EMBEDDINGS. *Submitted to ICLR 2017 conference*. 

Iyyer, M., Manjunatha V., Boyd-Graber, J., Daumé, H. III. (2015). Deep unordered compositionrivals syntactic methods for text classification. *Proceedings of the Association forComputational Linguistics*, 2015.

Le, Q. & Mikolov, T. Distributed representations of sentences and documents. In *Proceedings of The 31st International Conference on Machine Learning*, 2014.

Kiros, R., Zhu, Y, Salakhutdinov, R., Zemel, R., Urtasun, R, Torralba, A., Fidler, S. Skip-thought vectors. In *Advances in neural information processing systems*, 2015.

Socher, R., Huang, E. H., Pennin, J., Manning, C. D., Ng, A. Y. Dynamic pooling and unfolding recursive autoencoders for paraphrase detection. In *Advances in Neural Information Processing Systems*, 2011.

Blunsom, P., Grefenstette, E., Kalchbrenner, N. A convolutional neural network for modelling sentences. In *Proceedings of the 52nd Annual Meeting of the Association for Computational Linguistics*, 2014.

Tai, K. S., Socher, R., Manning, C. D. Improved semantic representations from tree-structured long short-term memory networks. *arXiv preprint arXiv:1503.00075*, 2015.

Wang, Y., Huang, H., Feng, C., Zhou, Q., Gu, J., Gao, X. Cse: Conceptual sentence embeddings based on attention model. In *Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)*, 2016.

Lexalytics.com: [https://www.lexalytics.com/](https://www.lexalytics.com/)

Salesforce Radian6: [https://socialstudio.radian6.com](https://socialstudio.radian6.com/)

IBM Cloud: [https://www.ibm.com/cloud/](https://www.ibm.com/cloud)

AviationBusinessConsultants.com: [https://aviationbusinessconsultants.com](https://aviationbusinessconsultants.com/)

Ansys: [https://www.ansys.com/solutions/solutions-by-industry/aerospace-and-defense](https://www.ansys.com/solutions/solutions-by-industry/aerospace)

Sprout Social CASE STUDIES: How Simply Measured Continues to Help ANSYS Grow Their Social Engagement by 19% Year-Over-Year. [https://sproutsocial.com/insights/case-studies/ansys/](https://sproutsocial.com/insights/case-studies/)

Seo & Park (2018). A Study on the Effects of Social Media Marketing Activities on Brand Equity and Customer Response in the Airline Industry. *Journal of Air Transport Management 66* (2018): 36-41. Web.

Studies in the Area of Air Transport Management Reported from Korea Aerospace University. *Marketing Weekly News* (2018): 66. Web.





