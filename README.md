# Web_Scraping

### Challenge : Scraping SEC for inside trading information.

SEC Form 4 is used by officers, directors, and other corporate “insiders” to notify the U.S. Securities and Exchange Commission (SEC) of their personal transactions in their company's securities.  For this exercise, please write a small scraper to extract information from Form 4 on SEC site. 

For instance, below link takes you to a SEC page of all filings by APPLE

https://www.sec.gov/Archives/edgar/data/320193/

320193 is a unique CIK code for APPLE in SEC system and there is a list of folders on that page. click on any of those hyperlinks will give you a list of files in html and xml formats. 

If you click on one of those hyperlinks (https://www.sec.gov/Archives/edgar/data/320193/000032019322000063), you will see four files and click on the link ending with 'index.html' will take you to filing detail page. Both .xml and .html files of the Form 4 are available and please develop a scraper to extract data of the Form 4. For simplicity, you can just focus on "Common Stock". 

Please take the scalability into consideration while developing this scraper as it should be able to extract multiple companies’ data a time. For this exercise, you do not need to scrap all filed on Form 4. Below is a list of companies with their CIK code and please feel free to include more companies if you like.  

TSLA	1318605

AAPL	320193

NVDA	1045810

AMZN	1018724

MSFT	789019

FB	1326801

GOOGL	1652044

MRNA	1682852

UPST	1647639

CRWD	1535527

SOFI	1818874

HOOD	1783879

PYPL	1633917

ABNB	1559720

AMD	2488

SEC website requires to include browser information while querying the data otherwise you might get “unauthorized access” error. You can use below headers for connection.
{ 'Connection': 'close',
         'Accept': 'application/json, text/javascript, */*; q=0.01', 'X-Requested-With': 'XMLHttpRequest',
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.163 Safari/537.36',
         }
