# pawl

How can we get more detail about content sharing at a per-pageview level?

- On page load, record and increment the URL hash with a random string
- Create a directed graph of these events. Each edge is `(page_load_hash, incremented_hash)`
- Combine with referer, cookies

This data is useful in understanding the relationships between no-referer sources (email, IM) and social sources. Other potentially interesting metrics include share depth and influencer identification.
