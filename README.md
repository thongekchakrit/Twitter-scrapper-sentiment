# Automated Twitter Keyword And Hashtag Sentiment Analysis

<p align="center">
  <img width="640" height="300" src="https://github.com/thongekchakrit/TwitAnlysis-to-csv/blob/master/images/overview.gif">
</p>

More and more people are turning online to voice their opinions, whether on products, services, politics, or daily issues. To get a better picture of how the crowd is feeling, it is important to analyze their opinions. 

In this project, using python, I have written a code that will semi-automatically scrape twitter (using your input keyword), perform sentiment analysis, plot the sentiments values onto two graphs and save the scraped tweets into a CSV file. The data was scrapped from Twitter using [Tweepy](http://docs.tweepy.org/en/v3.5.0/api.html), [Textblob](https://textblob.readthedocs.io/en/dev/) was used to perform sentiment analysis (lexicon method) and [Plotly](https://plotly.com/python/) was used for data visualization.

This project incorporates the understanding of API, object-oriented programming, regular expression and data visualization. I had fun making the project, especially while writing the code for automatic graph plotting!

## Getting Started

The instructions below will help you set up the environment. To get started download the 'notebook' folder or this repository as ZIP file.

### Prerequisites

To use the program, you need to statisfy the conditions below:

```
1. Anaconda (to get Jupyter Notebook)
2. Jupyter Notebook (or any other python software)
3. Twitter Developer Account (to get credential tokens)
```

All are free to use and getting these tools will take about 10 minutes to do so. Once you have those tools, go ahead and open the downloaded file ‘Twitter Scrapper Lexicon Analysis.ipynb’ on your computer. 

Next, you would need to navigate back to Twitter developer account. Now, create an application (free), and grab the API key (consumer key), API key secret (consumer secret key), access token and access token secret key from your ‘Project & App’ tab. 

Finally, you are ready to use the program!

### Demonstration of program

**Step 1:** Import the libraries. 

* If you dont have these libraries installed, type in the code below and hit SHIFT+ENTER.

```
!pip install textblob
!pip install tweepy
!pip install plotly
```

**Step 2:** Insert Twitter authentication keys that you have obtained.

<p align="center">
  <img width="640" height="250" src="https://github.com/thongekchakrit/TwitAnlysis-to-csv/blob/master/images/Settinguptwitterr.PNG">
</p>

**Step 3:** Excecute the cell. A prompt will appear requesting for your input, insert the keyword that you wish to find and hit ENTER. 

* For the keyword, you can insert one or more words, the end result is dependent on Twitter search algorithm.
* As an example, I will be searching for the keyword 'jamus lim', a Singaporean politician who is currently a local internet sentation.

<p align="center">
  <img width="640" height="250" src="https://github.com/thongekchakrit/TwitAnlysis-to-csv/blob/master/images/searchtwitterr.PNG">
</p>

**Step 4:** That's all! 

* The results are generated and an excel CSV file, under the name of 'Twitter_Analysis.csv' will be saved in the same folder where 'Twitter Scrapper Lexicon Analysis.ipynb' was. 

* Here are the results

![Result_1](https://github.com/thongekchakrit/TwitAnlysis-to-csv/blob/master/images/result_1.png)

![Result_2](https://github.com/thongekchakrit/TwitAnlysis-to-csv/blob/master/images/result_2.png)

The result is accurate to a certain extend. Singaporeans have high admiration for Jamus Lim and it was well reflected by the sentiment analysis. Out of the 34 scrapped tweets, 17 (50%) were deemed positive, 15(44%) were deemed neutral or objective and 2 (5%) were deemed negative. 

Although this program is not 100% accurate (especially so when we are analysing tweets where people are more likely to use short forms and slangs), it does give a very rough sense of what people are feeling. You can evalute the sentiment by looking at the CSV file. 

### What I wish to do next

```
1. Make a stand alone exe file using python Tkinter GUI and Pyinstaller
2. Create a looping automatic tweet scrapper (Stream Tweets) into a database (SQLite)
```

## Built With

* [Anaconda](https://www.anaconda.com/) - Required for Jupyter Notebook
* [Jupyter Notebook](https://jupyter.org/)
* [Plotly](https://plotly.com/python/) - Use to visualize data
* [Tweepy](http://docs.tweepy.org/en/v3.5.0/api.html) - Use to scrape twitter API
* [Textblob](https://textblob.readthedocs.io/en/dev/) - Use for sentiment analysis
* [Twitter Developer Account](https://developer.twitter.com/en)


## Author

* [Chakrit Thong Ek](https://github.com/thongekchakrit)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

**Inspired by** [LucidProgramming](https://www.youtube.com/watch?v=wlnx-7cm4Gg&t=23s)
