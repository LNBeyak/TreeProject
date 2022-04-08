# TreeProject
CSC 485/685 - Data Visualization Final Project Proposal

Initial Sketches

[Sheet1.pdf](https://github.com/LNBeyak/TreeProject/files/8328899/Sheet1.pdf)

[Project 4.pdf](https://github.com/LNBeyak/TreeProject/files/8328712/Project.4.pdf)

Domain & Data

This project aims to visualize a relationship between the tree population or coverage within certain cities and other variables related to quality of life such as income or life expectancy. We are interested in learning whether there is visual evidence of this relationship and how the amount of trees may add to the quality of life for those who live in the regions we survey. 
A few different datasets are being explored to illustrate the goal of the project. The following is a description of each dataset:

Health Equity Report: District of Columbia 2018 - The Health Equity Report for DC was released in 2018 as a reference measure of the social and structural determinants of health reported in the district. It provides data related to healthcare, transportation, housing, income, employment, education, outdoor environment, and more. 
[HER Report FINAL_with letter and table_02_08_2019.pdf](https://github.com/LNBeyak/TreeProject/files/8328785/HER.Report.FINAL_with.letter.and.table_02_08_2019.pdf)

Open Data DC – In order to reference the appropriate shape for the DC neighbourhoods, we are using the Open Data DC reference to best navigate the district and ensure it is portrayed correctly in the project visuals. It includes the mapped area of the neighbourhoods along with the datasets provided on the website. 
(https://opendata.dc.gov/datasets/DCGIS::dc-health-planning-neighborhoods/explore?location=38.890622%2C-77.022347%2C12.56)
(https://opendata.dc.gov/datasets/DCGIS::dc-health-planning-neighborhoods-to-census-tracts/explore)

Data Census – To explore other cities, the Data Census Bureau website is being referenced provide dataset on income, and other life expectancy related information. 
(https://data.census.gov/cedsci/advanced)

USDA Forest Coverage Datasets – Data collected by the USDA Forest Service programs is available as a map service to show the active forest coverage around the USA. These are used in the visuals for the density and tree population on a national level.
(https://data.fs.usda.gov/geodata/rastergateway/treecanopycover/)

The World Bank Forest Area - This dataset provides data collected globally in relation to forest area coverage. Although some countries are limited and vary between what years have been collected, we are focusing on the timelines with the most data to review and at least provide a visual of any changes throughout the records. 
(https://data.worldbank.org/indicator/AG.LND.FRST.ZS)

Related Work

Much of the work that relates to this project concerns “tree equity”. This term essentially means equal community tree canopy, which is related to societal and environmental benefits. A lot of the related work has to do with the discovery of tree inequity and how tree prevalence varies with different factors, like income and life expectancy.
A conservation group called American Forests claims to have coined the term “tree equity” and created a Tree Equity Score. They made several discoveries on the factors that have relationships with trees: surface temperature, income, employment, race, age and health. These discoveries then build the tree equity score. American Forests has done a lot of work to prove the relationships between tree prevalence and these factors (American Forests, n.d.).
This article from Live Science talks about observations made from a study published in the journal Environmental Health Perspectives. In this study, they researched how vegetation around homes influences womens’ life expectancy and contraction of different diseases. They discovered that women with more greenness near their homes had a 12% lower death rate, as well as “41 percent lower death rate from kidney disease, a 34 percent lower death rate from respiratory disease and a 13 percent lower death rate from cancer” (Rettner, 2016).
There are also many studies on the relationship between trees, particularly in urban areas, and climate change. Climate change and other environmental factors can influence social factors like income and life expectancy, so mitigating climate change through trees should also mitigate the associated social concerns. A USDA and US Forest Service article on Urban Forests and Climate Change dives into the importance of restoring forests, particularly vegetation in urban areas, to combat many of the issues associated with climate change (Safford et al., 2013).

Sources
American Forests. (n.d.). Tree Equity Score. American Forests. Retrieved from https://www.americanforests.org/tools-research-reports-and-guides/tree-equity-score/
Rettner, R. (April 19, 2016). How the Plants Around Your Home May Affect Your Life Span. Live Science. Retrieved from https://www.livescience.com/54463-vegetation-mortality.html
Safford, H., Larry, E., McPherson, E.G., Nowak, D.J., and Westphal, L.M.. (August 2013). Urban Forests and Climate Change. U.S. Department of Agriculture, Forest Service, Climate Change Resource Center. Retrieved from www.fs.usda.gov/ccrc/topics/urban-forests 

Project Staus Update - April 7, 2022

Visualization 1 – Bubble Chart:
<img width="452" alt="image" src="https://user-images.githubusercontent.com/34941328/162500767-51a31e21-18d7-4730-9aa4-e438b23ea841.png">

Visualization 2 – Scatter Chart:

<img width="452" alt="image" src="https://user-images.githubusercontent.com/34941328/162501041-a0b73b30-e952-4b4b-bc11-74d872493a80.png">

Visualization 3 – Slope Chart:

<img width="452" alt="image" src="https://user-images.githubusercontent.com/34941328/162501087-81d8f3c8-3203-483d-ac55-17d5e56a1a40.png">

Visualization 4 – Tree Map:

<img width="452" alt="image" src="https://user-images.githubusercontent.com/34941328/162501219-43e40512-f6fc-4e29-bf5a-a924897fb661.png">


Modifications:
Overall, our implementation so far aligns well with our proposal. We have started the implementation of visualizations 2-5 of the design sheet 5. As visualization 1 will combine elements of both the choropleth map and the tree map, we decided to implement it only after we have finished the initial implementations of these two visualisations. In our initial design, the map directly plotting trees was a small multiples visualization showing how the number of trees decreased over time. When plotting this visualization, however, we found that the decrease is difficult to spot in a small multiples format. When enabling users to switch between years, however, the decrease is more apparent. In the observable notebook accompanying this status update, we included both versions. However, currently we are leaning more towards the user input (not small multiple) version of this visualization for the final product.

Libraries/Software:
So far, we are using observable input objects to get interactive user input. These are easy to use, but not as customizable as they would be if we implemented buttons and other input elements ourselves. For some of the geographic data wrangling, we used ArcGIS. We also used it to make the map directly plot trees. For data cleaning and managing of non-geographic data, we used R and Excel. Other than this, we mainly used D3.
Implementation Approach:
Our initial implementation approach was to divide the individual visualizations up so that everyone is responsible for one visualization. However, we also organized a working session in which we worked on the project and helped each other. This approach has worked well so far, and thus we want to keep the division of responsibilities.

Features and Schedule:
We are slightly ahead of schedule, as we did not expect to be able to add any interactivity this early. Because of this, we are debating whether to move from observable to building a regular website once we finished our visualizations. We are hoping that this would give us the ability to further customize the final design of the project. However, we have not decided if we want to move in this direction yet.


Link to Observable:
https://observablehq.com/@efa8bf212e62395b/distreebution
