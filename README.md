“Soft navigations” are user-initiated but JS-driven same-document navigations.
* The Soft Navigation API considers a "soft navigation" when the following occurs:
*   A user-initiated interaction occurs, which results in DOM modifications that lead to sufficiently contentful paints, and a URL update occurs, which changes the history state (via **history.pushState**)

Here's the site I created: https://hard-soft-navigation-test-site-on-v.vercel.app/index.html
* Vercel: https://vercel.com/confusedpenguin59-2399s-projects/hard-soft-navigation-test-site-on-vercel

**Reference:**
* Source: https://github.com/WICG/soft-navigations?tab=readme-ov-file#overview
* For testing, refer to here: https://github.com/WICG/soft-navigations?tab=readme-ov-file#i-want-to-take-this-for-a-spin
* For debugging, check:
  *  chrome://settings/help (at least v144 Chrome)
  *  Inspect > Application > Frame > Origin Trails - to confirm SoftNavigation API is enabled

