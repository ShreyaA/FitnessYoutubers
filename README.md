<h1>Analyzing Youtube Video Data from Most Popular Fitness Channels featuring women </h1>

<h2> 1. Aims, objectives, background </h2>

<h3> 1.1 Introduction </h3>

Established in 2005, YouTube has evolved into the second-largest search engine globally, processing over 3 billion searches monthly, trailing only behind Google. Despite its pervasive influence, there remains a pervasive lack of clarity surrounding the mechanics of the YouTube algorithm and the determinants of a video's visibility and recommendation over others. YouTube boasts one of the most expansive and sophisticated industrial recommendation systems in existence.

For content creators, deciphering the factors influencing a video's success proves to be a formidable challenge. Numerous misconceptions circulate regarding the metrics contributing to a video's prominence, such as the significance of likes, comments, or the optimal duration of a video. Navigating through these uncertainties requires experimentation and a keen observation of trends within specific niches, shedding light on the elusive nature of YouTube's recommendation dynamics.

<h3> 1.2 Aims and objectives </h3>

Physical health is a huge component of overall well being. Personally, I exercise mostly by following YouTube videos created by female fitness influencers. As someone who is grateful to these people for sharing such valuable content for free, I wish to understand what does it take to succeed in this space, and what kind of fitness content is consumed by the rest of the world.

With this project, I would like to explore the following: 

* Work with Youtube API and how to obtain video data.
* Analyze video data and verify different commonly considered features about what makes a video do well on Youtube, for example:
    * Number of likes and comments
    * Video duration
    * Title length
    * Tags 
    * Temporal features: how often and what time of the week do they upload new videos?
    * Explore the trending topics using NLP techniques
    * Which popular topics are being covered in the videos (e.g. using wordcloud for video titles)?
    * Which questions are being asked in the comment sections in the videos
* Some budding ideas: the influence of shorts, virality factor, "challenge" based spread of videos.

<h3> 1.3 Steps of the project </h3>
    <ol>
    <li> Obtain video meta data via Youtube API for the top 10-15 channels in the data science niche (this includes several small steps: create a developer key, request data and transform the responses into a usable data format) </li>
<li> Prepocess data and engineer additional features for analysis </li>
<li> Exploratory data analysis </li>
<li> Conclusions </li>
    </ol>
    
<h3> 1.4. Dataset </h3>

<h4> Data selection </h4>

I have created my own dataset using the Google Youtube Data API version 3.0. The exact steps of data creation is presented in section 2. Data Creation below.

<h4> Data limitations </h4>

The dataset is a real-world dataset and suitable for the research. However, the selection of the top 11 Youtube channels (that feature videos that have English language titles) to include in the research is purely based on my knowledge of the internet and might not be accurate. My definition is "popular" is only based on subscriber count but there are other metrics that could be taken into consideration as well (e.g. views, engagement). The top 11 also seems arbitrary given the plethora of channels on Youtube. There might be smaller channels that might also very interesting to look into, which is a potential direction to explore in the future.

<h4> Ethics of data source </h4>

According to Youtube API's guide, the usage of Youtube API is free of charge given that your application send requests within a quota limit. "The YouTube Data API uses a quota to ensure that developers use the service as intended and do not create applications that unfairly reduce service quality or limit access for others. " The default quota allocation for each application is 10,000 units per day, and you could request additional quota by completing a form to YouTube API Services if you reach the quota limit.

Since all data requested from Youtube API is public data (which everyone on the Internet can see on Youtube), there is no particular privacy issues as far as I am concerned. In addition, the data is obtained only for research purposes in this case and not for any commercial interests.

<h2> TLDR; </h2>

* My suggestions to aspiring creators:
    * Create <b> 5-15 minute videos (warm ups, stretches, ab workouts, etc.) for repeat viewership </b> and to help those who are strapped for time, and those who want to start/maintain their exercise streak.
    * Post <b> shorts to increase reach and engagement </b>.
    * While shorter videos get more views per video, <b> established YouTubers have a more consistent audience that tune into their longer videos as well </b>. This would also boost your monetization - as YouTube can put more ads in longer videos.
    * Recommended themes: <b> motivational and transformation videos with body positive messaging </b> to inspire your viewers to start their own journey.
    * Many home workout videos target the full body, but ab videos tend to be popular as well, as noted earlier.
    * <b> Include terms like "Fat burn" , "hiit" (high intensity interval training), "challenge" in your titles </b> : they are quite popular - catering to those who have fat/weight loss as their target. YouTubers tend to encourage viewers to take on the challenge and consistenly perform certain workouts of their to see coveted results (such as abs in 15 days).
    * Mention whether your workout needs <b> equipment </b> is recommended as many people who engage in home exercises are at the beginner-intermediate level of their fitness journey and may not have dumbells and other exercise equipment.
    * Mentioning the <b> parts of the body that are being targeted - leg , booty, thigh </b> is a good strategy.
    * Mentioning the <b> duration of the workout (in minutes) </b> is standard practice among the chosen set of YouTubers.
    * <em> Being descriptive doesn't hurt. </em> Most-viewed videos tend to have average title length of 40-75 characters. 
    * Several videos feature 20-30 tags, so don't be shy while tagging.
    
* There is a high correlation between likes, comments and views. 

* Comments appear to be a slightly better indicator for interaction than likes.

* The number of likes seem to follow the "social proof", which means the more views the video has, the more people will like it.

* Comments on videos are generally positive.
