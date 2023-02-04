#Final Project Proposal


## Project title
Wealth Inequalities Affecting Pet Ownership in the Seattle-Area

### Authors
Paulina Fronckiewicz - pfron@uw.edu 
<br />
Veronica Fula - vfula@uw.edu 
<br />
Riley Baerg - rbaerg@uw.edu 
<br />
Wenxuan Dong - wenxud@uw.edu 

### Date

Winter 2023

## Abstract

Our main question is “does median household income affect the species, breed, and number of pets”? To address this concern, we will combine data from the US Census on median household income and from the City of Seattle on the number of pet licenses issued and  look at the species and breed columns. This is important because this can reflect social and wealth inequalities in our society and show trends over time that can tell us more about how events like COVID affected people at a personal level.

## Keywords

- **Primary Breed:** general breed makeup of species; majority breed; dominant genetics of animal species that fall into the category of a breed. 

- **Secondary Breed:** further descending breed than primary breed; less dominant genes that contribute less to animal species overall makeup. 

- **Species: animal-type:** dataset includes the following animal species in its pet licensing data: dog, cat, pig, goat. 

- **Median household income:** helps to understand how the economic situations of people in Seattle 

- **Zipcodes:** used to combine the two datasets and look at the geographical distribution of pet ownerhip and median income of each household with licensed pets.

<br />

## Proposal

### 1. Introduction  

The project centers around a dataset of pet licenses issued by the City of Seattle from January 24, 2017, to January 25, 2023. We also would like to combine this set with data on median household income, to see how income influences the type of pet they have, and what breed of pet. Another question would be to infer whether a pet is adopted or pure-bred based on the breed, and see how many there are in each zip code. We are motivated by the questions of how wealth affects the kinds of pets people own, since pets are an integral part of our society and the well-being of many people. They seem to be ubiquitous, so it would be interesting to see if income is reflected in their demographics, or if people simply have pets according to convenience or without regard to pedigree. This can also show how trends in pet ownership change over time and how events like COVID-19 and quarantine affected people economically. Quarantine affected what kinds of jobs people had, so that can affect maybe the species that they can take care of (pigs and goats might be more difficult since they need space, money and specialized vets to take care of them).

<br />

### 2. Related Work  

Some related work includes a survey done from 2020 to 2022 about various pet-related questions, such as whether they got a new pet in that year, if people spent more time with their pets due to COVID lockdown, and how worried they were about pet expenses. They also took age or generational data. They report that Millennials and Gen Z were more likely to be worried about pet-related expenses than Baby Boomers during the pandemic in 2020. The report attributes this to the pandemic impacted the economic situation of millions of people in the US, especially those with part-time or unguaranteed work. They also note that more people got pets in 2022 than in 2020 (14% vs 10%, respectively). This can potentially signify that the economic situation is improving and/or that people are in more need of companionship thanks to lockdown. This study shows that a link exists between economic factors and pet ownership and also that age can be another factor influencing our investigation that is not represented in our dataset.
<br />
Bureau, U. S. C. (2021). INCOME IN THE PAST 12 MONTHS (IN 2021 INFLATION-ADJUSTED DOLLARS). Explore census data. Retrieved February 3, 2023, from https://data.census.gov/table?q=median%2Bincome&g=0400000US53%248600000 

Seattle, C. of. (2023, January 25). Seattle Pet Licenses: City of seattle open data portal. Seattle Open Data. Retrieved February 3, 2023, from https://data.seattle.gov/Community/Seattle-Pet-Licenses/jguv-t9rb 

Statista (2022). How COVID-19 affected pet ownership in the U.S. 2020-2022 [Dataset]. Retrieved February 3, 2023, from https://www.statista.com/statistics/1191395/pet-ownership-status-due-to-covid-19-in-the-us/

<br />

### 3. The Dataset

**Dataset 1: Seattle Pet Licenses**
- The data was found on Seattle Open Data Website: https://data.seattle.gov/Community/Seattle-Pet-Licenses/jguv-t9rb 

- Dataset Owner - Arlene Ehrlich, Provided by: City of Seattle.

- This data is documented by shelters and pet stores to track on their end the transactions of animals to the public. Animals must be lawfully licensed, and therefore those records are traced to hold someone accountable for the animal. 

- Collection of this data began due to lawful order from the Department of Finance and Administrative Services to citizens to license all cats, dogs, goats, and pigs. 

- 43.9K Observations as of January 25, 2023. 

- 7 Columns: License Issue Data, License Number, Animal’s Name, Species, Primary Breed, Secondary Breed, ZIP Code.

- To analyze this data we must consider income inequalities and the greater impact on the Seattle area. Purchasing and caring for a pet requires a significant amount of money to take care of. Some households can afford to care for multiple expensive purebred animals while some can barely afford to feed an animal saved from a shelter. How does income factor in on pet ownership and owner density in the Seattle area? Is there a preferred breed or animal based on income bracket and area code? 

- The Seattle Pet Licensing dataset includes only four animals in the data frame due to the Department of Finance and Administrative Services only requiring licensing on those four animal-types. Obviously there are more than four animals that could possibly be considered as pets, and the animals that do not fit into that category could be either much more or much less expensive to take care of (outliers). First, take fish as an example: one measly goldfish does not require much space, time, effort, or money to take care of -- a single fish bowl, maybe some decorations, and some fish pellets. Now consider a snake, it is considered proper to feed them live prey in order to train them (a reward system, and a means of training the snake not to bite humans) -- just one snake may require hundreds a month! Another limitation is that the dataset does not include a Boolean column depicting if the animal is purebred or not. This is not an unsolvable problem, but knowing if the animal was purebred or not could provide more information on income inequalities. One last problem that this data set overlooks is the issue of unlicensed pet ownership. Even today people insist on selling pets under the table for discount prices so it goes without saying that criminally selling pets will be overlooked by this dataset.

<br />

**Dataset 2: Median household income in Washington by zipcode**
- The data was found on data.census.gov website:
https://data.census.gov/table?q=median+income&g=0400000US53$8600000 
It was filtered to include median income data for zip codes in Washington by using the following guide found on Reddit:
https://www.reddit.com/r/datasets/comments/hixfeo/how_to_obtain_median_income_data_for_zip_codes/ 

- The data was collected by the United States Census Bureau which is a principal agency of the U.S. Federal Statistical System (Source: U.S. Census Bureau, 2021 American Community Survey 1-Year Estimates)

- The American Community Survey (ACS) produced population, demographic and housing unit estimates, but the Census Bureau's Population Estimates Program produced and disseminated the official estimates of the population for the nation, states, counties, cities, and towns and estimates of housing units for states and counties. Data are collected from respondents directly (including businesses), through the censuses and surveys.

- The data was collected to generate regular and in-depth statistics about the country. This information is essential for the development of government initiatives, regulations, and decision-making processes.

- There are 607 observations (rows).

- There are 259 features (columns).

- When working with this data it is important to consider privacy concerns such as if the personal information collected through the census is protected and kept confidential. Furthermore, it is crucial to consider if there is a risk of biased data collection and analysis which could lead to unequal representation or discrimination of certain groups, as well as, if the representation and accuracy is sufficient

- Although census data is a reliable source of information, it can include some limitations and problems. Firstly, the census can be a subject to undercounting certain populations, such as homeless individuals, immigrants, and people from marginalized communities, which could result in inaccurate representation of the population. Secondly, the quality of the data can be influenced by factors such as response error, data processing errors or measurement inaccuracies. Lastly, the non-response bias could impact the reliability of the data by providing an inaccurate representation of the population.
 

<br />

### 4. Implications

Our analysis and final product could help educate people on the relationship between income and the type of pet, and more specifically, its breed. For policymakers, this project could bring about a better understanding of the economical condition of those who raise one or more pets and thus make more effective policies for Seattle, or specifically its local pet industry and pet owners as well as revise existing policies with defects. The project may also bring attention to the financial condition of those with moderate or low-incomes and a need for emotional support. For technologists and designers, the program helps them when they are formulating or workshopping products. For example, an urban planner may want to know the income of one area of people who breed a pet when planning the city. A technologist or a designer may consult the project when they are designing a product geared towards pet owners that are at a specific income level or adding a new function to an existing product.

<br />

### 5. Limitations & Challenges

What challenges or limitations might you need to address with your project idea? Briefly discuss (at least 150 words) 
We pick the data of pet licenses and the pet owner information from the state government and there might be some pets not registered in Seattle. So the data has limitations in showing the type and number of the pet. Also, the license needs to renew for a certain period. So we can not know if the person changes pet or loses a pet, so the data is not so up-to-date in short term. Also, we pick two datasets, one is about pets and another is about the income of people. Mixing those two datasets and analyze accurately together is a challenge. We also plan to create a 2D data visualization on our website to show the data. Changing those data and processing them into charts and pictures on a website needs a huge amount of code and knowledge of coding more than we learned in this course. This could be a challenging task for us.

<br />

#### Acknowledgements
We would like to thank Seattle Open Data Library for providing this data set and the author of the Seattle Pet Licenses Data Frame, Arlene Ehrlich. Without this library open to the public we would likely be struggling with finding such a wide range of data over the past half decade. We confirm and acknowledge that this data is accurate and up to date; as it is written under law, it is a legal obligation of pet owners of the Seattle area to license their pet. Finally we would like to thank the pets that appeared in this dataset, we could not have done it without you. 
