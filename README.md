# Phase 1 Project Description


### Business Problem

Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.


### Key Business Questions for Data Analysis

     * Over the course of the past decade which movies have had the largest box office success in terms of both domestic and worldwide sales?

     * What is the relationship between production costs and expected worldwide gross revenue?

     * What can Microsoft expect to pay in movie production costs?

      * What are some attributes of movie success? Consider audience attention spans when it comes to     movie length. Also consider the time of year of when movies are frequently released.


### Data Sources and Description

There are three primary databases that will be used to answer the business questions. These include data from Box Office Mojo, IMDB, and a The Numbers database.

#### Box Office Mojo dataset 

Box Office Mojo is an American website that tracks movie box office revenue in a systematic and algorithmic way. The Box Office Mojo dataset used for this analysis contains data about movie titles, which studio released the film, and gross revenue broken out into domestic and foreign returns.  The movie release years for this dataset range from 2010 to 2018. This dataset is in CSV format and contains 3387 records. Most of the records are complete with most data nearly complete, except for Foreign Gross revenue where about one third of the data is missing.  

#### IMDB dataset

IMDb (an abbreviation of Internet Movie Database) is an online database of information related to films, television series, home videos, video games, and streaming content online – including cast, production crew and personal biographies, plot summaries, trivia, ratings, and fan and critical reviews. The IMDb dataset is a relational database with several tables. It is the lengthiest out of all the datasets used for this analysis. It contains over 146,000 records. For this analysis three of the relational tables were used to build a dataframe that complements the other datasets and focuses on the key business questions by including movie genres, ratings, and movie runtime in minutes.  

#### The Numbers dataset

The Numbers is a film industry data website that tracks box office revenue in a systematic, algorithmic way. The company also conducts research services and forecasts incomes of film projects. This dataset contains similar information to the Box Office Mojo dataset but it also contains production budgets and exact release dates, along with the revenue records. This dataset is in CSV format and contains 5782 records with no missing data. 

### Data Workflow Process

* The datasets were individually examined to identify their content and structure. Using the Pandas and SQLite3 libraries three individual dataframes based on each dataset was created. 


* The three dataframes were merged into one dataframe to ensure uniformity across the datasets. 


* This "super" dataframe was examined for duplicate data, missing data and datatypes. Duplicate data was dropped. Missing data was cleaned by replacing with relevant mean, median, or mode values. Some missing data was categorized as missing and other missing data was dropped if it did not greatly affect the overall data spread.  


* The "super" dataframe was then analyzed by extracting descriptive statistical info. The top 50 movies measured by worldwide gross revenue were extracted for statistical info and for information related directly to our key business questions related to costs, revenue, movie lengths, and release times. 


* Exploratory and Explanatory data visualizations were then created to identify patterns and trends and to better communicate findings. 


* Finally, conclusions and concrete recommendations to Microsoft were developed based on our driving business questions to help Microsoft break into the Movie Business. 


### Three Visualizations




![scatter_budget_revenue-Copy1](https://user-images.githubusercontent.com/104652254/178409291-8bb2d52f-e93a-4f4b-bad0-f2d07e2be079.png)

![median_budget_cost-Copy1](https://user-images.githubusercontent.com/104652254/178409330-343f3243-9552-41db-bf6a-7598f2ec6644.png)

![movie_month-Copy1](https://user-images.githubusercontent.com/104652254/178409478-92b2e148-fd63-4337-b565-0a7c5cf0f82f.png)

![movie_minutes-Copy1](https://user-images.githubusercontent.com/104652254/178409521-42955208-8245-41fe-8fa4-3578ae18edf2.png)


### Navigating Repository

*Inside this repository is a jupyter notebook with all code, comments, and markdown. There is also a pdf that you can examine without having to open a jupyter notebook.
*The three databases that the notebook relies on are also available in the main repo directory. 
*The repo also contains images directly related to the business recommendations. They are also posted above in this readme.md.
*Finally, this repo contains a presentation pdf of slides that lays out the business context and recommendations to Microsoft executive to support them in their decision to break into the movie business. 


### Conclusion


* For the top 50 films per year the median production budget was USD 75 million, most films budgets ranged between USD 40 to 140 million. These costs reflect a median of 26% of revenue but can vary between 17-39%. 


* Despite the steep initial production costs, the top 50 films each year enjoyed a domestic revenue median of USD 100 million. To further pad revenue worldwide releases brought in a median of USD 240 million with an interquartile range of USD 153 million to USD 443 million. A real risk remains, however, of creating a movie that barely covers production costs and possibly delivers a blow to the company's brand. 


* Timing is important when releasing a film. Many films are released around October, November, and December followed by June and July. May, June, and July see some of the highest grossing films come out. 


* Most films range between 99 to 127 minutes with a median of 112 minutes.

### Recommendations


* Microsoft should set aside a fund of USD 75 million per film in order to break into the top 50 films in a calendar year. The initial budget can be set lower towards the USD 40 million range but no lower. Be prepared with a cushion of funds up to that USD 75 million mark, especially because Microsoft is new to the industry. What may be a lower cost film for other studios, Microsoft will possibly have to spend more initially to establish connections with movie directors, actors, distribution networks, marketing structures and the development of movie infrastructure that it may currently lack. Microsoft could easily spend in the hundreds of millions of dollars to create just one box office hit, but it is likely worth starting with a few films that have productions costs set close to the median.


* To ensure production costs are covered and to expand the return on initial investments, Microsoft should consider a worldwide release of their films instead of to domestic audiences only. The potential to match domestic revenue and beyond with a is a real possibility. Beware the risks, however, no movie is guaranteed box office success. Microsoft should consider development of three movie ideas to take to production to spread risk. Despite higher initial investments for three films the chance of delivering a successful film measured in revenue is higher. 


* Microsoft should release an initial film sometime at the end of May or early June. This is the beginning of the summer movie season when many films are released and when some of the highest grossing films come out. November and December are also good times, but so many films come out during this time it's possible Microsoft's film could get lost in the mix. 


* For an initial release the movie should range between 99 to 127 minutes. The sweet spot is around 112 minutes for many films. Longer films may require a greater attentional effort from audiences. Longer films also appear to slowly, but steadily, add to production costs. 


       
