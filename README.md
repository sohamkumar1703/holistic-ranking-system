## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Dataset info](#dataset-info)
* [Proposed Methodology](#proposed-methodology)

## General info
The work proposes a collective, holistic ranking system for countries based on various factors, such as economic freedom, environmental sustainability, and human well-being. While individual country rankings based on factors such as GDP, education, and healthcare are common, they lack a comprehensive world ranking system. Moreover, the classification of countries into developed, developing, and underdeveloped categories can be subjective and inaccurate. Three world indexes - the Human Development Index (HDI), the Social Progress Index (SPI), and the Innovation Index (II) were selected as reference datasets. The data was reduced performing principal component analysis and merged to create a new dataset. The missing score were predicted using CART and various clustering techniques were explored to best categorize the regions. Independent component analysis was performed on the final dataset and visualizations were made based on the resulting clusters. The proposed system also has the potential to improve international relations and facilitate significant decision-making.
	
## Technologies
Project is created with:
* RStudio version: 2022.07.2+576
* R version: 4.2.2

## Dataset info
Data is collected from:
* United Nations Development Programme (UNDP). (2021). Human Development Indices and Indicators: 2021 Statistical Update.
* Social Progress Imperative. (2021). 2021 Social Progress Index.
* World Intellectual Property Organization .(2021) Global Innovation Index.




