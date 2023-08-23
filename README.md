# Coping-youtube-urls
These are steps to copy the Youtube urls from any specific channels using the inspect console.


### Follow these steps to scrape the data from youtube-:
#### Step1 -: First of all open your youtube channel and go to the videos tab.

#### Step2-: Right click on anywhere in screen and click on Inpect elements.

#### Step3-: Click on console tab then refresh your webpage.

#### Step4-: Now you have to copy this code and paste it in console to load your all videos on that page.
```var scroll = setInterval(function(){ window.scrollBy(0, 1000)}, 1000);```

#### Step5-: Now you have to wait some seconds to load all videos

#### Step6-: Now you have to copy this code and paste it in console to get all videos title and link in the console.
```window.clearInterval(scroll); console.clear(); urls = $$('a'); urls.forEach(function(v,i,a){if (v.id=="video-title"){console.log('\t'+v.title+'\t'+v.href+'\t')}});```

#### Step7-: Now press Ctrl+A and CTRL+C then open google sheet or excel sheets to paste this data. You can delete the first column. 
