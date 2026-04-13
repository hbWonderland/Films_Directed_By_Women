# Films Directed by Women
**A linked dataset of (almost) all films directed by one or more women from the inception of film to 1974.**

## Dataset Description
The dataset contains 111 records of films from 1896 to 1973, all directed by women. The films originate from countries across the globe, span a wide variety of genres and formats, and are funded both privately and by major studios.

I chose this dataset as an AFAB filmmaker myself with a background in film studies and critical theory. I thought this subject was interesting for scholars considering trends in film and global history, feminism, genre, funding, and more. I originally pulled this data from the Wikipedia article [List of films directed by women](https://en.wikipedia.org/wiki/List_of_films_directed_by_women), converting the html with custom Python code into a clean dataset. I still have all the films from 1973 to 2025 in my original spreadsheet, and hope to continue working on a larger linked dataset in the future.

Unfortunately, many films in the dataset published here are obscure, and several were removed due to lack of external linking options.

## Ontologies and Controlled Vocabularies
Schema.org, Wikidata, VIAF, Geonames, my own defined terms set (for genre, keywords, and format), XSD, RDFs

## Linking Strategy
Originally the goal with this collection was to use a healthy collection of links to: 
* VIAF
* EIDR
* IMDB
* Other databases


However, due to the obscure nature of many of these films, the linking strategy was:
* Wikidata for schema:Movie, schema:director, and schema:datePublished
* VIAF for schema:productionCompany
* Geonames for schema:countryOfOrigin

The budget and box office gross numbers are pulled from IMDB, but as literals they do not link to their source. Finally, for genre, subgenre/keyword, and format, I created my own defined term sets and hosted them on my website - there are notoriously few useful controlled vocabularies for physical film media and genres of critical and popular relevance.

## Sample Triples
* [Bury Me an Angel](https://www.wikidata.org/wiki/Q5001110) is a [Movie](https://schema.org/Movie).
* [Barbara Peeters](https://www.wikidata.org/wiki/Q4859217) is a [Director](https://schema.org/director).
* Bury Me an Angel was made in the [United States](https://www.geonames.org/6252001/united-states.html).
* Bury Me an Angel has the genre [Biker](https://andigraceson.media/tech/).
* Mono is a Format [Defined Term](https://andigraceson.media/tech/).
