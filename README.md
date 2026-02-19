“Soft navigations” are user-initiated but JS-driven same-document navigations.
* The Soft Navigation API considers a "soft navigation" when the following occurs:
*   A user-initiated interaction occurs, which results in DOM modifications that lead to sufficiently contentful paints, and a URL update occurs, which changes the history state (via **history.pushState**)

Here's the site I created: https://hard-soft-navigation-test-site-on-v.vercel.app/index.html
* Vercel: https://vercel.com/confusedpenguin59-2399s-projects/hard-soft-navigation-test-site-on-vercel

**Reference:**
* Source: https://github.com/WICG/soft-navigations?tab=readme-ov-file#overview (**token expires Mar 9, 2026**)
* For testing setup, refer to here: https://github.com/WICG/soft-navigations?tab=readme-ov-file#i-want-to-take-this-for-a-spin
  * For local testing, put all these files in a single directory. Then run python3 -m http.server (or https.server - I forget), then visit [http://localhost.](http://localhost:8000/index.html) (Note: Vercel does all of this automagically. Just upload your updated files, and that's it. Instant update.)
* For debugging, check:
  *  chrome://settings/help (at least v144 Chrome)
  *  Inspect > Application > Frame > Origin Trails - to confirm SoftNavigation API is enabled


