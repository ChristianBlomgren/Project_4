# Housing Price Predictor - Metro Phoenix

<h3>Team:</h3>
<ul>
    <li>Christian Blomgren, Drew Kirke, Tim Spendley</li>
</ul>

<h3>Overview</h3>
<P>The goal of this project was to utilize machine learning fundamentals to identify the most accurate ML model able 
to predict the expected sale price for a home in the Phoenix metro region. The process would use recent home sale prices from the following cities: Phoenix, Scottsdale, Tempe, Glendale and Peoria.</p>

<h3>Data Source</h3>

<p>In order to utilize current data in the model, the choice was made to scrape current home prices (as of May 30, 2024) from the Zillow&trade; website. Two sets of data were retrieved: a set of recently sold homes (&lt;7 days) for use in training the model, and homes currently available for sale for use in predicting the expected price.<p>

<p>Becuase of technical challenges with scraping manually (via Beautiful Soup) and after extensive research, the team used a third-party service - Apify&trade; - to scrape the data. Apify provides a user-agent to scrape the site based on a url construct provided by the user.</p>

<b>Data url: </b><a href="https://www.zillow.com/phoenix-az/sold/?searchQueryState=%7B%22pagination%22%3A%7B%7D%2C%22isMapVisible%22%3Atrue%2C%22mapBounds%22%3A%7B%22west%22%3A-112.63061986914062%2C%22east%22%3A-111.55121313085937%2C%22south%22%3A33.28514328583089%2C%22north%22%3A33.925649143779%7D%2C%22regionSelection%22%3A%5B%7B%22regionId%22%3A40326%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A47958%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A54346%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A18298%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A40298%2C%22regionType%22%3A6%7D%5D%2C%22filterState%22%3A%7B%22sort%22%3A%7B%22value%22%3A%22globalrelevanceex%22%7D%2C%22ah%22%3A%7B%22value%22%3Atrue%7D%2C%22rs%22%3A%7B%22value%22%3Atrue%7D%2C%22fsba%22%3A%7B%22value%22%3Afalse%7D%2C%22fsbo%22%3A%7B%22value%22%3Afalse%7D%2C%22nc%22%3A%7B%22value%22%3Afalse%7D%2C%22cmsn%22%3A%7B%22value%22%3Afalse%7D%2C%22auc%22%3A%7B%22value%22%3Afalse%7D%2C%22fore%22%3A%7B%22value%22%3Afalse%7D%7D%2C%22isListVisible%22%3Atrue%7D">Zillow Results Page</a>


<h3>Results</h3>
<p>Two models were evaluated in an effort to effectively predict housing prices. The evaluation process used the recently sold data
to train and test the model, and then was run against homes listed for sale to predict their listed price. This was compared with the actual listed price to determine the effectiveness of the model.</p>

<p>Of the two models (Keras Sequential and Linear Regression) the Sequential model was most effective, although not at a level at which the team could recommend putting the model into use. The measurement results were:</p>
<ul>
    <li>Mean Absolute Error: $231,140 agaist a mean housing price of $690,000</li>
    <li>An r-squared value of 0.64 that, while positive, is not as close to 1 as would be ideal.</li>
</ul>

<h3>Conclusion</h3>
<p>Given the results of the models employed, a better solution should be sought before finalizing the model for production. Better modeling could likely be achieved through some combination of the following steps:</p>
<ul>
    <li>Identify additional attributes that could impact price variance and determine data sources.</li>
    <li>Execute other model types (Regression Tree, KNN) to determine if a better model fit can be found.</li>
    <li>Expand our dataset by including additional locations in the metro area to increase the sample size.</li>
    <li>Research similar projects to understand whether others investigating a similar outcome of new ideas that 
    might aid in the process.</li>
</ul>


<h3>Libraries and Tools</h3>
<h5>Libraries</h5>
<ul>
    <li>Data Cleaning: Pandas, SQL Alchemy</li>
    <li>Model Training: SKLearn (model_selection, prepocessing, metrics), Keras (models, layers)</li>
    <li>Visualization: Matplotlib</li>
</ul>

<h5>Tools</h5>
<ul>
    <li>SQLLite</li>
    <li>Jupyter</li>
    <li>Tableau</li>
</ul>

<h3>References</h3>
<ul>
    <li><a href="https://www.zillow.com/">Zillow.com</a> - Housing Listings
    <li><a href="https://apify.com/">Apify.com</a> - Full stack web-scraping and data extraction platform.
<ul>
