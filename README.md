## Developing a Holistic Ranking System using Global Indexes


## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Dataset info](#dataset-info)
* [Proposed Methodology](#proposed-methodology)
* [Results](#results)
* [Conclusion](#conclusion)

## General info
The work proposes a collective, holistic ranking system for countries based on various factors, such as economic freedom, environmental sustainability, and human well-being. While individual country rankings based on factors such as GDP, education, and healthcare are common, they lack a comprehensive world ranking system. Moreover, the classification of countries into developed, developing, and underdeveloped categories can be subjective and inaccurate. Three world indexes - the Human Development Index (HDI), the Social Progress Index (SPI), and the Innovation Index (II) were selected as reference datasets. The data was preprocessed to make the country names uniform, scaled and reduced performing principal component analysis and merged to create a new dataset. The missing score were predicted using CART, Predicitive Mean Matching and Regrssion.The final data was reduced to two independent components and clustering techniques were explored to best categorize the regions based on those components. Visualizations were made based on the resulting clusters. The proposed system also has the potential to improve international relations and facilitate significant decision-making.
	
## Technologies
Project is created with:
* RStudio version: 2022.07.2+576
* R version: 4.2.2

## Dataset info
Data is collected from:
* United Nations Development Programme (UNDP). (2021). Human Development Indices and Indicators: 2021 Statistical Update.
* Social Progress Imperative. (2021). 2021 Social Progress Index.
* World Intellectual Property Organization .(2021) Global Innovation Index.

## Proposed Methodolgy

![Proposed_Methodology](https://github.com/sohamkumar1703/holistic-ranking-system/assets/71141510/efdaa5ec-a17a-4c64-aea0-94cbf338176d)

Detailed explanation is given in [Report.pdf](https://github.com/sohamkumar1703/holistic-ranking-system/Report.pdf) under **Proposed Metholodogy** section.

## Results

The performaces of various clustering methods on our dataset is shown as below:

![Clustering_method_performance](https://github.com/sohamkumar1703/holistic-ranking-system/assets/71141510/9d80071e-5cd6-4b6e-a38c-f4a1f43cf9b7)

The best silhuoutte score was obtained for 3 clusters. A world plot mapping each country in the dataset to their deirved cluster is shown as below.
![World_Plot](https://github.com/sohamkumar1703/holistic-ranking-system/assets/71141510/0145bba6-ac9d-43aa-8fb0-867984c302ff)

More results can be seen in [Results](https://github.com/sohamkumar1703/holistic-ranking-system/Results) folder with interpretation in [Report.pdf](https://github.com/sohamkumar1703/holistic-ranking-system/Report.pdf) under **Results and Discussion** section.

## Conclusion
The proposed work has successfully ranked countries based on their Social Progress Score, Human Development Score, and Global Innovation Score. Finally, we categorized the countries into three clusters, with a silhouette score of 0.48. Based on our observations, North America, Australia, New Zealand, Japan, South Korea, Europe, and Chile fall under category 3, which shows a higher band of scores and are marked as developed countries. Countries like India, China, South Sudan, Republic of Congo, and Central African Republic fall into category 2, which falls into the moderate score
band and are marked as developing countries. Regions like most of Africa, South America, Central Asia, and Southeast Asia fall into the lowest score band and are marked as poor-performing countries. K – means, K – medoid and Fuzzy clustering provides promising results for clustering in such scenarios. Dimensionality reduction and factor analysis is very crucial for extracting the most important factors which affects the country’s category. However further work can be done by including more indexes for comparison. The results will vary each year so the source datasets need to be updated every year and fed into the system to get the new resuts.
