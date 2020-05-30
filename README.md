# AUMSA-project-2
This is a Wordpress project created as a part of AUMSA 2020 submission requirement for my personal blog http://yeeiriser.azurewebsites.net/

Wordpress provides and hosts basic services and skeletons for creating a website. Users can modify the layout of the website by inserting code in php file.  However, for non-technical users, it is too intimidating and time-consuming to use this approach. Thus, Wordpress allows developers to create different kinds of both free and paid plugins which are beneficial to non-technical users in customizing the website and extending Wordpress functionalities beyond the basic without writing a code.
The problems exhibit on my Wordpress website ranging from the most important to the least are as follows:
1)	The message shown on search engine are automatically picked up by search engine’s algorithm which sometimes doesn’t tell the most interesting story of the article.
2)	Apart from visitor counts, web admin doesn’t have any deeper insights such as demographic-wise e.g. breakdown of visitors based on country of origin and type of device, or behavior-wise e.g. time spent on each page.
3)	When there’re too many pictures on the page, it takes longer to load. This will undermine user experience.
4)	Basic features and widgets provided on Wordpress are not engaging enough. You can write a plain text, highlight a quote, add picture, embed a video, but if you need more eye-catching features such as Carousel images, you’ll need a plugin to help.

According to the problems above, SEO plugin allows editor to specify the relevant messages which should be shown on search engine; Analytics plugin provide several metrics for audience insights; Cache management plugin can be configured to improved speed through cache and the use of lazyload image; and front-end page builder plugin has plenty of widgets and CSS enhancement features to customize the content presentation.
After researching from users’ feedbacks, my selections are as follows.
1)	SEO –Yoast and Rank Math are the among one of the top popularities due to their wholesome functionalities. Yoast is more complicated than Rank Math in terms of setting up and its free version might not be able to beat Rank Math as it still limits more advance feature for premium users. Though Yoast provides keyword optimization with preview interface both on desktop and mobile and the fact that it stays in the market longer makes it widely acceptable. It also provides content analysis based on blogger’s best practices such as low readability level due to frequent usage of a more than 20 words per sentence.
2)	Analytics – I end up using MonsterInsights rather than Analytify. Both of them can be integrated to Google Analytics – one of the most important features that other plugins don’t offer. Analytify seems to be slightly superior than MonsterInsights for premium users, as it’s claimed to be cheaper with similar level of functionality and also being able to dig into individual posts and pages. However, I’ve tried setting up the plugin, but there was a problem on authentication step on Google Webmaster, so I switched to MonsterInsights and it works.
3)	Cache management – similar case happened to the cache management selections as well. I chose to implement WP Total Cache at first because users heavily recommended this particular plugin claiming that it can offer up to 80% bandwidth savings. The only con side is that it is known to be ‘developer friendly’ plugin as there’re so many tech jargons under configuration. I’ve tried to configure the same way as suggested by bloggers; however, the cache somehow breaks my blog’s heading text on every page, and I couldn’t retrieve it. Thus, I considered using WP Super Cache as it provides similar functionality but comes in 3 modes including a simple mode for non-technical users and the least risky.
4)	Front-end page builder – I chose Elementor over Divi and Beaver mainly because it offers freemium, though covers more elements and pre-made templates. And apparently, it’s the most popular Front-end page builder among the three.

<b>The high-level steps of how you implemented each plugin.</b>

After install the plugins and activate them, next steps are summarized below.

Yoast SEO	
1. Go to https://www.google.com/webmasters and verify the website address.
2. Get the HTML tag and paste it on Yoast SEO setting.
3. The features will pop up at the bottom of the page of your draft.

MonsterInsights	
1. Under MonsterInsights’s Google Authentication setting, select ‘Connect MonsterInsights’ and it’ll prompt you to Google account.
2. Click ‘Allow’ to give access to Google Analytics dashboard.

WP Super Cache	
1. Under WP Super Cache setting, select ‘caching on’.
2. Under Advance tab, enable all of these: ‘use PHP to serve cache files’, ‘Compress pages so they’re served more quickly to visitors, Don’t cache pages for known users’, and ‘Cache rebuild’.

<b>The applicable benefits realized or expected to be realized after implementing each plugin.</b>
1)	Yoast SEO allows me to preview search result and edit the message I want Google to show accordingly. Readability also provides me comments about the content and how to improve it.
2)	MonsterInsights shows various metrics about audience behaviors.
3)	WP Super Cache makes the website loads faster.
4)	Elemontor allows me to build a carousel image, so it fits many pictures without taking up much space on the page. Example is in the middle of this page http://yeeiriser.azurewebsites.net/2020/05/27/the-mentalist/

