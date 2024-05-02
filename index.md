---
layout: default
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
            color: black;
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
    <h1 class="page-title">The story of BigFoot and how to find him</h1>
    <br>
    <br>
    <h2>Introdution</h2>
    <div>
        <p>
        The legend of Bigfoot has long been etched into the tapestry of American folklore for centuries. The tall, hairy elusive creature is said to roam the vast territories of North America wilderness. The creature seems to always be one step ahead of hunters, always prowling in the blurry edge of a camera shot, howling in the darkness, scaring the dogs. 
        The roots of the tale of Bigfoot can be linked to many other legends, however it was around the mid 20th century when the bigfoot fanbase truly exploded. With the advent of widespread media coverage, reports of Bigfoot sightings began to flood in from all corners of the continent. From the dense forests of the Pacific Northwest to the remote swamps of the American South, people claimed to have encountered this mysterious creature.
        Armed with a lose understanding of folklore and basic carpentry Ray L. Wallace kicked off the modern bigfoot legends still prevalent today. In 1958 Wallce created oversized footprints using a pair of carved wooden feet in the woods of california. He never did admit to the hoax but family came out after his death to clear up the mystery. Despite this many will swear on their life to have had an encounter with the creature, this is backed up by numerous reports with varying degrees of “evidence” <a href="https://www.nytimes.com/2003/01/03/us/search-for-bigfoot-outlives-the-man-who-created-him.html" target="_blank">Nytimes </a>[1]. Numerous times bigfoot sightings have been plagued by hoaxes, sparking controversy and interest in the community.<a href="https://books.google.dk/books?id=2RcqAAAAIBAJ&pg=PA3&dq=Bigfoot&article_id=6740,20897&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAQQAg#v=onepage&q=Bigfoot&f=false" target="_blank">Dyers</a>[2]  <a href="https://books.google.dk/books?id=7KgyAAAAIBAJ&pg=PA43&dq=Bigfoot&article_id=2608,3085237&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAkQAg#v=onepage&q=Bigfoot&f=false" target="_blank">Duo</a>[3].
        </p>
    <h2>Our Dataset</h2>
    <p>
        These reports have been collected by the Bigfoot Research Organisation (BFRO), and later been compiled by users on Kaggle with added weather data based on location and temporal data. The dataset is relatively small with 5082 reports spanning from 1950 to 2023, it contains a detailed description of the encounters as well as geographical data. The reports are from all over the place and this article wishes to examine what patterns can be observed in bigfoot reportings.
    </p>
        <div>
        <h3>Figure 1: Wordcloud made from Bigfoot report descriptions (2008-2023)</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/SocialDataFinal/assets/images/bigfootwordclout.png"
            width="1025"
            height="820"
            >
    </div>
    <h2>The history of Bigfoot</h2>
        <div>
        <h3>Figure 2: The amount of Bigfoot reports each year </h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/SocialDataFinal/assets/images/BarChart.html"
            width="1025"
            height="600"
            >
    </div>
    <p>
Analyzing the frequency of reports per year reveals a noteworthy pattern, commencing around 1950 and marked by several significant peaks, notably in 1978 and during the period of 2003-2005. Preceding these peaks is often a notable bigfoot sighting that captures widespread attention in the media. This is reminiscent of the origins of the bigfoot legend, as elucidated by a New York Times article <a href="https://www.nytimes.com/2003/01/03/us/search-for-bigfoot-outlives-the-man-who-created-him.html" target="_blank">Nytimes </a>[1]. The piece details the revelation that the initial footprints were part of a prank that spiraled out of control, spawning a narrative unintended by its perpetrators.
        <br>
            <br>
The surge in 1978 corresponds to numerous alleged sightings reported by Bob Stamps, who subsequently gained prominence as a purported bigfoot expert, appearing in various articles and radio broadcasts <a href="https://books.google.dk/books?id=sWsfAAAAIBAJ&pg=PA5&dq=bigfoot&article_id=1255,6281184&hl=en&sa=X&ved=2ahUKEwiaju7WmOWFAxUgLBAIHZfkBtEQ6AF6BAgJEAI#v=onepage&q=bigfoot&f=false" target="_blank">[4] </a> <a href="https://books.google.dk/books?id=_5gfAAAAIBAJ&pg=PA2&dq=bigfoot&article_id=1507,3144857&hl=en&sa=X&ved=2ahUKEwiaju7WmOWFAxUgLBAIHZfkBtEQ6AF6BAgFEAI#v=onepage&q=bigfoot&f=falsel" target="_blank">[5] </a>. The most recent spike, however, stemmed from a deliberate hoax, involving two individuals attempting to sell a purported bigfoot corpse for $25,000, which was later exposed as a costume stored in a freezer, perpetuated by Dyers and Whitton. <a href="https://books.google.dk/books?id=2RcqAAAAIBAJ&pg=PA3&dq=Bigfoot&article_id=6740,20897&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAQQAg#v=onepage&q=Bigfoot&f=false" target="_blank">Dyers</a>[2]  <a href="https://books.google.dk/books?id=7KgyAAAAIBAJ&pg=PA43&dq=Bigfoot&article_id=2608,3085237&hl=en&sa=X&ved=2ahUKEwjJrPr2seKFAxVdAxAIHUONCeM4FBDoAXoECAkQAg#v=onepage&q=Bigfoot&f=false" target="_blank">Duo</a>[3].  
        <br>
        <br>
This observation doesn't definitively affirm or debunk the existence of bigfoot; rather, it underscores a fascinating trend wherein bigfoot sightings tend to proliferate following widespread media coverage. This phenomenon may suggest heightened public interest in the subject, prompting more individuals to actively seek out potential sightings. Alternatively, it could indicate opportunists capitalizing on the hype, as exemplified by Dyers and Whitton's actions in 2003.
        <br>
        <br>
It's intriguing to note that the viral dissemination of information is not a contemporary occurrence; rather, it has historically fueled further media attention and subsequent public fascination with the subject.
    </p>
        <h2>How to find Bigfoot</h2>
            <div class="img">
        <h3>Figure 3:A plot of all counties in the US and their reported Bigfoot sightings</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/SocialDataFinal/assets/images/County.html"
            width="1025"
            height="550"
            >
    </div>
    <p>
The plot on figure 3 is a Cloropleth map of the USA with each county geo separated. From this we can locate areas of high bigfoot sightings. Interestingly we can see that the areas of the three famous bigfoot sightings previously discussed all have high report counts in their respective counties. We see that counties with the bigfoot footprints from 1958 have a high volume of bigfoot sightings of 31, with neighbouring countries having similar highs. The counties in question are close to the Rockies and have high amounts of mountainous and forested area.  This tells a very similar story to the other viral bigfoot sightings discussed. High bigfoot sighting density in respective and neighbouring counties. The washington area (top left) also features a large number of sightings likely due to its dense forests and rugged terrain, which provide ample hiding places for a creature like Bigfoot. Additionally, the Pacific Northwest has a long history of Bigfoot sightings and cultural stories surrounding the creature, further contributing to the high number of reports in that region. A zoomed in view of a heatmap for all reported sighitngs in that area can be seen on figure 4
 <div>
        <h3>Figure 4: A zoomed in view of the washington area from a heatmap</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/SocialDataFinal/assets/images/washington.png"
            width="1025"
            height="450"
            >
    </div>
        <br>
        <br>
Moving towards the Appalachian Mountains, we observe another cluster of counties with notable Bigfoot sightings. The dense forests and remote areas of the Appalachians offer similar habitat characteristics to those found in the Rockies, making them ideal locations for Bigfoot sightings.
        <br>
        <br>
Furthermore, the overlap between high sighting areas and regions known for outdoor recreational activities, such as hiking, camping, and hunting, suggests that human presence in these remote areas might contribute to the frequency of reported sightings. It's plausible that encounters with large, unfamiliar creatures in these environments could be misidentified as Bigfoot.
        <br>
        <br>
        However there is also a high density in counties of florida especially in the everglades which 
is a large wetland. This goes against the pattern observed in other areas of the US. On figure 5 a snippet of a heatmap of the everglades is shown on figure 5. 
 <div>
        <h3>Figure 5: A zoomed in view of the washington area from a heatmap</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/SocialDataFinal/assets/images/florida.png"
            width="1200"
            height="550"
            >
    </div>
    </p>
    <p>
    </p>
    <div>
        <h3>Figure 6: A heatmap showing all Bigfoot sightings for a given year</h3>
        <embed 
            type="text/html" 
            src="{{ site.baseurl }}/SocialDataFinal/assets/images/heatmap.html"
            width="1025"
            height="550"
            >
    </div>
    <p>
       On figure 6 a full heatmap is shown for each year of the reported Bigfoot sightings in the dataset. It includes  
    </p>
    <audio controls>
    <source src="{{ site.baseurl }}/SocialDataFinal/assets/images/Bigfoot_sound.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
    </audio>
    <h2>Concluding Thoughts on Bigfoot</h2>
    <p>
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
            <a href="https://books.google.dk/books?id=sWsfAAAAIBAJ&pg=PA5&dq=bigfoot&article_id=1255,6281184&hl=en&sa=X&ved=2ahUKEwiaju7WmOWFAxUgLBAIHZfkBtEQ6AF6BAgJEAI#v=onepage&q=bigfoot&f=false" target="_blank"> Search continues for Bigfoot </a>
        </li>
        <li>
            <a href="https://books.google.dk/books?id=_5gfAAAAIBAJ&pg=PA2&dq=bigfoot&article_id=1507,3144857&hl=en&sa=X&ved=2ahUKEwiaju7WmOWFAxUgLBAIHZfkBtEQ6AF6BAgFEAI#v=onepage&q=bigfoot&f=false" target="_blank"> Man, 27, Seeks Bigfoot </a>
        </li>
        <li>
            <a href="https://books.google.dk/books?id=_5gfAAAAIBAJ&pg=PA2&dq=bigfoot&article_id=1507,3144857&hl=en&sa=X&ved=2ahUKEwiaju7WmOWFAxUgLBAIHZfkBtEQ6AF6BAgFEAI#v=onepage&q=bigfoot&f=false" target="_blank">Man,27, Seeks Bigfoot</a>
        </li>
    </ol>
