# Housing Price Predictor - Metro Phoenix

<h3>Team:</h3>
<ul>
    <li>Christian Blomgren</li>
    <li>Drew Kirke</li>
    <li>Tim Spendley
</ul>

<h3>Overview</h3>
<P>(Project Summary - to be written)  </p>

<h3>Data Source</h3>

<p>In order to utilize current data in the model, the choice was made to scrape current home prices (as of May 30, 2024) from the Zillow&trade; website. Two sets of data were retrieved: a set of recently sold homes (&lt;7 days) for use in training the model, and homes currently available for sale for use in predicting the expected price.<p>

<p>Becuase of technical challenges with scraping manually (via Beautiful Soup) and after extensive research, the team used a third-party service - Apify&trade; - to scrape the data. Apify provides a user-agent to scrape the site based on a url construct provided by the user.</p>

<b>Data url:</b><a href="https://www.zillow.com/phoenix-az/sold/?searchQueryState=%7B%22pagination%22%3A%7B%7D%2C%22isMapVisible%22%3Atrue%2C%22mapBounds%22%3A%7B%22west%22%3A-112.63061986914062%2C%22east%22%3A-111.55121313085937%2C%22south%22%3A33.28514328583089%2C%22north%22%3A33.925649143779%7D%2C%22regionSelection%22%3A%5B%7B%22regionId%22%3A40326%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A47958%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A54346%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A18298%2C%22regionType%22%3A6%7D%2C%7B%22regionId%22%3A40298%2C%22regionType%22%3A6%7D%5D%2C%22filterState%22%3A%7B%22sort%22%3A%7B%22value%22%3A%22globalrelevanceex%22%7D%2C%22ah%22%3A%7B%22value%22%3Atrue%7D%2C%22rs%22%3A%7B%22value%22%3Atrue%7D%2C%22fsba%22%3A%7B%22value%22%3Afalse%7D%2C%22fsbo%22%3A%7B%22value%22%3Afalse%7D%2C%22nc%22%3A%7B%22value%22%3Afalse%7D%2C%22cmsn%22%3A%7B%22value%22%3Afalse%7D%2C%22auc%22%3A%7B%22value%22%3Afalse%7D%2C%22fore%22%3A%7B%22value%22%3Afalse%7D%7D%2C%22isListVisible%22%3Atrue%7D">Zillow Results Page</a>

<h3>Libraries and Dependencies</h3>
<h5>Data Cleaning</h5>
<ul>
    <li>Libraries: Pandas, SQL Alchemy</li>
    <li>Dependencies: Sqlite, Jupyter</li>
</ul>
<h5>Model Training</h5>
<ul>
    <li>Libraries: SKLearn (model_selection, prepocessing, metrics), Keras (models, layers)</li>
    <li>Dependencies: Sqlite, Jupyter</li>
</ul>
<h5>Visualization</h5>
<ul>
    <li>Libraries: Pandas, SQL Alchemy</li>
    <li>Dependencies: Sqlite, Jupyter</li>
</ul>


<h3>Results and Conclusions</h3>
<p>(Summary details - will create from visualizations/presentation)</p>


<h3>References</h3>
<ul>
    <li><a href="https://www.zillow.com/">Zillow.com</a> - Housing Listings
    <li><a href="https://apify.com/">Apify.com</a> - Full stack web-scraping and data extraction platform.
<ul>
