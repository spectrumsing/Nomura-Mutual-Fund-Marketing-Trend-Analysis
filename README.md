# Course Project: Increasing Sales Conversion Rate by Applying Trending Topic and Words
This is the final project for the course <a href="http://coursemap.aca.ntu.edu.tw/course_map_all/course.php?code=723+M9900" target="_blank">Fin7067: Fintech-Text Mining and Machine Learning</a> at National Taiwan University. Our group collaborated with <a href="https://www.nomurafunds.com.tw/Web/Content/#/index" target="_blank">Nomura Asset Management Taiwan</a> to explore ways to improve marketing ROI.  

## Introduction
The current common practice of asset managers is to follow the traditional Top-Down marketing process, starting with determining which product to promote, then analyze the target audience, select the marketing channel, and finally plan out the promotion. However, in the age of digitalization, the Bottom-Up approach could prove beneficial. It may be used to explore popular investment topics and key words, reversely develop marketing strategies, and even deliberately include specific keywords in advertising materials.

Our goal is to discover and summarize popular words to accurately grasp the trending topics among investors, increase sales conversion rate, and eventually improve marketing ROI.

## Design Process
We first scrapped content from online forums(<a href="https://forum.fundhot.com/" target="_blank">Fundhot</a>, <a href="https://www.ptt.cc/bbs/Fund/index.html" target="_blank">PTT Fund</a>), news outlets(<a href="https://www.businesstoday.com.tw/" target="_blank">Business Today</a>, <a href="https://www.businessweekly.com.tw/" target="_blank">Business Weekly</a>, <a href="https://www.cnyes.com/" target="_blank">Anue</a>, <a href="https://www.gvm.com.tw/" target="_blank">Global Views Magazine</a>), and industry peers(<a href="https://tw.allianzgi.com/zh-tw" target="_blank">Allianz Global Investors Taiwan</a>), then parsed it using Beautiful Soup, and subsequently segmented the text with <a href="https://github.com/fxsjy/jieba#jieba-1" target="_blank">Jieba</a>.

We opt for Latent Dirichlet Allocation(LDA) as the topic modeling method and used <a href="https://github.com/bmabey/pyLDAvis" target="_blank">pyLDAvis</a> to visualize the fitted LDA topic model to help us interpret the topics.

Finally, the categorized data were presented as an interactive stacked bar chart. It could be used in conjunction with the keywords identified with the LDA model to give the marketing team a better understanding of the market trends.

See 'Visuals' folder for the graph as well as the visualized LDA model.
