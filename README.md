DBpedia_HITS_Scores
===================


##Source Dataset


DBpedia_PageLinks_Cleaned Dataset (3.9) is used to compute Hubs and Authority(HITS) scores. More details about DBpedia_PageLinks_Cleaned Dataset and how it is created can be found [here](http://semanticmultimedia.org/node/6).


##Implementation

JUNG — the Java Universal Network/Graph Framework is used to compute HITS score. JUNG is a software library that provides a common and extendible language for the modeling, analysis, and visualization of data that can be represented as a graph or network. 

You can get the soucre code at [JUNG HITS Implementation](https://github.com/dineshreddykdp/JungGraphMeasures)

Parameters used while computing HITS

```
No of iterations: 100 //Number of iterations used before terminating
Tolerance: 0 //Minimum change from one step to the next
Alpha: 0.15 //the probability of a hub giving some authority to all vertices, and of an authority increasing the score of   all hubs (not just those connected via links)
```
##Citation

If you are using this dataset please cite as:

```
{dbpedia-graphmeasures,
  Author = {Dinesh Reddy},
  Title = {DBpedia GraphMeasures},
  Location = {http://semanticmultimedia.org/node/6},
  Resource type = {dataset},
  Publisher = {Hasso Plattner Institute},
  Publication date = {July 2014},
}
```
##Details of the datasets


Details | English | German
------- | ------- | ------
Number of Triples(resources) | 4984633 | 1689764
File Memory | 71 MB | 24.2 MB
Format | Turtle | Turtle



##Schema 


Top 5 resources with high HITS scores from DBpedia_page_links_cleaned_English Dataset

```
<http://dbpedia.org/resource/List_of_University_of_Pennsylvania_people> <http://dbpedia.org/ontology/wikiHITS> "0.005060736032883985"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/List_of_primate_cities> <http://dbpedia.org/ontology/wikiHITS> "0.004795846442805017"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/Demonym> <http://dbpedia.org/ontology/wikiHITS> "0.0045679803080603465"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/History_of_Western_civilization> <http://dbpedia.org/ontology/wikiHITS> "0.00451331484186086"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://dbpedia.org/resource/List_of_Irish_exonyms> <http://dbpedia.org/ontology/wikiHITS> "0.004389936643258905"^^<http://www.w3.org/2001/XMLSchema#float> .
```

Top 5 resources with high HITS scores from DBpedia_page_links_cleaned_German Dataset

```
<http://de.dbpedia.org/resource/1974> <http://dbpedia.org/ontology/wikiHITS> "0.005532562545603328"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/1981> <http://dbpedia.org/ontology/wikiHITS> "0.0055152634545923345"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/1946> <http://dbpedia.org/ontology/wikiHITS> "0.0053877619872892205"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/2006> <http://dbpedia.org/ontology/wikiHITS> "0.0052940707715464575"^^<http://www.w3.org/2001/XMLSchema#float> .
<http://de.dbpedia.org/resource/1945> <http://dbpedia.org/ontology/wikiHITS> "0.005256885176742795"^^<http://www.w3.org/2001/XMLSchema#float> .
```
