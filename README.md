# view-all-facets

An element providing a way to view all facets in a dialog if number of facets is very large. Used with elastic-checkbox-list-filter
to create elasticsearch filters.

Example:
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

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

