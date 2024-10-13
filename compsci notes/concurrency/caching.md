caching is an example of how thinking ahead is implemented in computer architecture

caching results greatly improves the speed of a program, as instructions dont need to be fetched from secondary storage

although it is quicker to access items from main memory than secondary storage, it is even faster to access items from registers on the processor

an advanced version of the concept is ==prefetching==, which involves data being requested from the main memory before it is required


as **prefetching** is predictive, it  requires a **probabilistic** algorithm to predict when a piece of data will be needed

Caching is also used with web pages to reduce the number of requests from the client to the web server and vice versa

Although caching improves speed and efficiency, the probabilistic nature means that you can have frequent **cache misses** and when the wrong data is fetched, it has to be removed/**flushed**
