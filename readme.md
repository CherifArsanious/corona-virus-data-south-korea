# Covid-19 (Corona Virus) dataset collected by South Korea-shared on Kaggle website
## by Cherif Arsanious


## Dataset
From World Health Organization - On 31 December 2019, WHO was alerted to several cases of pneumonia in Wuhan City, Hubei Province of China. The virus did not match any other known virus. This raised concern because when a virus is new, we do not know how it affects people.

So daily level information on the affected people can give some interesting insights when it is made available to the broader data science community.

2019 Novel Coronavirus (2019-nCoV) is a virus (more specifically, a coronavirus) identified as the cause of an outbreak of respiratory illness first detected in Wuhan, China. Early on, many of the patients in the outbreak in Wuhan, China reportedly had some link to a large seafood and animal market, suggesting animal-to-person spread. However, a growing number of patients reportedly have not had exposure to animal markets, indicating person-to-person spread is occurring. At this time, it’s unclear how easily or sustainably this virus is spreading between people - CDC

COVID-19 has infected more than 8000 people in South Korea.
KCDC (Korea Centers for Disease Control & Prevention) announces the information of COVID-19 quickly and transparently.
Kaggle website made a structured dataset based on the report materials of KCDC and local governments.
Also, we analyze and visualize the data using various data mining or visualization techniques.

link to Kaggle dataset https://www.kaggle.com/kimjihoo/coronavirusdataset

## Summary of Findings

> The number of female infected by the coronavirus is higher than the number of male infected. From the data gathered, 53.9% of patients were females where 41.8% where males

> by plotting age distribution of patients through a bar chart, I noticed it is quiet interesting, because the media was propaganding that youth are almost protected from infection but the data of South Korea is showing other wise. The higher patient age ratio infected were the 20s with 21% of the whole patients, the second age range is the 50s with 17.6%. The myth that kids are among the least infected is still valid here with only 3.4% of the patients.

> The plot distribuation of deceased ages implies that also the age range 20s where infected the highest but the mortality rate is 0%. More than 60% of deceased patients where older than their 40s.

> The majority of patients contacted between 10 and 25 persons before being diagnosed with the coronavirus, and that probably explains why it is has a wide spread and transmission, specially the virus has an incubation period of 14 days.

> The province with the highest number of infections is Gyeonigsangbuk-do with more than 1000 cases which represent about 47% of cases in South Korea

> from inspecting sex and age variables by clustered barchart and heatmapping, the people in their 20s are still the highest in getting infectied by the coronavirus wether female or male, and after them are people in their 50s as as noted before in the univariate exploaration of sex, female are more suceptible to get infected in almost every age ranges except in young patients below 20s where more male patients than female patients. 

> By visual inspecting both the state variable and the age range variable through clustered bar chart and heat mapping, it appears that although the people in their 20s were the  highest in getting infected but it appears here that they recorded zero deathes and patinets under 30s in general did not record any death in this dataset, and all the deathes occured for people above 30s with the majority hapening for patients between 50s till 80s. 

> by visual inspecting the two categorical variable sex and state, i notice that although female being more suceptible to get infected but here it appears that the deathes in female is lower than in males and that female are faster to be released and so they are healing faster.

> from inspecting the contact number variable with age variable by faceting, it becomes apparant that one possible cause that the 20s has the hishgest infection proportion is that they widest and highest histogram spread which means that the people in their 20s come in contact with many people so they most susceptible to get infected and same wise they are also most risk to spread the virus to many people before manifesting symptoms of virus or being diagnosed positive in the coronavirus test.

> All Observations made here are merly visual observations made through the different plottings that actually require more in depth analysis and more availability of big data and model building before confirming any of them. 
By plotting pair grid of several numerical variables (['nb_of_patients', 'avg_temp', 'max_wind_speed','avg_relative_humidity','elementary_school_count', 'kindergarten_count', 'university_count',
'elderly_population_ratio','nursing_home_count']), several observations are made:

* There is a weak positive pearson correlation between the number of kindergarten, schools in any province and the number of coronavirus patients. In the case of count of universities, the relation is moderate positive with a value of 0.51. This could be due to the high density of these places and that makes sense why most countries closed the premissies of their schools and universities. We see earlier on previous visualizations that 20s age  people are most susceptible to get infected by coronavirus and that observation here comes to support the previous observation so provinces with high number of active universities will have higher risk of having higher number of patients.

* there is a weak negative relationship between the average temperature and humidity on one hand and the number of patients on the other hand in the provinces. This could weakly suggest the assumption that the Covid 19 does not spread highly in high temperatured humid regions. The previous known strains of coronaviruses were weak in high temperatures but we still don't enough information to sustain that in the new Covid-19. Some researchers are already investigating the temperature effect https://www.accuweather.com/en/health-wellness/higher-temperatures-affect-survival-of-new-coronavirus-pathologist-says/700800

* There is a weak positive pearson correltion between the ratio of elderly in the province and the number of its coronavirus patients. We see eralier on previous visualization that elderly people are highly susceptible to get infected by coronavirus and that observation here comes to support the previous pbservation so provinces with high elederly ratio will have higher risk of having higher number of patients.

> by investigating the age, sex and contact variables together by a facet grid using boxplot, I noticed that in age ranges (20s, 30s, 40s, 50s) male gender has more contact than female gender. In other age ranges they pretty similar. This observation may suggest that male in different age ranges contact more people than female before being diagnosed with coronavirus. This fact may be due to the gender inequality issue in South Korea where men have higher proportions in education enviroment and work enviroment. https://en.wikipedia.org/wiki/Gender_inequality_in_South_Korea 

> by plotting provinces, age ranges and contacted people together through FacetGrid, I noticed that in general the provinces that has the highest number of patients has also the highest distribution in contact number and highest contact number.  

## Key Insights for Presentation

> I tried to add all the titles and labels and unify sizes and color palettes among all visualizations so in the presentaion slide deck i only chose what visualization to show but the polishing was also done in the exploration step