---
layout: default
title: The story of BigFoot and how to find him
---

<html>
<head>  
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Garamond, serif; /* Change the font family here */
        }
    </style>
	<style>
        .page-title {
            color: white;
            font-size: 32px;
        }
        h3 {
            font-size: 14px;
            text-align: center
        }
		.column {
			float: left;
			width: 80%;
			padding: 10px;
			box-sizing: border-box;
            text-align: center;
		}
         .column embed {
            max-width: 100%; /* Ensure images don't exceed the column width */
            height: auto; /* Allow images to adjust their height proportionally */
            display: block; /* Make sure images don't overflow horizontally */
            margin: 0 auto; /* Center the images horizontally */
        }
		.column img {
			display: block; /* make the image a block element */
			max-width: 100%; /* set the maximum width of the image to the width of its parent element */
			height: auto; /* allow the height of the image to adjust proportionally */
			margin: 0 auto; /* center the image horizontally */
		}
		.column p {
			width: 100%; /* set the width of the paragraph text to 80% of the column */
			margin: 0 auto; /* center the paragraph text horizontally */
            text-align: justify
		}
        .border-right {
            border-right: 1px solid black;
        }
		.clearfix::after {
			content: "";
			clear: both;
			display: table;
		}
        div {
            text-align: justify
        }
        .back-gif {
            position: absolute;
            left:0;
            width: 100%;
            height: auto;
            z-index:-1;
            transform: translateY(-80%);
        }
        footer {
            text-align: right;
        }
        .center {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 85%;
        }
        iframe {
            display: block;
            border-style:none;
            margin: 0 auto;
        }
	</style>
</head>

<body>
    <div>
        <img src="{{ site.baseurl }}/assets/images/bigfootwalking.gif" class="back-gif" alt="Messy">
    </div>
    <h1 class="page-title">{{ page.title }}</h1>
    <p style="color:white">The story of BigFoot and how to find him</p>
    <br>
    <br>
    <h2>Introdution</h2>
    <div>
        <p>
        The legend of Bigfoot has long been etched into the tapestry of American folklore for centuries. The tall, hairy elusive creature is said to roam the vast territories of North America wilderness. The creature seems to always be one step ahead of hunters, always prowling in the blurry edge of a camera shot, howling in the darkness, scaring the dogs. 
        The roots of the tale of Bigfoot can be linked to many other legends, however it was around the mid 20th century when the bigfoot fanbase truly exploded. With the advent of widespread media coverage, reports of Bigfoot sightings began to flood in from all corners of the continent. From the dense forests of the Pacific Northwest to the remote swamps of the American South, people claimed to have encountered this mysterious creature.
        Armed with a lose understand of folklore and basic carpentry Ray L. Wallace kicked off the modern bigfoot legends still prevalent today. In 1958 Wallce created oversized footprints using a pair of carved wooden feet in the woods of california. He never did admit to the hoax but family came out after his death to clear up the mystery. Despite this many will swear on their life to have had an encounter with the creature, this is backed up by numerous reports with varying degrees of “evidence” <a href="https://www.nytimes.com/2003/01/03/us/search-for-bigfoot-outlives-the-man-who-created-him.html" target="_blank">Nytimes </a>[1]. Numerous times bigfoot sightings have been plagued by hoaxes, sparking controversy and interest in the community.<a href="https://books.google.dk/books?id=2RcqAAAAIBAJ&pg=PA3&dq=Bigfoot&article_id=6740,20897&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAQQAg#v=onepage&q=Bigfoot&f=false" target="_blank">Dyers</a>[2]  <a href="https://books.google.dk/books?id=7KgyAAAAIBAJ&pg=PA43&dq=Bigfoot&article_id=2608,3085237&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAkQAg#v=onepage&q=Bigfoot&f=false" target="_blank">Duo</a>[3].
        </p>
    <h2>Our Dataset</h2>
    <p>
        These reports have been collected by the Bigfoot Research Organisation (BFRO), and later been compiled by users on Kaggle with added weather data based on location and temporal data. The dataset is relatively small with 5082 reports spanning from 1950 to 2023, it contains a detailed description of the encounters as well as geographical data. The reports are from all over the place and this article wishes to examine what patterns can be observed in bigfoot reportings.
    </p>
        <div>
        <h3>Figure 1: Wordcloud made from Bigfoot report descriptions (2008-2023)</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/assets/images/bigfootwordclout.png"
            width="1025"
            height="800"
            >
    </div>
    <h2>The history of Bigfoot</h2>
    <p>
Analyzing the frequency of reports per year reveals a noteworthy pattern, commencing around 1950 and marked by several significant peaks, notably in 1978 and during the period of 2003-2005. Preceding these peaks is often a notable bigfoot sighting that captures widespread attention in the media. This is reminiscent of the origins of the bigfoot legend, as elucidated by a New York Times article Nytimes. The piece details the revelation that the initial footprints were part of a prank that spiraled out of control, spawning a narrative unintended by its perpetrators.
        <br>
            <br>
The surge in 1978 corresponds to numerous alleged sightings reported by Bob Stamps, who subsequently gained prominence as a purported bigfoot expert, appearing in various articles and radio broadcasts1 2. The most recent spike, however, stemmed from a deliberate hoax, involving two individuals attempting to sell a purported bigfoot corpse for $25,000, which was later exposed as a costume stored in a freezer, perpetuated by Dyers and Whitton. Dyers Dou.  
        <br>
        <br>
This observation doesn't definitively affirm or debunk the existence of bigfoot; rather, it underscores a fascinating trend wherein bigfoot sightings tend to proliferate following widespread media coverage. This phenomenon may suggest heightened public interest in the subject, prompting more individuals to actively seek out potential sightings. Alternatively, it could indicate opportunists capitalizing on the hype, as exemplified by Dyers and Whitton's actions in 2003.
        <br>
        <br>
It's intriguing to note that the viral dissemination of information is not a contemporary occurrence; rather, it has historically fueled further media attention and subsequent public fascination with the subject.
    </p>
    <audio controls>
    <source src="{{ site.baseurl }}/assets/images/Bigfoot_sound.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
    </audio>
    <div>
        <h3>Figure 2: The amount of Bigfoot reports each year </h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/assets/images/BarChart.html"
            width="1025"
            height="600"
            >
    </div>
    <p>
        While we observe a significant increase in street cleaning requests from the citizens of San Francisco we must be wary in concluding that this can be solely attributed to the streets getting more and more dirty. The increase in requests is of course the principal proxy for dirty streets, but other factors such as the population growth of San Francisco might also affect the tendency. However, The San Francisco Standard recently reported a decline in the population from 2020 to 2022, which we would expect to observe in Figure 2, if the contribution of population estimates was significant <a href="https://sfstandard.com/research-data/san-francisco-bay-area-california-population-decline-census-pandemic-covid/" target="_blank">[7]</a>. Nonetheless, factors such as technology adoption, 311 service awareness, and many others must also be considered as contributing factors to the trend. 
        <br>
        <br>
        In particular, it is interesting to reflect on the fact that in 2008 the iPhone was introduced only 6 months earlier, and the first Android phone was not released until 2009. Fast-forward to today where almost every citizen has a smartphone, and it is much easier to report issues to the 311 Customer Service Center <a href="https://www.statista.com/statistics/201182/forecast-of-smartphone-users-in-the-us/" target="_blank">[8]</a>. This could be a contributing factor to the increase in requests, but it is difficult to quantify the effect of this. This and many other factors as mentioned above are interesting to investigate. Nevertheless, by visually inspecting request tickets we can still get a good idea of the severity of the problem. 
        <br>
        <br>
        We do this in Figure 3, where we show a slideshow of images depicting some of the reported cases. This demonstrates that not all cases are frivolous, and implies that San Francisco does indeed face a severe problem with dirty streets. One could for example imagine the rareness of such occurences in a city such as Copenhagen, which has a very efficient waste management system.
    </p>
    <div class="img">
        <h3>Figure 3:Counties</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/assets/images/County.html"
            width="1025"
            height="550"
            >
    </div>
    <h2>From Needles to Christmas Trees: Decoding San Francisco's Dirty Secrets</h2>
    <p>
        So, we now know that the defilement of San Francisco has increased steadily every year from 2008 to the present time, which shows an unpleasant trend of a city in trouble. Nevertheless, just having an increase in citizen requests can not explain the whole story. As explained above multiple factors are contributing to the increase, but looking into how this increase takes place is another point of analysis that is extremely interesting. What types of requests are most significant, and how do the specific tendencies for each of these look? Are parts of the city more affected by the increase than others, and if so which and why? By answering questions like these it is possible to notice specific patterns that might explain how the City of San Francisco are handling the increase, and maybe catch sight of efforts to decrease specific categories.
        <br>
        <br>
        In Figure 3 below, tendency shows that the larger categories have been a growing issue at least since 2008, when data started being collected. A pattern that stands out is that of the Christmas trees, that only get requested after Christmas - logically making sense. However, this pattern contrasts with Loose Garbage and Debris which has a decrease in its common pattern that matches the christmas tree category. This might be due to the fact that the request type Christmas Trees was first introduced here, and hence the requests about christmas trees on the streets that were earlier categorized as Loose Garbage and Debris are now categorized as Christmas Trees.
        <br>
        <br>
        Another interesting insight we gain from Figure 3 is related to the Human or Animal Waste and Needles categories. Right around 2018 where NBC Bay Area and other news outlets drew attention to the issue of dirty streets, we see a break and decrease in the requests related to these categories. This observation coincides with the reportings of specific measures being taken into action regarding the clean up of specifically these two somewhat more unpleasant categories <a href="https://www.sfchronicle.com/bayarea/article/SF-to-get-team-dedicated-to-clearing-used-needles-12858548.php" target="_blank">[9]</a><a href="https://www.sfaf.org/collections/status/getting-syringes-off-san-francisco-streets/" target="_blank">[10]</a>. This is a positive sign that the city is taking action to improve the situation, and it is interesting to see if this trend continues in the future.
    </p>
    <div>
        <h3>Figure 4: Trends in San Francisco Street Cleaning Requests by Category (2008-2023)</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/assets/images/timeSeriesPlot.html"
            width="1025"
            height="550"
            >
    </div>
    <p>
        In a majority of the stories covering the dirty streets of San Francisco news outlets tend to focus their attention to only a few districts. In particular the Tenderloin district is often mentioned as a district with a severe problem. Nevertheless, as mentioned in the introduction this project aims at achieving a more general understanding of the problem, and therefore we will look at the problem from a complete district-level perspective. 
        <br>
        <br>
        In Figure 4, we show the number of requests per district per year. From this figure, we quickly observe that throughout practically all years the Mission district stands out. This is not surprising as the Mission district is both one of the most populated districts and also one of the districts with the highest homeless population. 
        <br>
        <br>
        On the other hand, a suprising insight is that the Tenderloin and South of Market districts seem to be catching up with the dirty streets. In the years from approximately 2008 to 2019 these districts get as severe a number of requests as the Mission district. However, this has not been the case since 2019. This is contrary to what we would expect, as the Tenderloin and South of Market districts are often mentioned in the stories referenced among the most problematic districts. At first glance a positive sign, but a possible explanation could be that during the COVID-19 pandemic reportings in these areas have been less frequent as it coincides with the time where the pandemic hit the hardest. Nevertheless, this is just a hypothesis that could be investigated further, but is outside the scope of this report. On the other hand, another possible explanation is that the notable increase in the number of requests in the Mission district during the same period suggests a significant shift of requests towards that area. In other words, this implies that the problem may not have been resolved but rather relocated.
    </p>
    <div>
        <h3>Figure 5: A Yearly District-Level Perspective on Street Cleaning Requests</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/assets/images/timeSeriesPlot.html"
            width="1050"
            height="725"
            >
    </div>
    <h2>Mission, South of Market and Tenderloin: A Trifecta of Trouble</h2>
    <p>
        Even though Figure 4 showed signs of a Tenderloin and South of Market in progress, it is still interesting to look at the three districts in more detail as the three districts are often the center of attention for many negative stories about the city. Recently (February 2023) <a href="https://www.cbsnews.com/sanfrancisco/news/surging-crime-dirty-streets-local-residents-say-san-franciscos-mission-district-is-in-crisis/" target="_blank">CBS News</a> [11] reported a story about a business owner in the Mission district debating the surging crimes and dirty streets. While in 2022 <a href="https://www.sfchronicle.com/bayarea/article/sf-mission-tents-17037918.php" target="_blank">San Francisco Chronicle</a> [12] ran a story about how Mission is turning into a worse version of the notorious Tenderloin. It is therefore of interest to look more into these districts, and see if we can find any patterns that might explain why these districts are often mentioned, and more importantly whether the districts are in fact rightfully considered a trifecta of trouble.
        <br>
        <br>
        To answer this, we employ a second dataset that we can use to support the analysis. This dataset is the San Francisco Police Department Incident Reports dataset, which contains information about all the incidents reported to the San Francisco Police Department from 2003 to present. The dataset contains information about the type of incident, the district, the date and time of the incident, and the location of the incident <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry" target="_blank">[13]</a><a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783" target="_blank">[14]</a>. By utilizing this dataset we can get a better understanding of the incidents that occur in the three districts, and see if there are any patterns that might explain why these districts are often mentioned. We therefore show a similar figure as Figure 4, but instead of showing the number of street cleaning requests, we show the number of crime incidents reported to the San Francisco Police Department in Figure 5.
        <br>
        <br>
        From Figure 5, we observe that the Mission district is still the district with the most incidents reported to the San Francisco Police Department. Moreover, we also observe that the Tenderloin and South of Market districts are not far behind. Hence, it seems that the three districts are indeed a trifecta of trouble, when we consider crime and street cleaning data. It is interesting to see that the correlation between crime incidents and street cleaning request is so strong. It shows a worrying sign that such populated and central areas of a city like San Francisco are the home of such a high number of crime incidents and street cleaning requests. Yet, it is well known that crime and poverty are closely related, and the three districts are also among the poorest districts in San Francisco, so the correlation between the two datasets might not be that surprising. But why is this the case? And what measures should the city take to solve the problem? Answering questions like these requires a more in-depth analysis that also includes social data about the demographics of the districts and other related factors that can help explain the problem. As mentioned related to Figure 4, the Mission district is widely known for its high homeless population, and this might be a factor that can help explain the problem. However, getting a more detailed answer to these questions is outside the scope of this report, but is definitely something that could be investigated further.
    </p>
    <div>
        <h3>Figure 6: Trends in San Francisco Street Cleaning Requests by Category (2008-2023)</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/assets/images/timeSeriesPlot.html"
            width="1025"
            height="550"
            >
    </div>
    <h2>Concluding Thoughts</h2>
    <p>
        From our comprehensive analysis of street cleanliness in San Francisco, several key takeaways emerge. Firstly, it is evident that San Francisco has been grappling with cleanliness issues over the years, with the number of cleaning requests increasing significantly from 2008 to 2023. This upward trend suggests that San Francisco's streets are becoming progressively dirtier, affecting the city's image and quality of life for its residents. Hence, confirming that the analysis put out by the NBC Bay Area is still valid, as well as our first hypothesis.
        <br>
        Nevertheless, the rise in street cleaning requests may not entirely indicate an increase in dirtiness. Other factors such as technological advancements, population growth, and awareness of the 311 service could also contribute to this surge. While San Francisco's grimy streets are a pressing issue, it is essential to consider these underlying factors when interpreting the data.
        <br>
        <br>
        The dirty streets are still a prevalent issue today in San Francisco. However, when examining the types of cleanliness complaints, we notice a decrease in requests related to "Human or Animal Waste" and "Needles" around 2018, coinciding with the city's efforts to tackle these specific problems. This positive trend might suggest the city's actions are yielding results and should be sustained.
        <br>
        The data also reveals a geographically uneven distribution of cleanliness issues, with districts like Mission, Tenderloin, and South of Market being most affected. Yet, there seems to be a shift in cleanliness complaints from Tenderloin and South of Market to the Mission district in recent years, suggesting that the problem might be moving rather than resolving.
        <br>
        <br>
        We also observe that a strong correlation exists between areas with high cleaning requests and crime incidents. Mission, Tenderloin, and South of Market, often highlighted as problematic areas, indeed exhibit a high number of both cleaning requests and crime incidents. This correlation, although not surprising considering these areas' socioeconomic status, deserves deeper investigation. Nonetheless, this also confirms the second hypothesis that the city's cleanliness is very much focused on a specific area of the city.
        <br>
        Looking forward, the findings from this report offer several potential directions for further research and action. One clear area is to delve deeper into the reasons behind the geographical shift of cleanliness complaints. Another is to investigate the strong correlation between cleaning requests and crime incidents and the potential underlying socioeconomic factors. Understanding these aspects could provide valuable insights into formulating effective strategies to improve the cleanliness of San Francisco's streets. A potential solution may lie in studying and adopting strategies from cities like Los Angeles, known for its more efficient trash collection programs in terms of money spent per collected trash.
        <br>
        <br>
        As the city grapples with these challenges, it is crucial for residents and visitors to be mindful of the situation, especially when navigating the "trifecta of trouble". Until comprehensive solutions are implemented, the people must be vigilant and proactive in maintaining cleanliness in their neighborhoods.
    </p>
    <a id="references" style="color:inherit; text-decoration: none !important;"><h2>References</h2></a>
    <ol type="1">
        <li>
            <a href="https://www.nytimes.com/2003/01/03/us/search-for-bigfoot-outlives-the-man-who-created-him.html" target="_blank"> How Dirty Search for Bigfoot Outlives The Man Who Created Him </a>
        </li>
        <li>
            <a href="https://books.google.dk/books?id=2RcqAAAAIBAJ&pg=PA3&dq=Bigfoot&article_id=6740,20897&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAQQAg#v=onepage&q=Bigfoot&f=false" target="_blank"> Bigfoot hunters claim they posses a tall tale on ice </a>
        </li>
        <li>
            <a href="https://books.google.dk/books?id=7KgyAAAAIBAJ&pg=PA43&dq=Bigfoot&article_id=2608,3085237&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAkQAg#v=onepage&q=Bigfoot&f=false" target="_blank"> Duo: We Found (the real) Bigfoot </a>
        </li>
        <li>
            <a href="https://londonformayor.com/policies/clean-streets-clean-city-2/" target="_blank"> Mayor Breed: Clean Streets, Clean City </a>
        </li>
        <li>
            <a href="https://sf311.org/" target="_blank"> SF 311 </a>
        </li>
        <li>
            <a href="https://www.youtube.com/watch?v=VEOkX9dp85I&ab_channel=NBCBayArea" target="_blank">NBC Bay Area: Behind the Story: Walking San Francisco's Dirty Streets</a>
        </li>
        <li>
            <a href="https://sfstandard.com/research-data/san-francisco-bay-area-california-population-decline-census-pandemic-covid/" target="_blank">The SF Standard: It’s Official: A Quarter Million People Fled the Bay Area Since Covid</a>
        </li>
        <li>
            <a href="https://www.statista.com/statistics/201182/forecast-of-smartphone-users-in-the-us/" target="_blank">US Smartphone Users 2009-2040</a>
        </li>
        <li>
            <a href="https://www.sfchronicle.com/bayarea/article/SF-to-get-team-dedicated-to-clearing-used-needles-12858548.php" target="_blank">SF Chronicle: SF to get team dedicated to clearing used needles from city’s streets</a>
        </li>
        <li>
            <a href="https://www.sfaf.org/collections/status/getting-syringes-off-san-francisco-streets/" target="_blank">SF Aids Foundation: Getting syringes off San Francisco streets</a>
        </li>
        <li>
            <a href="https://www.cbsnews.com/sanfrancisco/news/surging-crime-dirty-streets-local-residents-say-san-franciscos-mission-district-is-in-crisis/" target="_blank">CBS News: Surging crime, dirty streets; Local residents say San Francisco's Mission District is in crisis</a>
        </li>
        <li>
            <a href="https://www.sfchronicle.com/bayarea/article/sf-mission-tents-17037918.php" target="_blank">SF Chronicle: ‘A neighborhood in chaos’: Is the Mission following in the Tenderloin’s footsteps?</a>
        </li>
        <li>
            <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry" target="_blank">San Francisco Police Department Crime Incident Report from 2003-2018</a>
        </li>
        <li>
            <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783" target="_blank">San Francisco Police Department Crime Incident Report from 2018 to present</a>
        </li>
    </ol>
