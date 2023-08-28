# Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection
More details see https://janzhuj.github.io//Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/

Did you know that the United States spends over $4 trillion annually on healthcare? Unfortunately, between 3% and 10% of this spending is lost to abuse, waste, and fraud. As I researched healthcare claims data, I discovered the staggering amount spent on prescription drug claims each year. There is a crisis of drug abuse and fraud, particularly with labeled drugs such as opioids, antibiotics, long-acting opioids, and antipsychotics for the elderly. This is a serious issue that not only hurts the health and well-being of individuals and society but also leads to higher costs for care and exorbitant financial losses for individuals and organizations.

When our aim is to identify suspicious claims, we face a problem: there is an overwhelming amount of healthcare data. It’s like finding a needle in a haystack. What we can do is to conduct claim segmentation and then identify suspicious claims. This way, we reduce the size of the search pool, cluster similar claims into groups, and make the anomaly detection task easier.

Here is an overview of overall Medicare Part D Prescibers scenario in the US. We can see the number of providers in each state in 2021, and the claims percentage by drug label, brand, insurance plan, and subsidy. We can also easily identify the specialty with the most providers, claims, and costs. In addition, we have a histogram to show us the average health condition of bentificiaries.

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/2d52fb9b-386f-46ed-9271-b3606144867d)

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/18730a96-679a-41da-899c-bafccecdbac3)

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/b8ca863f-73af-46d2-b641-1351374e46d5)

I applied k-means clustering to partition claim data into k clusters in which each observation belonged to the cluster with the nearest centroid, and used KElbowVisualizer to identify optimum number of clusters. As shown in below, I decided that 6 is the optimum number of clusters.

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/59efd82d-ce94-420f-b58d-368c7f68b399)

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/46fb33a8-8dd1-42e6-a8d6-ffa12bed2070)

Mothed 1： direct method using scatter plot.

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/4fd1ca8e-69b5-4e6d-bf10-ad63a6884260)

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/1fd663ee-520e-49c9-b4fd-657bf4b51d7b)

Method 2: Unsupervised Anomaly Detection

![image](https://github.com/Janzhuj/Medicare-Part-D-Claims-Segmentation-and-Anomaly-Detection/assets/99841253/0cf125d6-8a84-4ffd-ad51-e513064e02fe)
