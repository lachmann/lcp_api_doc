---
title: API v1
language_tabs:
  - ruby: Ruby
  - curl: Shell
language_clients:
  - ruby: ""
  - curl: ""
toc_footers: []
includes: [
  api/v1/wares,
  api/v1/vessels,
  api/v1/petrographics,
  api/v1/kilns,
  api/v1/shapes,
  api/v1/sites,
  api/v1/references,
  api/v1/periods,
  api/v1/period_categories,
  api/v1/images,
  api/v1/functional_categories,
  api/v1/contributors,
  api/v1/citations
]
search: true
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="api-title">API v1</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

Base URLs:

* <a href="https://www.levantineceramics.org/">https://www.levantineceramics.org/</a>

<h1 id="authentitation">Introduction</h1>
_The Levantine Ceramics Project_ (LCP) is an open, interactive website focused on ceramics produced in the Levant from the Neolithic era (c. 5500 B.C.E.) through the Ottoman period (c. 1920 C.E.). Here you can submit and find information—whether long published or newly discovered—about ceramic wares, shapes, specific vessels, scientific analyses, kiln sites, and chronology. The LCP makes it simple to access, share, use, and refine data, to link scholars and to foster collaborative research. **Watch a brief video about the LCP** [here](https://www.youtube.com/watch?v=kFk_7f4B1vY).

<h1 id="authentitation">Authentication</h1>
<aside class="warning">
  Every endpoint requires authentiation
</aside>

The Levantine Ceramics Project expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer <token>`
