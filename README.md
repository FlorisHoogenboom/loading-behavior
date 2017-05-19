# Loadingbehavior

Provides simple functionality to keep track of multiple loading elements.

When getting started with Polymer I often encountered the problem of having a component that loads data from multiple different sources. In many cases the databinding functionality did not completely fulfill my whishes, namely: to keep track of all elements and expose a single property to the outside.

## Examples
Include the behavior in your element. Then, any element that itself exposes a loading property can be monitored by setting `loadingChanged` as the event listener to the *on-changed* event of that property. E.g. for `iron-ajax`:

```html
<iron-ajax
  auto
  url="..."
  on-loading-changed="loadingChanged"></iron-ajax>
```
