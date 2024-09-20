# Buildings in Koblenz (Mapping Koblenz Project)

via [https://tinyurl.com/2843nwew](https://tinyurl.com/2843nwew)

```
#defaultView:Map
SELECT ?item ?itemLabel ?geo ?layerLabel WHERE {
  ?item wdt:P131 wd:Q922978.
  ?item wdt:P2 ?layer.
  ?item wdt:P48 ?geo.
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
} ORDER BY ?typeLabel
```

# Pharmacies in Koblenz (Mapping Koblenz Project)

via [https://tinyurl.com/26nwwdhp](https://tinyurl.com/26nwwdhp)

```
#defaultView:Map
SELECT ?Pharmacy ?PharmacyLabel ?Coordinate_location WHERE {
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
  ?Pharmacy wdt:P280 wd:Q480860;
    wdt:P47 wd:Q10399;
    wdt:P131 wd:Q922978.
  OPTIONAL { ?Pharmacy wdt:P48 ?Coordinate_location. }
}
```