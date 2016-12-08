# view-all-facets

A Polymer Element showing a button that opens a dialog with checkbox-list-display elements.  This lets users view all facets in a separate dialog window if the number of facets is very large.  Can be used with the [elastic-checkbox-list-filter](https://github.com/DigElements/elastic-checkbox-list-filter) element to create elasticsearch filters.

### Example
```html
    <view-all-facets
        title="Country"
        buckets="[[countryResult.aggregations.countryAgg.countryAgg.buckets]]"
        loading="[[countryLoading]]"
        error="[[countryError]]"
        facet-selection="{{countryFacetSelection}}"
        agg-count="{{countryCount}}">
    </view-all-facets>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install
