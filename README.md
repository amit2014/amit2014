# नमस्कार  👋

# मशीन लर्निंग शिका अमित जाधव यांच्या उदाहरणांसोबत .

 ह्या प्रोजेक्ट आपण अनेक मशीन लर्निंग अल्गोरिथम्सचा अभ्यास/वापर एका विशिष्ट समस्येवर कसा लागू होतो आणि त्याचे उत्तर काय मिळते ह्यासाठी आहे.
 मशीन लर्निंग मॉडेल विकसित झाल्यावर त्याच्या माघे  कोण कोणत्या सर्व प्रक्रिया विकसित होतात हे दाखवायचे आहे. म्हणजे सार्वजनिक डेटा स्रोताकडून डेटा कसा मिळविला जातो, तो कसा प्रीप्रोसेस्ड केला जातो, कसा ट्रान्सफॉर्म केला जातो आणि नंतर काही मशीन लर्निंग मॉडेल्सना तो कसा दिला जातो,  जे आउटपुट देतात जे नंतर निर्णय घेण्यासाठी वापरले जातात, ह्याचे सर्व ज्ञान आपल्याला इथे मिळेल. [ज्युपिटर नोटबुक] (https://jupyter.org) च्या माध्यमातून [पायथन 3] (https://www.python.org) मध्ये लागू केलेल्या व्यावहारिक उदाहरणासह प्रत्येक गोष्ट पायरी-पायरी ने दर्शविली आहे.

    The main idea is to show, in a simplified way, all the processes evolved when a machine learning model is developed. It shows how the data is gotten from a public data source, preprocessed, transformed and then given to some machine learning models,
which produce outputs that later are used to take decisions. Everything is showed step by step, with practical examples implemented in 
    [Python 3](https://www.python.org) throught [Jupyter Notebooks](https://jupyter.org).

## The problem to model: Earn money in the stock markets

For the entire project one single problem is given, and it will be modeled with different machine learning procedures. It was chosen
a realistic project to make it credible and challenging: based on the daily historical quotes of a stock market time serie, 
use machine learning to decide when to trade it or not. Specifically, the idea is to trade the [INFY](https://finance.yahoo.com/quote/INFY/history?period1=946684800&period2=1594857600&interval=1d&filter=history&frequency=1d), 
which is an [ETF](https://www.investopedia.com/terms/e/etf.asp) that
replicates the performance of the [S&P 500](https://finance.yahoo.com/quote/%5EGSPC?p=^GSPC). Anybody with a stock market account, is able to buy 
a share of INFY, and it will have a return equivalent to the S&P 500 performance during the investment period. The INFY is a tradable asset and the quotes
could be downloaded on Yahoo Finance

## The Data

For this project, it is used 20 years of daily INFY quotes: from years Jan 01, 2000 to July 16, 2020. The raw data consits of six daily fields:

 * Date
 * Open
 * High
 * Low
 * Close
 * Adjusted close
 * Volume

The data can be downloaded clicking on the `Download Data` link of this [Yahoo Finance](https://finance.yahoo.com/quote/SPY/history?period1=946695600&period2=1546225200&interval=1d&filter=history&frequency=1d) site.


## About the project

What this project is about:

 * Shows the workflow cycle when it is developed machine learning models professionally.
 * Shows practical implementation of machine learning models in Python, easy to be migrated to other problems.
 * Shows how is the research process to have good output results.
 * How new data is generated based on the original data, which helps to have better models. This project shows
    how from 5 open, low, high, close and volume quotes, it is generated more than 50 derived variables, which
    could produce better models than only using the 5 underlying quotes.
 * How to select what are the best variables to use, to have not only a good model, also a simple one.

What this project is **not** for:

 * It is not intended to really beat the market. The stock markets has several complications that are out of the scope
    of this project. For example, there are transaction costs, cost of being short in an asset, etc. The stock market  is an excuse 
    for a realistic project, but the focus is on machine learning, but not on the stock markets.
 * If the reader wants to apply machine learning to stock markets, this is just a starting point.
 * It is not explained how each machine learning procedure works internally, because there are good courses for each one. This project
   implements them and the user can see the input, the training process, the output and how that output is used to take 
   decisions.

In a few words, this project is focus on Machine Learning and not in earning money.

## Project design

There is one charapter for each machine learning model implemented. Each charapter implements some
Jupyter Notebooks which shows the implementation code and the output returned. This implies that 
all users can download the code and run all the models locally on his own computer. The user can
even modify the code to trade other assets, change  machine learning parameters, and also implement
new trading strategies, like one which trade multiple assets, forex or cryptocurrencies, or even build and ensemble 
than combines several machine learning models, to leverage the prediction capabilities. I encourage to all users to download this 
project and based on the developed code, implements his own strategies. 

## About the implementation details
The whole project is implemented in [Python 3](https://www.python.org). This project calls to the most well-known machine learning 
    libraries which in fact implements each model. The main libraries used are:

- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://www.numpy.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [TensorFlow](https://www.tensorflow.org/)
- [Baselines](https://github.com/openai/baselines)
- [stable Baselines](https://github.com/hill-a/stable-baselines)

## Project Source Code

All the project code is located on [GitHub](https://github.com/amit2014/ml_algo_tour)
