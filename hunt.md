##HTTP Response Scavenger Hunt

####Assignment

For this Lab you will be making HTTP requests in your terminal using **curl** and scavenging for data in the response you get back. **curl** is short for "Client for URL's" and is a tool that allows us to make HTTP requests in our terminal.  

___________________________________________

**Phase 1: Make a GET request to google**

In terminal:

`curl -v https://www.google.com`

Find your response header

  - What status did you get back?
  - What content-type did you get back?
  - What came after the key "Set-Cookie"?
  - What date did this request come back on?
  - What came after the key "Transfer-Encoding?"

Find your response body

  - What was the first line in your response body?

_______________________________________________

**Phase 2: Make a GET request to the OMDBAPI**

In terminal:

`curl -v http://www.omdbapi.com`  

Find your response header

  - What status did you get back?
  - What content-type did you get back?
  - What was your content length?
  - What date did this request come back on?

Find your response body

  - What was the first line in your response body?

___________________________________________________

**Phase 3: Make a GET request to the OMDBAPI with parameters**

In terminal:  

`curl -v http://www.omdbapi.com/?s=Titanic`

Find your response header

  - What status did you get back?
  - What content-type did you get back?
  - What was your content length?

Find your response body

  - Look at the data that came back. What data structures do these look like?
  - What year did Titanic II come out?

_______________________________________________________________________

**Phase 4: Make a GET request to the OMDBAPI with different parameters**

Now search for one of your favorite movies.

`curl -v http://www.omdbapi.com/?t=<insert your favorite movie here>`

*If the title of your favorite movie has spaces, replace these with %20*  
i.e. `curl -v http://www.omdbapi.com/?t=the%20matrix` 

Find the response header  

  - What was the Cache-Control?
  - What value is after the key Expires?

Find the response body

  - What year was your favorite movie released?
  - What was your favorite movie rated?
