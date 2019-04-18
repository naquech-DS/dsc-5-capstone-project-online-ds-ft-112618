
# Are E-Books Overtaking Printed Books at the SPL?

This <a href='https://data.seattle.gov/Community/Checkouts-by-Title/tmmm-ytt6'>data set </a> is made available through the Open Data Program by the City of Seattle; it consists of monthly counts by title of checkout for all physical and digital items from 2005 to present from the Seattle Public Library. The set is updated at the beginning of each month, as of March 2019 it contained more than 33 million of entries with 11 columns. Each row is a checkout count with the following information: 

<br>

<table style="width:80%">
  <tr>
    <th>Column Name</th>
    <th>Description</th> 
    <th>Data Type</th>
  </tr>
  <tr>
    <td>UsageClass</td>
    <td>Denotes if item is “physical” or “digital”</td>
    <td>text</td>
  </tr>
  <tr>
    <td>CheckoutType</td>
    <td>Denotes the vendor tool used to check out the item</td>
    <td>text</td>
  </tr>
  <tr>
    <td>MaterialType</td>
    <td>Describes the type of item checked out (examples: book, song movie, music, magazine)</td>
    <td>text</td>
  </tr>
  <tr>
    <td>CheckoutYear</td>
    <td>The 4-digit year of checkout for this record</td>
    <td>number</td>
  </tr>
    <tr>
    <td>CheckoutMonth</td>
    <td>The month of checkout for this record</td>
    <td>number</td>
  </tr>
    <tr>
    <td>Checkouts</td>
    <td>A count of the number of times the title was checked out within the “Checkout Month”</td>
    <td>number</td>
  </tr>
    <tr>
    <td>Title</td>
    <td>The full title and subtitle of an individual item</td>
    <td>text</td>
  </tr>
    <tr>
    <td>Creator</td>
    <td>The author or entity responsible for authoring the item</td>
    <td>text</td>
  </tr>
    <tr>
    <td>Subjects</td>
    <td>The subject of the item as it appears in the catalog</td>
    <td>text</td>
  </tr>
    <tr>
    <td>Publisher</td>
    <td>The publisher of the title</td>
    <td>text</td>
  </tr>
    <tr>
    <td>PublicationYear</td>
    <td>The year from the catalog record in which the item was published, printed, or copyrighted.</td>
    <td>text</td>
  </tr>
</table>

## Question: Are digital books challenging printed books in the Seattle Public Library?

<p>The Seattle Public Library has been recording all digital and pshysical checkouts since April 2005 and has over 33.4 million of entries which get updated every month, the library also affers and promotes a wide collection of e-books and audiobooks that are availabe for multiple devices.</p>
<p>With this analysis I compare and try to predict checkcout formats for the SPL</p>  

## Methodology

OSEMiN

<b>Obtain</b> Gather information, obtain the data.

<b>Scrub</b> Clean, reduce noise, remove data that is not needed; check, remove or replace missing or null values, extract columns or format data types.

<b>Explore</b> Set up the data, check for multicollinearity, make sure the dataset meets what is necessary for the type of model to apply later on.

<b>Model</b> Implement supervised or unsupervised algorithms.

<b>Interpret</b> Evaluate the results.

## Initial Findings
Over the past decade digital content has made a valiant effort at catching up.
<div>
    <a href="https://plot.ly/~natyquin/64/?share_key=nz6Dr2Em09GlAZoz6o4MAE" target="_blank" title="plot from API" style="display: block; text-align: center;"><img src="https://plot.ly/~natyquin/64.png?share_key=nz6Dr2Em09GlAZoz6o4MAE" alt="plot from API" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="natyquin:64" sharekey-plotly="nz6Dr2Em09GlAZoz6o4MAE" src="https://plot.ly/embed.js" async></script>
</div>

<div>
    <a href="https://plot.ly/~natyquin/68/?share_key=2K35Vfba0Z8DCeomAVaWso" target="_blank" title="plot from API (1)" style="display: block; text-align: center;"><img src="https://plot.ly/~natyquin/68.png?share_key=2K35Vfba0Z8DCeomAVaWso" alt="plot from API (1)" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="natyquin:68" sharekey-plotly="2K35Vfba0Z8DCeomAVaWso" src="https://plot.ly/embed.js" async></script>
</div>
Sound Disc comes second with 3.87M of checkouts, e-books have been chekedout 3.6M times.

<div>
    <a href="https://plot.ly/~natyquin/70/?share_key=j5xxCL96yzhj7EDxt6HMET" target="_blank" title="plot from API (2)" style="display: block; text-align: center;"><img src="https://plot.ly/~natyquin/70.png?share_key=j5xxCL96yzhj7EDxt6HMET" alt="plot from API (2)" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="natyquin:70" sharekey-plotly="j5xxCL96yzhj7EDxt6HMET" src="https://plot.ly/embed.js" async></script>
</div>
Library users are constant for all months during the year

### Most Checkout Titles in the last 6 months

<img src="Images/Screen Shot 2019-04-17 at 5.36.12 PM.png" width=400>
<br>Becoming Michelle Obama was top of the list for the first two months of 2019

<div>
    <a href="https://plot.ly/~natyquin/72/?share_key=VlwfkPWF6FhgjM1TfVNOjX" target="_blank" title="plot from API (3)" style="display: block; text-align: center;"><img src="https://plot.ly/~natyquin/72.png?share_key=VlwfkPWF6FhgjM1TfVNOjX" alt="plot from API (3)" style="max-width: 100%;width: 800px;"  width="800" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="natyquin:72" sharekey-plotly="VlwfkPWF6FhgjM1TfVNOjX" src="https://plot.ly/embed.js" async></script>
</div>

<br> Juvenile Fiction makes number 6 in the list of the top 50, may be an indication that teenagers are still reading...

### Most Checkout Authors
<img src="Images/Screen Shot 2019-04-17 at 5.54.00 PM.png" alt="Authors">
<br>James Patterson, Agatha Christie and Stephen King are top of the list!

## Classification and Predictions

Supervised learning is when we want to predict a certain outcome from a given input and the goal is to train a model that can make accurate predictions for new, never-seen before data. To answer the initial question of clasifying digital and physical checkouts I have used a Logistic Regression model.

The most important features that the classifier takes into account are:

- <b>Checkout type:</b> the tool used to check out an item, the SPL has 5 different tools
 - Freegal: stream and download songs
 - OverDrive: access e-books and audiobooks
 - Horizon: information portal used by the library previously
 - Hoopla: stream movies or TV shows
 - Zinio: digital magazines
- <b>Checkout year</b>
- <b>Creator: </b>the author or entity responsible for authoring the item.
- <b>Subjects: </b>there are over 788,000 different subjects.
- <b>Publication year:</b> the year in which the item was published, printed, or copyrighted.
- <b>_check_eq_publ:</b> this column describes if the title was checked out the same year it was published.


### Counts of correct and incorrect classification

To apply the algortihm I took a random sample from the original set with 'entries without replacement' to avoid choosing any entry more than once. The matrix below is a summary of prediction results on our classification problem.

<br><img src="Images/Screen Shot 2019-04-17 at 6.25.49 PM.png" alt="Authors">

* Total number of digital counts (0) is 15,010
* Total number of physical counts (1) is 15,185
* Correct values predicted by the model: 25,533 
* More errors were made by predicting physical counts (4,633) than predicting digital counts (299)

## Conclusions and Recomendations

* Printed books remain the most popular means of reading.
* The model can predict digital counts slightly better.
* The data schema needs to be reorganized. 
    * There are more than 788 thousand subjects which can be reduce to a smaller number of categories. 
    * Duplicates made due to possible manual entries: William Shakespeare, Shakespeare William, Shakespeare.  
    
### Future work
* Since the author and creator columns have many duplicates, I'd like to manipulate those strings to find the most common names and get a better sense of these entries.
* Make a different target and apply other algorithms.    

## Sources

* https://towardsdatascience.com/understanding-feature-engineering-part-2-categorical-data-f54324193e63
* https://stackoverflow.com/questions/48697770/xgboost-model-consistently-obtaining-100-accuracy
* https://machinelearningmastery.com/tactics-to-combat-imbalanced-classes-in-your-machine-learning-dataset/
* https://machinelearningmastery.com/classification-accuracy-is-not-enough-more-performance-measures-you-can-use/
* https://stats.stackexchange.com/questions/369428/deciding-between-get-dummies-and-labelencoder-for-categorical-variables-in-a-lin
* https://discuss.analyticsvidhya.com/t/label-encoding-vs-one-hot-encoding-in-machine-learning-model/7411
* https://www.analyticsvidhya.com/blog/2016/03/complete-guide-parameter-tuning-xgboost-with-codes-python/
* https://stackoverflow.com/questions/22137723/convert-number-strings-with-commas-in-pandas-dataframe-to-float
* https://realpython.com/python-data-cleaning-numpy-pandas/
* Andreas C. Müller & Sarah Guido. Introduction to Machine learning with Python. 2017
* Jake VanderPlas. Python Data Science Handbook. 2016
