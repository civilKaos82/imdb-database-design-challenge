# Schema Design: Internet Movie Database 
 

## Summary 
Are we familiar with the Internet Movie Database (IMDb)?  If not, well, it's a database ... a database that contains a whole slew of data related to movies.  Titles, directors, producers.  It's all there.  Users are able to interact with this database in different ways, including the website [imdb.com][].

In this challenge, we're going to look at the imdb.com website and infer the schema of the database.  For example, take a look at the [full cast and crew][imdb sharknado 3] for a movie.  What can we deduce?  The database stores data about movies:  the title, release date, etc.  It stores data about people, like their real names.  It associates people with movies, noting their roles and if the role is being a cast member, the character's name.

Now we know a little bit about what data is in the database, but what does the schema look like?


##Releases

###Release 0 : Design schema

Requirements:

1. A person has a first and last name
2. A person has many roles
3. A person with a roles is in a movie (e.g., "Producer of X", "Supporting Actor in Y")
4. A movie has a title, rating, and release date
5. A movie has a genre, and a genre has many movies
6. A person can have awards, and awards can be won by multiple people (e.g., "Best Actor" is an awards, won by someone in 2010 and 2011)


Design a database schema for IMDB that meets the requirements.

Use [SQL Designer](https://schemadesigner.devbootcamp.com/) to create your schema.  When you are done, save the XML of your schema and copy it into the source file `imdb.md`. Then, take a screenshot of your final schema design, and upload it using a free image-upload service like [Min.us](http://minus.com).  Paste the URL of the screenshot into your source file (before your XML code). 


<!-- ##Optimize Your Learning  -->

##Resources


* [SQL Designer](https://schemadesigner.devbootcamp.com/)
[imdb.com]: http://www.imdb.com
[imdb sharknado 3]: http://www.imdb.com/title/tt3899796/fullcredits?ref_=tt_ov_st_sm