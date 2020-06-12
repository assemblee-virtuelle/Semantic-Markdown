# Idea _to find a solution that will be silently ignored by normal Markdown processors_

_or **almost** ignored..._

**Use referenced links _(cf.[commonmark.org])_**

`Tomorrow I am travelling to [Berlin][Place]`

gives

Tomorrow I am travelling to [Berlin][Place]


**For titles**

    ### [European Semantic Web Conference][Event]
    Lorem ipsum..
	
gives

### [European Semantic Web Conference][Event]
Lorem ipsum..

**For URI**

    Tomorrow I am travelling to [Berlin](https://www.wikidata.org/wiki/Q64)
   
gives

Tomorrow I am travelling to [Berlin](https://www.wikidata.org/wiki/Q64)

but think to add a footnote for `[Berlin]`

Example of footnotes :

    [schema]: http://schema.org/  
    [rdfs]: http://www.w3.org/2000/01/rdf-schema#  
    [Place]: http://schema.org/ ".schema:Place"  
    [Event]: http://schema.org/ ".schema:Event"  
	[Berlin]: http://schema.org/ ".schema:Place"


[commonmark.org]: https://spec.commonmark.org/0.29/#link-reference-definitions

[schema]: http://schema.org/
[rdfs]: http://www.w3.org/2000/01/rdf-schema#
[Place]: http://schema.org/ ".schema:Place" 
[Event]: http://schema.org/ ".schema:Event" 
[Berlin]: http://schema.org/ ".schema:Place"
