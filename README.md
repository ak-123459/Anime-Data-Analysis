<img src="https://i.ibb.co/vYPNmCb/banner-github-png.png" alt="banner-github-png" width="2000" border="0">


<br></br>

from recent years anime gain popularity between people in various type movies,[ova(Original video animation)](https://en.m.wikipedia.org/wiki/Original_video_animation)   ,[ona(Original net animation)](https://en.m.wikipedia.org/wiki/Original_net_animation) etc.the aim of this projects using anlytics skills visualize the trends and patterns from previous released anime dataset to know future trends.



***

 <div align= "start">
  
  &nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/Ksw7GWz/list.png" width="50" alt="list" border="0"></a> <div/>

  <div align= "start">
  
- ## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Prerequisites](#Prerequisites)
4. [Project Structure](#Project-Structure)
5. [Methodology](#Methodlogy)
6. [Data Visualisation](#Data-Visualisation)
7. [Key Findings](#KeyFindings)
8. [Recommendations](#Recommendations)
9. [Conclusion](#Conclusion)
10. [Contributors](#Contributors)

 <div/>






***


<div align= "start">
 
  &nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/x2mBdn3/file.png"  width="50" alt="file" border="0"></a> <div/>
  
<div align= "start">


 
- ## **Project Overview**
[**Anime**](https://en.wikipedia.org/wiki/Anime#:~:text=Anime%20is%20distributed%20theatrically%2C%20through%20television%20broadcasts%2C%20directly,numerous%20genres%20targeting%20various%20broad%20and%20niche%20audiences), As a type of animation, anime is an art form that comprises many genres found in other mediums; it is sometimes mistakenly classified as a genre itself.[8] In Japanese, the term anime is used to refer to all animated works, regardless of style or origin.there are many anime-series-produce  during past years that are more expensive  like Dragon Ball Super  (2017 - Present) and this anime cost are $170,000(1,43,57,010 Indian Rupee) Per Episode,to know more go throw the link [*top most expensive anime produced*](https://screenrant.com/most-expensive-anime-series-produce-how-much/) .so we can imagine the budget of the anime. so in this project our aim was to understand the trends of previous years released anime,top most rank anime,most rated anime and why they are most popular?,top most producing anime studios,what type of content in anime the peples wants to to see .at the end of all analysis I have suggested some [Recommendations](#Recommendations) that  we have find from  insights for better decision making.

 <div/>

 
<br></br>






***


<div align= "start">
&nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/D9vKsxH/dataset.png" alt="dataset" border="0"  width="50"></a> <div/>
 

  
 <div align= "start">
   
- ## **Dataset**


 To know about the dataset  go through the link.you can also download the dataset 🔗  -> [Anime-dataset](https://www.kaggle.com/datasets/dbdmobile/myanimelist-dataset?select=anime-dataset-2023.csv) 

***Note***:- you need to download only anime-dataset-2023.csv from the kaggle.
  
  </div>






***



<div align= "start">
 
&nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/9TTK8Gc/icons8-requirements-64.png" width="50" alt="icons8-requirements-64" border="0"></a>

</div>



<div align= "start">
  
 - ## **Prerequisites**
   

### Technical skills
- `Power Bi Desktop`
- `Kaggle'
- `Data visualization`
- `Statatics`
- `ETL(Extract transform load)`
  
</div>



***


<div align= "start">
 
&nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/DDYn9zS/icons8-structure-48.png" width="50" alt="icons8-structure-48" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'></a><br />
</div>



<div align= "start">
  
 - ## **Project Structure**



   
- **Main/**
  
  - `Anime-Dashboard.pdf`: **Data Visualisations** in .pdf format.


  - `Anime-Dashboard.pbix`: Data Visualisation in .pbix format.
 
  


- **Main/**
  - `anime-dashboard-template.pbit .pbit`:template  to build others power bi Dashboard.


- `requirements.txt`: software requirements.
- `README.md`: This file.
  
   </div>







***


<div align= "start">

&nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/SyNZJd3/icons8-skills-64.png" width="50" alt="icons8-skills-64" border="0"></a>

</div>


<div align= "start">

- ### **Methodology**
  In the field of data analytics/data science a analyst need to  follow some steps like probelm statements,data extraction,data transfromations and data loading we called that process ETL(Extract transform load) and also Descriptive analytics.in the down below the basic method we have followed in each step-
  
  #### 1. Problem Definition


  Here are the some key points and questions we have explored.
  
  ##### Task List

  Descriptive Analysis(Summary):
    
    - Most favourites anime
    - Most Scored anime by users
    - top rated anime
    - Max episodes in overall produced anime
    - Max scored by users


  Data Visualization:
  
   - Top praducers minimum 50 anim
   - visualization of anime genres using wordcloud visuals.

Data visulalizations(time series):
   - year-vise anime released by type of anime
   - year-vise median durations differences by type of anime
   - year-vise median score(rating) diff. by rating(content rating type)
   - last 13 years median ranks by source
   - by age rating(content type rating) year-vise median differences  of favourite anime
   - year-vise total anime released by source



#### 2. Data Collection
  **Tools** -  *Poer-Bi Data Source*
  We have downloaded the dataset from the open source machine learning and data scienece websites [kaggle](https://www.kaggle.com/datasets/dbdmobile/myanimelist-dataset?select=anime-dataset-2023.csv) and also imported in power bi using excel workbook.

&nbsp; &nbsp;
  #### 3. Data Preprocessing
  **Tools** - *Power-BI Query Editor*
   - Removing nan values,empty,duplcates

   - creating a new column from Aired column by splitting by delimiter(to) and after renaming it.
   - I have faced a problem when visualization of Genres column data because this column contains multiple values in aingle row like Action,Adventure,scifi. but we needed the single value in each row show how we achieve this in power bi.so here the step-by step guide how we have done this -:
     1) first select the "genres" column in power bi query editor.
     2) go to the add new column and split by delimiter(comma).
     3) now select the all new created columns and click on the unpivot columns.
     4) now a new new column created you just need to rename it.
     5) now right click on the new generated column and click on the remove other columns.
     6) now close and apply you can visualize the new created columns data using wordcloud.

&nbsp; &nbsp;
  #### 4.Data Visualisations
 **Tools** - *Power BI DashBoard*
    

&nbsp; &nbsp;
  #### 5. Report Building
  
   **Tools** - *Power BI Report-View*

</div>




***

<div align= "start">

&nbsp; &nbsp; <a href="https://imgbb.com/"><img src="https://i.ibb.co/MCtrJKX/find-1.png" alt="find-1" width="50" border="0"></a>

</div>


<div align= "start">


- ## **Key Findings**

- Action,Adventure,sci-fi movies genres are most common along in all released anime.
- after year 2000 [ONA(Original net animation)](https://en.m.wikipedia.org/wiki/Original_net_animation) type are producing more compare to others type of anime.
- after 2000 - current years all most all anime episides durations has decreased only leaving movies type anime.
-[R- (violence and profanity)](https://myanimelist.net/forum/?topicid=629067)
  content rating movies  rating score found >7 and going to increased year by year.also teen 13 +,R+ mild nudity with rating score >6.
  
-  [R- (violence and profanity)](https://myanimelist.net/forum/?topicid=629067) and R+ mild nudity type content are most favoured compare to other type of contents.
-  from the [manga](https://en.m.wikipedia.org/wiki/Manga)    source anime and original source anime are producing more.[manga](https://en.m.wikipedia.org/wiki/Manga)    source type anime rank are better compare to others type of anime.

 
</div>



***



<div align= "start">

 &nbsp; &nbsp;<a href="https://imgbb.com/"><img src="https://i.ibb.co/q11pdTW/recommended.png" alt="find-1" width="50" border="0"></a>


</div>


<div align= "start">



- ## **Recommendations** 

<div align= "start">

 - ## **Contributors** 
 [**Akash Prasad Mishra**](https://github.com/ak-123459),[**Shivam Tamrakar**](https://github.com/ShivamTamrakar16)
   

</div>

***






 



