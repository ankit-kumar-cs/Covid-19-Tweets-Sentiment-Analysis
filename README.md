# Twitter-Sentiment-Visualization-for-Lockdown-Extension
**1**. First we need to collect the data of tweets. We have used the [Download Data Link](https://ieee-dataport.org/open-access/coronavirus-covid-19-tweets-dataset) to collect the tweets.</br>
**2**. The downloaded data is in csv file so have to combine all csv files of a particular **phase**.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;Use [This File MergeData.ipynb](MergeData.ipynb) to merge all the csv files of a particular phase in one text file.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;File generated after this step will look like this [Text File](final-phase4.txt)</br>
**3**. After step 2 now we have one text file in each phase folder that contains all the tweet ids. Now our task is to</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp; Hydrate the text file to get actual tweets and other information about the tweets.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(2)&nbsp; Apply pre-processing on the data to clean the data.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(3)&nbsp; Changing the data in required format.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;To accomplish the above mentioned tasks use the [HydrateTweets.ipynb File](HydrateTweets.ipynb).</br>
        &nbsp;&nbsp;&nbsp;&nbsp;A [final_cleaned_data.csv](final_cleaned_data.csv) file will be created that contains data to be visualized.</br>
**4**. Now we will apply some Python Data Science techniques for **Sentiment Analysis**. To accomplish following tasks</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp; Calculate sentiment value of each tweet.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp; Calculate weight of each tweet.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp; Subdivide the sentiment into Positive,Negative,Weakly Positive,etc.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp; Calculate Average Sentiment Value.</br>
        &nbsp;&nbsp;&nbsp;&nbsp;Use [sentiment_analyis.py](sentiment_analysis.py)</br>
**5**. After the sentiment analysis we have [plot_data.csv](plot_data.csv) and [plot_data_1.csv](plot_data_1.csv) which contains the data to be plotted.</br>
**6**. Final step is to visualise the data. We have used Watson Studio with IBM Cognos Analytics for this purpose. </br>
        &nbsp;&nbsp;&nbsp;&nbsp; Link of the dashboard [Visualisation](https://dataplatform.cloud.ibm.com/dashboards/1eae785d-7db1-4a2f-b6b2-b42ac2cce86a/view/7915f71f38b7349171e9e6e4079f2a527b347709b3bb8106d6807b490d637297a96017c0c82d1e5dde120d36fbe8135cce)
