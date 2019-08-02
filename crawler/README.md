
# Wardley Map Blog Graph     
This blog hosts original articles about the Wardley Mapping method.   A strategy mapping and thinking tool.  
To maximize the value of this blog, I need to figure out the highest valueable articles to read first. And more, I need to analyse the relationship between concepts and pages so that I can explore the world of super-thinking easier.  
    
This tool will crawl the [blog.gardeviance.org](blog.gardeviance.org) website and build a graph between all pages, so that you could use any graphy-analysis tool of your choice to find most valuable knowledge.  
    
# How to run the crawler    
 ## First install Scrapy 

    $ sudo apt install python3 python3-pip python3-venv  
    
## Install crawler requirements  

    $ git clone https://github.com/vantt/wardleymapBlog  
    $ cd wardleymapBlog/crawler 
    
    $ python3 -m venv env  
    $ source env/bin/activate  
    $ pip3 install -r requirements.txt  

  
## Run Crawler  
### First run the crawler:  

    $ ./runspider.sh  

  
### Build Graph data  

    $ ./rebuild_graph.py  


## Crawling Result
Result file will be put in [data] folder inside the crawler.
They are in json-line format. Each line is a json-record contains the page-information (title, url) and links to all other pages. 
 
{"url": "https://fs.blog/the-knowledge-project/", "id": 878911802, "title": "The Knowledge Project with Shane Parrish", "links": {"664197469": "https://itunes.apple.com/us/podcast/the-knowledge-project-podcast-by-shane-parrish/id990149481?mt=2", "608962016": "https://www.stitcher.com/podcast/shane-parrish/the-knowledge-project", "2503421208": "https://open.spotify.com/show/1VyK52NSZHaDKeMJzT4TSM", "4227195128": "https://overcast.fm/itunes990149481/the-knowledge-project-with-shane-parrish", "1872324716": "http://subscribeonandroid.com/theknowledgeproject.libsyn.com/rss", "1784428517": "https://play.google.com/music/listen?u=0#/ps/I5jjqydj2cft3iv2q6lmwwxkaau", "2607495604": "https://fs.blog/sue-johnson/", "4070835184": "https://fs.blog/jonathan-haidt/", "2892593722": "https://fs.blog/jim-dethmer/", "3739989806": "https://fs.blog/thomas-tull/", "2727648062": "https://fs.blog/gabriel-weinberg/", "1125610307": "https://fs.blog/sheila-heen/", "2563002376": "https://fs.blog/daniel-gross/", "1761605076": "https://fs.blog/scott-page/", "1470541694": "https://fs.blog/jason-fried", "16386020": "https://fs.blog/howard-marks/", "2444158675": "https://fs.blog/laura-markham/", "1262704348": "https://fs.blog/celeste-headlee/", "3436728153": "https://fs.blog/josh-wolfe/", "3501103913": "https://fs.blog/brent-gilchrist/", "2094360544": "https://fs.blog/adam-robinson-pt2/", "1475884067": "https://fs.blog/adam-robinson-pt1/", "4059873383": "https://fs.blog/sophie-gregoire-trudeau/", "147570101": "https://fs.blog/dan-kluger/", "2721262310": "https://fs.blog/barbara-coloroso/", "284809354": "https://fs.blog/jennifer-garvey-berger/", "1493097462": "https://fs.blog/atul-gawande/", "2575132512": "https://fs.blog/tobi-lutke/", "1809285569": "https://fs.blog/ben-thompson/", "3576581397": "https://fs.blog/tyler-cowen/", "2163821018": "https://fs.blog/ali-almossawi/", "435596355": "https://fs.blog/annie-duke/", "2405924832": "https://fs.blog/william-macaskill/", "4023830316": "https://fs.blog/robert-greene/", "4160963371": "https://fs.blog/amelia-boone/", "1985728860": "https://fs.blog/dan-ariely/", "252656594": "https://fs.blog/2018/05/patrick-collison/", "981014442": "https://fs.blog/2018/04/learning-barbara-oakley/", "257904239": "https://fs.blog/2018/03/margaret-heffernan/", "2652036969": "https://fs.blog/2018/03/dacher-keltner-power/", "1267796678": "https://fs.blog/2018/02/michael-mauboussin-interview/", "1098625359": "https://fs.blog/2018/01/chris-voss/", "3432833203": "https://fs.blog/2017/12/warren-berger/", "2618190890": "https://fs.blog/2017/11/gary-taubes-sugar/", "828657730": "https://fs.blog/susan-cain/", "878225249": "https://fs.blog/ray-dalio/", "3922308260": "https://fs.blog/adam-grant/", "171460203": "https://fs.blog/ed-latimore/", "2327403674": "https://fs.blog/2017/07/marc-garneau-future-transportation/", "2964268501": "https://fs.blog/rory-sutherland/", "361830566": "https://fs.blog/naval-ravikant/", "1093079238": "http://traffic.libsyn.com/theknowledgeproject/TKP_Greece_History_No_Ad.mp3", "96323087": "http://traffic.libsyn.com/theknowledgeproject/TKP_Greece_Wine_No_Ad.mp3", "1896324291": "https://fs.blog/samuel-arbesman/", "4294329162": "https://fs.blog/morgan-housel/", "2677184442": "https://fs.blog/pedro-domingos/", "830407570": "https://fs.blog/veronique-rivest/", "2319046850": "https://fs.blog/ryan-holiday/", "3259875466": "https://fs.blog/alexander-shelley/", "1165853197": "https://fs.blog/julia-galef/", "3365593372": "https://fs.blog/venkatesh-rao/", "3305153399": "https://fs.blog/philip-tetlock/", "379469860": "https://fs.blog/chris-dixon/", "439120079": "https://fs.blog/jason-zweig/", "2518389791": "https://fs.blog/sanjay-bakshi/", "2219374316": "https://fs.blog/michael-lombardi/", "2876592106": "https://fs.blog/michael-mauboussin/", "1015062712": "https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=8EK856PWBGKCW", "60952684": "https://www.fs.blog/privacy-policy/"}}

## Graph Analysis
crawling data and final graph data will be put in **[data]** folder
