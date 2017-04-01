# Improving Navigation-Based Internal links for SEO  

The way you structure and organize internal links plays an important role in how both users and search engines are able to navigate your website, ultimately impacting your website’s rankings.

Search engines like Google use links to crawl the web. The crawlers click on each link that appears on a page ( both internal links and external links ) and then all the links on each subsequent page, and so on. This allows the search engines to find your pages and rank them in their indices.

For this reason, the way you link the pages on your website plays a big role in how search engines crawl, understand and rank your site. How do you make sure your site architecture is optimal and that internal links are organized correctly? Let’s explore how calculating a metric I call Internal PageRank can help us with this task.

# Basic site architecture and navigation-based internal links 

There are two basic types of internal links: 
1. The internal links that form your site’s navigational structure 
2. The secondary internal links that appear in context throughout your site.

![strict-internal-linking-for-seo-800x449](https://cloud.githubusercontent.com/assets/4533327/24578475/ae414334-16e9-11e7-8168-f4e8f5289e78.png)

The first step to getting your internal links in order is to organize common navigation elements and adhere to a well-organized site structure. I recommend creating a classic internal linking structure and utilizing Bruce Clay’s silo architecture as a foundation for internal links.

## Step 1: Crawl with Screaming Frog

We need to crawl our website. For this example, I use Screaming Frog, as it is a standard tool in an SEO practitioner’s arsenal.

Start by launching Screaming Frog and crawling your website. When the crawl is finished, select Bulk Export > All Outlinks from the top menu, and save the CSV file to your desired location.

![screamingfrog-outlinks](https://cloud.githubusercontent.com/assets/4533327/24578508/3283ce46-16ea-11e7-8ed8-86825be64cc6.png)

The CSV contains a list of all the internal links on your website. We will use this list to create a network and calculate Internal PageRank.

## Step 2: Calculate Internal PageRank with R

Install the igraph library by launching the R console and executing:

install.packages("igraph")

Once the library is installed, you will be able to use the code in this account.

<img width="989" alt="screen shot 2017-04-01 at 3 15 47 pm" src="https://cloud.githubusercontent.com/assets/4533327/24578697/3b11138a-16ee-11e7-801d-08771e26c328.png">

## The output will be 

![cd-inlinks-screamingfrog](https://cloud.githubusercontent.com/assets/4533327/24578670/b8349bc6-16ed-11e7-9244-25cf4d0c06ac.png)
