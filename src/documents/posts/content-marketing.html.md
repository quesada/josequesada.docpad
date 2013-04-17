---
title: How to blog data-driven to maximize impact, using competitors' social data and special google searches 
layout: post
tags: ['blogging','strategy', 'data-science', 'content-marketing']
date: 02/27/2013
---

I'm sure you have thought a lot about getting traffic from google searches by writing content. This is content marketing the safest way (for now) to acquire links. Google employs PhDs to prevent most SEO tricks, and because of that SEO best practices change from time to time. But focusing on excellent content is a safe bet, since most other methods have a high risk of being detected algorithmically. 

The way I see it, there are two problems you need to solve: (1) how to find good topics that your audience craves, and (2) how to get others to link to you. Let's try to answer these questions with data, as it should be :).

What comes next is a how-to to blog in a data-driven way. The hacks may seem too simple to actually work, even naive. But applying these systematically will get you results; and results you can measure. Try them for a week, and compare it with your previous blogging routine. This stuff relies on (1) collecting data from content nearby that is liked, so you can write similar posts, and (2) special google searches to get links.

There are many blog posts on [blogging strategy](http://www.problogger.net/archives/2008/12/10/you-need-a-blog-strategy/). But I haven't found actionable advice that is data-driven on a single post. Here is my attempt to write such a post for you.

##What to write

###The effect table
If you are a stand-up comedian, you get immediate feedback as you perform. This helps you morph your story on the fly, do more of what works. But since there's no record of what people laughed at in the last 6 months... your guesses are limited to the time slice they are looking at you on stage. The more data you have, the better your guesses will be. As a blogger, you have an even better superpower: you can tap into what your audience likes not only when you write, but when others write. And then use this information to target exactly what your audience likes like a heat-seeking missile. I'll show you how.

We are going to create a table that gives you clarity that few bloggers have (unless they possess super-human intuition). We will use it to make decisions for all the key questions on the rest of the post.

(Credit: I got this idea from Neil Patel's mailing list, but I have added my own twist).

**I call this the 'effect table'**. Let's put in it anything that answers the question: 'are my efforts having the effect I want, and if so, how much?'

1. Create an spreadsheet that lists all your competing blogs.

2. For each post, you want to get an idea about how much their readership liked the content. Nothing better than counting tweets, facebook likes and all the obvious social submissions. You can automate this by using [sharedcount](http://sharedcount.com/). Take the url and paste it in the textbox. Since you want to do this for multiple urls, you could use their 'multi-url dashboard'.  The last time I tried, the table didn't render on chrome 25; it does work on firefox, but the rendering is sloppy (headers are to the right of the table, columns are not aligned. It doesn't matter, because what you need is the 'export to CSV' function, and this works great. You will get something like the table below. I used two random posts; you should use the most recent posts from your competitors, or pundits you follow in your field.

3. This technique will show you clearly which topics will get your audience engaged. You can write content related to those topics and they'll  likely outperform topics that you generate 'by hunch'. It's kind of scary how most bloggers, your competitors included, will be just be following 'what they personally like' as a compass for writing. While the human brain is pretty good at detecting trends, it's never a bad idea to supplement its capacity with hard numbers. This is the power of a data-driven blogging strategy.

Following what the data tells us also increases our chances of writing a big hit. And it works wonders for writer's block.
 

 <table class="pretty-table" summary="Social media data for two random posts.">
 
<tr><th scope="col">URL</th><th scope="col">FB Likes</th><th scope="col">FB Shares</th><th scope="col">FB Comments</th><th scope="col">FB Total</th><th scope="col">Tweets</th><th scope="col">+1s</th><th scope="col">Diggs</th><th scope="col">Pins</th><th scope="col">LinkedIn Shares</th></tr>

<tr><th scope="row"><a href="http://newscenter.berkeley.edu/2013/03/25/robert-wilensky-dies-at-61/"> Wilensky dies at 61</a></th><td>1</td><td>6</td><td>0</td><td>7</td><td>48</td><td>3</td><td>0</td><td>0</td><td>0</td></tr>

<tr><th scope="row"><a href="http://irce.internetretailer.com/2013/"> Iretailer conf</a></th><td>62</td><td>12</td><td>7</td><td>81</td><td>10</td><td>0</td><td>0</td><td>0</td><td>6</td></tr>
</table>

<br>

Some other data you can add is 'number of comments' on the post, and 'Hacker news votes' if the story was submitted to hacker news.  

One small detail: bear in mind that post date matters.

The date is often in the url, so no need to add a different column. Comparing a 3yo post with one out for a day is wrong because the older post has had more time to collect mentions and likes. This is even more of an issue for evergreen content. However, for normal, newsy stuff, after a week of social media swirl counts are stable.

### Should you stay on topic, blogging only relevant stuff for your audience?

When blogging, do you need laser focus on your audience's pain points? i.e., are detours damaging? Is every blog post that fails to hit their pain deducting from your perceived expertise?

This is a question I struggle with myself. Most of the posts I'd like to write are highly technical. To date I have not attempted to write posts with formulas, or complex graphs, because they do not work as well as more 'marketer friendly' posts (I learnt this by using the effect table).

I don't have data, but every time a member of your audience checks his mail or rss reader, to find a post that has NOTHING to do with his problems or one too advanced for his level, you are in danger of losing him. Although a sparkling of tangential posts is ok, be careful. Survey your audience, they might tell you when you were blogging something they didn't care about. And of course, look at your engagement data. Are they commenting? Retweeting? Each audience is different, though. You can test yours, with the effect table.

But what do you do with those posts you have in your scratch box that are great, but not super-targeted for your audience? I recommend to post them in social media sites. I'm covering this next.

### How long?
How long should a post be? Above 2000 words gets the best google rankings, and the most backlinks.

The [serpIQ](http://blog.serpiq.com/how-important-is-content-length-why-data-driven-seo-trumps-guru-opinions/) blog analyzed the top 10 search results for over 20,000 keywords and noticed a pattern.

The average content length for a web page that ranks in the top 10 results for any keyword on Google has at least 2000 words. And the higher up you go on the search listings page, the more content each web page contains.

![picture alt](/images/optimal-post-length.jpg "Optimal post length")   

##Where to write

###Should you post on your own blog, or do a guest post?

Guest posting involves writing an article and publishing it on a web site owned by another publisher. They get a free article and you get a free link. Unfortunately, this technique is very close to paying for links -a very large violation of the Google Webmaster Guidelines. You aren’t paying for links with cash, but you are effectively paying for links with writing work. However, this is still in the spirit of what google stands for: making a better web. So I think guest posting is safe, and will be in the near future.

By making strategic partnerships with other bloggers, you can produce content and put it in a great location. But how well does it work?

You can check: 

1. Audience match. How well does the audience of the other site match your audience or the audience you hope to build?

2. Site popularity. How large an audience does the other site have? How many people will see your content?

3. Audience activity. There are some audiences that are simply more active online. Programmers, for example, all have blogs and a good twitter following.

4. Average effect. If you stick the last 5 posts from the host blogger in the effect table, ... are the numbers something you'd want to see on your own content?

5. Authority. are search engines likely to see the site as an authority? Are your readers? This correlates with their average effect, but it's not only how much they propagate on the net. How popular a post is is not necessarily related to how authoritative it is. If you have doubts, think LOLcats. They would score high on effect, but low on authority.

Finding data about the relative contribution of guest posting is challenging. The ideal situation would be to check your referrer stats, but this only works if you guest-blogged there at least once.  

Taken to a extreme, maintaining your own blog may not be necessary. Some don't even run an own blog, but build a following by guest posting. One example is @FAKEGRIMLOCK, an anonymous poster than writes in all caps and copies the primitive grammar of a robot T-rex. Why his persona is so effective is material for another post. He started commenting on Fred Wilson's AVC blog, then got invited to guest post, then moved on to a solo career that includes a book and a blog. But climbing the fame mountain by commenting on other people's blogs is exceptional.

###How much do you need to blog in-house? 

1. Enough to make sure a future blogger host sees your content as valuable for his audience. Writing a quality post for another blogger is a great way to network with that blogger. But you must demonstrate that you are a worthwhile person to talk to, and this happens in your own blog.

2. Enough so that followers from your guest post find it a good place to stay. Ideally after having seen your guest article people will follow you back to your home base, your site, and read more.

###Should you post in quora, g+, LinkedIn, etc?

Sometimes you have content that just doesn't fit the 'persona' in your blog. I wonder if having posts that are all over the place will damage the type of 'highly targeted' blog that would convert the most.

A great way to test this would be to make an experiment. Take two bloggers with similar audiences (say 1000 active readers); Let one of them be laser-focus, posting twice per week only on-topic. Let the other one post more (3 times per week), but rambling a bit. Check the engagement numbers. Which one you think has growh a better, more responsive audience?

While I have no data on this, I suspect the always-on-topic blogger would have a better audience. I'd love to run such an experiment, though.

So what to do with posts that would break the flow on your own blog? Post them on these social media sites. You should try an effect table for your quora, g+, LinkedIn, etc. It might be that one of these channels even outperforms posting on your own blog. LinkedIn seems useful for showing off professional expertise.

## How to get links

There are many creative ways to build links, but we will stick to the basics for now. Let's say that: 

- (1) You can guest post, which obviously produces at least a link back to your main site.,
- (2) ... and you can use sites that like to link to resources like yours.

(Credit: I got this idea from Rob Wailing's mailing list.)


### Find blogs that take guest posts

One of the hardest tasks for guest posting is finding blogs that allow guest posts.

One trick is to use Google syntax you can narrow down your list to blogs that accept guest posts.

Here are the two searches you would run:

	inpostauthor:guest [your market]
	inurl:category/guest [your market]

<br>

So for example,

	inpostauthor:guest sport clothes
	inurl:category/guest sport clothes
<br>

This query would search for web sites that talk about "sports clothing" and have a links page. Which is what you want to do if you are looking to build links to a sports clothing website 

Now, it may be to your advantage to write on your own blog, and get sites to link to you. Or you may want to produce links for a guest post (a bit of a stretch, but this could be a reasonable thing to do).

You should add your guest posts to a table similar to the one in the 'What to write' section. Compare stats with posts on your own blog, and with posts by the host. Are they performing better than the host's average? Tell him that the next time you want to get featured.

While finding the right places to guest post could be outsourced, I'd try to follow the blog for a while. Consider whether the topic that you’re writing about has been covered before - or at least covered recently. Darren Rowse from Pro-Blogger prefers aspiring guest bloggers to contact him _before_ writing the post. Check of they have any recommendations for guest bloggers before commiting time to it.

Are your guest posts working for you? Remember coming back to your guest posts say a month later, and add them to your effect table.

### Find sites that like to link to resources like yours

You need to find all sites that have a links section, and that are in your ballpark content area. Here's the search command I would use on Google:

	intitle:"sport clothes" inurl:"links"
<br>
For each result I found, I'd send a custom email to see if they would be interested in linking to my website.

You can get ~ 10-15% of the websites you email to link back to your website. This is a task that any VA can do for under $10/hr. So even if you get only one backlink per hour, it's not a bad price, assuming the quality of the sites you email is high. Launch your favorite backlink analysis tool and check out that blog’s links. A higher number of quality links indicates a healthier blog.

For more creative ways of link building, a great place to look is [inbound](http://inbound.org). 

These special queries will only get more powerful as google indexes more Semantic Markup. You can filter by date of post, by location, ... and maybe one day by product mentioned in the article.

The biggest mistake you can make is not to measure the results. If you apply any of the advice above, and it makes a big splash in your bottom line, I'd love to hear about it.

