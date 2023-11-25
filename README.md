# programming-language-data
Created for a talk "Evolution of Programming Languages". This contains data about programming languages, which languages influenced which other ones, which standards came first, and who might have been involved in the creation of those languages. It's a fascinating topic. Contained in this repository are the slides from the original presentation, and the data from the Neo4j database I used to create the graph in the last slide. This is what I want to see developed. Maybe there's a better graph database out there. Maybe Neo4j with Cypher can be better visualized with some other tool--I'd love to see this on a timeline. I'm sure there are mistakes in the dataset that need corrected. I know there are some Unicode character conversions that got screwed up when I was moving some of the data around, and those need to be fixed as well. Please submit pull requests in whatever way seems best. I'm adding all the files that seem relevant.

I have not seen this information presented in this way anywhere else on the web, which is why I decided to start compiling it myself, and I'll continue to work on it in my &lt;sarcasm&gt; ample &lt;/sarcasm&gt; free time. I think the information is valuable, and that this history could, and should, be compiled into a book, or set of books, or possibly as part of someone's dissertation. If that ever comes to pass, let me know, I'd love to read it!

## Getting Started

1. Find and download Neo4j Desktop [here-ish at the time of writing, requires registration](https://neo4j.com/product/developer-tools/)
2. Create new DBMS from languages.dump
3. Play with Cypher
4. Update/add info
5. Submit pull requests

## Limitations

- This database is not intended to include esolangs or "joke" languages. Did a few sneak in? Maybe. If you find one, note it, and remove it, unless it is somehow significant in the history and/or made a significant influence on another language. [INTERCAL](https://en.wikipedia.org/wiki/INTERCAL) might belong in the database as a first of its kind, for instance.
- The initial dataset contains some circular "influenced" references. This is usually when language A had a feature that language B liked, and language A decided to pilfer some other feature that language B had in a subsequent version, and so on. This happened a lot. Whether this should remain in the database or be separated by version is undecided at this time. Perhaps attributes can be added to the "influenced" relationships to specify what, when, and how, but that information may be hard to come by. I'm open to suggestion, but I also see this as a limitation of the data.

## Goals

- While the names in the initial dataset have "also-known-as" values in parentheses, it would be nice to be able to "search" the dataset with alternative names, with the most common name as the "one" that's shown most prominently.
- An interactive graph that can be browsed by anyone, from anywhere. Whether this is via a Neo4j Bloom public instance, or a Heroku app, or something else, is up to the individual who wants to design it. Have fun!

This information is licensed under [CC-BY-SA-4.0](https://choosealicense.com/licenses/cc-by-sa-4.0/). Do with it what you will, but people put a lot of time and effort into it, so remember that!
