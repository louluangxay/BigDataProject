# BigDataProject
Mike:
* How to browse/copy the files from S3?  Read this https://pandaespresso.me/2018/06/21/using-gdelt-data-with-hive/
* It could give you an error about credentials.  You'll need to create an access key for your user.  https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html#Using_CreateAccessKey

## Team:
### Hilary Ligon, L, Peter Riley, Mike Labadie and Lou Luangxay
GDELT (Global Database of Events, Language, and Tone)
Dataset Summary
“In essence, within 15 minutes of GDELT monitoring a news report breaking anywhere the world, it has translated it, processed it to identify all events, counts, quotes, people, organizations, locations, themes, emotions, relevant imagery, video, and embedded social media posts, placed it into the global context, and made all of this available via a live open metadata firehose enabling open research on the planet itself.”

## What datasets are available and what’s  in each file? 
Headlines/Events (2.5TB size)
## Codebook
http://data.gdeltproject.org/documentation/GDELT-Event_Codebook-V2.0.pdf
Time, Actors, Event Actions (with tone/sentiment), Geography 
http://data.gdeltproject.org/gdeltv2/<yyyymmdd>*.export.CSV.zip
Mention Progression
http://data.gdeltproject.org/gdeltv2/<yyyymmdd>*.mentions.CSV.zip
## Sentiment Analysis
Global Knowledge Graph ( a boxed set of 37 million images through April 2016 is now available.)
Codebook
http://data.gdeltproject.org/documentation/GDELT-Global_Knowledge_Graph_Codebook-V2.1.pdf
## Files
http://data.gdeltproject.org/gdeltv2/<yyyymmdd>*.gkg.csv.zip
## Model Ideas
Can you model the sentiment relationship between U.S. media outlets and international outlets to a specific topic arising during Trump’s presidency (e.g., tariffs, sanctions, G20 meetings, official visits)?
Could you identify countries or particular media outlets where sentiment differs the most on the specific topic?
Perhaps this would be an unsupervised model to find countries that tend to cover events similarly.
This would use the events and sentiment analysis datasets.
Could you try to predict how coverage of an event will change?
Could you identify instances where the sentiment will change most dramatically?
This would use the mention progression dataset.
