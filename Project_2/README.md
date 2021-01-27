### Project Title:
## Science Fiction Films - Predicting Popularity

### Description and Data Sources:
Utilizing data scraped from [IMDB](https://www.imdb.com/?ref_=nv_home), [Rotten Tomatoes](https://www.rottentomatoes.com/), [The Numbers](https://www.the-numbers.com/movie/budgets/all), and [Box Office Mojo](https://www.boxofficemojo.com/?ref_=bo_nb_se_mojologo),
I investigated which features seemed to correlate with the highest domestic box office grosses.  The set of films chosen were the [top 2000 science fiction films](https://www.imdb.com/search/title/?title_type=movie&genres=sci-fi&start=1&explore=title_type,genres&ref_=adv_nxt) rated by popularity on IMDB.

### Tools Used:

Beautiful Soup

Selenium

Seaborn

sklearn

### Features:
Initial numerical features included production budget, runtime, and year.  Initial categorical variables included crossover genres and [MPAA ratings](https://www.regmovies.com/static/en/us/mpaa-ratings). For the final model, categorical variables were created from [Tomatometer](https://www.rottentomatoes.com/about) scores (over 60% positive rating 'certified fresh'), [Metascore](https://www.metacritic.com/about-metascores) ratings (over 60% positive rating 'meta green'), and a numerical variable of age was created as a transformation of the year feature. Intermediate explorations also included an investigation of whether a director's film count impacted box office grosses, but no correlation was found in the final model.

### Target Variable:
The target variable for this investigation was domestic box office grosses, measured in US dollars.

### Possible Impacts:
The use case envisioned for this data was the current transition from in-person theatrical releases to online streaming services for release of movies.  In a home environment where big budget CGI and large scale production costs might yield lesser visual impact on smaller screens, studios could pivot toward other features of movies that positively impact revenue.  

For science fiction movies, in this linear regression model, while budget was still the most salient feature, genre crossover categories such as Action, Adventure, and Animation correlated with higher grosses, while Crime crossovers correlated with a negative impact on grosses.  

Additionally, critical reception scoring, such as Rotten Tomatoes Tomatometer and Metascore, positively correlated with increased box office grosses.  

Finally, an MPAA rating of R for the film positively correlated with increased box office grosses.  

In the era of recommender systems, being able to mine box office release data for information on genres, MPAA ratings, and critical reception scores might help studios to produce titles sharing these characteristics for lesser budget and greater annual recurring revenue in the online streaming delivery category.
