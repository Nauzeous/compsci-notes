Pagerank is a trademarked algorithm developed by one of google's founders, Larry Page.

It is used to rank website pages and results returned by a search engine

Google and other search engines use many algorithms to rank search results, but PageRank is the first and most famous

It fundamentally works by checking the number and quality of links  to a page to determine how important the page is

The idea behind this system is that websites that are more important and reliable are linked to often

The quality of a link is dependent on how many links a webpage has - if a webpage has millions of links, it is unlikely that one link will have significant meaning

The pagerank algorithm is as follows

PR(A) = (1-d) + d (PR(T1)/C(T1) + PR(T2)/C(T2) ..... PR(Tn)/C(Tn))

or $$PR(A) = (1-d)+d\sum_{n=T1}^{Tn} PR(n)/C(n)$$
Each page starts with a pagerank of 1, and the process is iterated over. The process works iteratively to avoid circular dependencies.


## PR(Tn)/C(Tn)
PR(T1)/C(T1) represents the page rank of a page linking to A divided by the total number of links from the page
the maximum value for PR(T1)/C(T1) is 1 as if a page has only 1 link, to page A, you are doing (1/1)

the page rank over total links is summed over all websites which link to A

If websites that do not link to A are included, you would end up with $$PR(n)/0$$
resulting in a division by 0 error
## d

the letter *d* represents a dampening factor, preventing a single web page from having too much influence on the page rank

d is usually set to 0.85

(1-d) is a constant term added  to the pagerank to ensure a minimum pagerank, so all pages can have influence on another page's pagerank



