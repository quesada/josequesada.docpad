---
title: Technical reasons not to use google website optimizer (and Usability reasons too)
layout: post
tags: ['testing', 'abtesting','optimization','GWO']
date: 12/21/2012
---

AB testing shows multiple variations of your website and measures which
one leads to higher sales. If you have 100 visitors a day, AB testing
can turn 2 purchases into 12 purchases, all with the same amount of
daily traffic. Google Website Optimizer (GWO) comes from a company that
knows AB testing, most shopping carts support it via plugins, and is
free. How could this be a bad choice? The devil is in the details. I’ll
list a few reasons.

Ambiguous goal
--------------

GWO seemingly aims at two clients, the non-technical marketer, and the
technical person (who happily inserts javascript on their pages). But it
doesn’t serve either of them particularly well.

### The non-technical Marketing expert

GWO targets the non-technical marketer, since you do not need to write
code to use GWO. Since some small shops do not have technical talent in
house, and big shops have overloaded IT departments, not having to write
code is a big plus. Even in shops large enough to have an IT department
AND resources for AB testing, in our experience IT usually is pretty
isolated from the marketing department. Having the marketers do their
own tests is very empowering. If ease-of-use and simplicity are the
goals, then there are better, simpler tools. Even visual ones. Marketers
who want to run AB testing without code can use Optimizely or Visual
Website Optimizer. Optimizely goal is “to make it as easy as humanly
possible for you to create and run A/B tests on your site. All you need
to do is enter your website URL and point and click on what you want to
change. Absolutely no coding or engineering required. “ Visual Website
Optimizer is an excellent choice too. We just don’t see very many shops
actually using either of them, but we will cover this on another post.

### The programmer

Actually, the hipster term for a programmer tasked to do this work on a
website is ‘Growth hacker’ :) Turns out that for a ‘Growth hacker’ is at
a loss when using GWO. The ‘data scientist’ in your team won’t be very
happy either. GWO won't let you play around with the data they collected
for you.You will know that one variation performed better than the
other. You wouldn't know if one variation resulted in more time spent,
less advert clicks, more user interaction (in terms of comments), or
more purchases. And you won't know how it affected your overall funnel
behavior. The ‘Growth hacker’ will be the first to point out a bunch of
technical reasons in which it GWO fails short...

Technical reasons
-----------------

### Problems with dynamic sites

The ‘Growth hacker’ will not be happy with how GWO deals with dynamic
content. Google Website Optimizer does "in-line content replacement" of
tested elements. That's not a problem on static landing pages, but it's
a no-go on most dynamic sites. Which happen to be a majority on 2012’s
internet. In GWO, you end up essentially having to rewrite any variant
to be displayable in Javascript. pages where you have AJAX and Flash
elements are possible, but require workarounds.

### Two-url requirement

Using variation pages causes SEO and site problems when the test ends
unless you manage your server to produce 301 errors. So you'll either
need to keep the losers alive forever or set up redirects from each of
the losers to the winner every time you end a test. If being a lot of
server admin work was not enough, this has consequences for the test
results. The browsers loads two pages, and then it redirects to one of
the two alternatives. As a consequence, the marginal load for the
redirect to B artificially biases test results. Search engines penalize
duplicate content, which is exactly what you get when your two
variations, in independent URLs, are online. I believe google is smart
enough to detect the doings of its own product, and not penalizing GWO
users. But even without this penalty, putting the same content on two
URLs visible to users encourages them to link to both. Even after the
test declared it as a loser, the second url may need to stay around
forever. In fact, you risk to disappoint the users that bookmarked the
alternative which lost.

### Load time

Every time you do a test with two alternatives, it will cost you an
extra page load. With shoppers being extremely sensitive to [loading
times](http://www.hindawi.com/journals/ahci/2009/121494/tab2/), speed is
crucial. Causing an extra page load is just about the worst thing you
can do for page load speed.

### To Google Website Optimizer, all of your visitors are the same

In the current GWO, you cannot filter which users go into the test. Not
by search terms. Not by geography. Not by demographics.This goes against
the very essence of optimization. Using demographics for targeting
should be trivial, and a big honking feature for any testing software.
In fact, the web seems to start leaving behind demographics and focus on
psychographics. Times cannot be better for targeting. Consumer are
divided according to their lifestyle, personality, values... There are
some spectacular examples out there. Target could [predict that a teen
girl was pregnant before her father
did](http://www.forbes.com/sites/kashmirhill/2012/02/16/how-target-figured-out-a-teen-girl-was-pregnant-before-her-father-did/).
With some thought, and a good campaign, one can get incredibly accurate
targeting. Demographics help you understand who buys your product or
service, while psychographics helps you understand why they buy. Another
way to put it is that demographics are things that can be observed from
the outside, such as age and race, while psychographics are internal
attributes or attitudes. Still, GWO will not let you use your
hard-earned targeting results.

Usability reasons
-----------------

### Time it takes to set up a test

Using GWO, I feel It takes me too many steps to get to results. It
doesn’t feel productive. This is a reason why you often see Google
Website Optimizer only used on static landing pages and other non-core
site areas. As mentioned above, it just doesn’t work very well with
dynamic pages. That is, most contemporary CMS-based sites would have to
be ‘bypassed’ somehow. You'll need to manually create all of the
different pages you're going to test. But time is of issue not only for
the servers: the humans doing it in Javascript sacrifices convenience,
to a level that may make you too lazy to actually test things. For
example, deploying an AB test live on one of my sites took two minutes
(using a server-side test framework), but when I run experiments with
GWO it requires 15 minutes at a minimum.

### Dealing with tags

Google calls them "page sections." Omniture calls them "mboxes." They
define sections that you want to affect in your testing. For this
approach to work, you have to wrap tags around every variable area on
every page and/or template. If you make changes later, then you’ll have
to re-tag, re-QA, and push again your code. This is enough work to make
me think twice about doing any testing. I can see how shops, with
limited resources, struggle to do proper testing, or simply postpone it
to the mythical day ‘when we have more resources’. In sum, google
website optimizer’s usability would make
[Mordac](http://dilbert.com/strips/comic/2007-11-16/) proud.

Summary
-------

In our experience, Businesses see the value in A/B testing but they just
aren't doing it. If you, or anyone on your team, can program, it’s worth
looking at a server-side solution (more on this in another post). A
server-side solution will have several advantages:

-   It leads to faster loading pages, prevent horrible mistakes, and
    gives more flexibility to target your visitors, as we saw in
    ‘technical reasons’
-   It’s easier to set up tests, as we saw in the ‘usability’ section

Finally, all data stays in-house. If you ever come up with some better
analytic method, you can run it retrospectively. Google Website
Optimizer is a great product but if you are short on time and don't want
to muck with your code, look somewhere else. For more reviews, see
[this](http://mroptimization.com/multivariate-testing-and-targeting-vendors/multivariate-testing-with-google-website-optimizer-the-final-word)
(on multivariate testing). Why do we care? Soon, we will open up the
beta for fluidshopping, where we tackle this problem heads on. If you
feel your shop should be doing be doing more A/B testing, or just doing
it more efficiently, keep tuned. If you [give us your
email](http://fluidshopping.com/), we will let you know when it’s ready.
