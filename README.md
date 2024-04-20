<h1 align="center"> ✨ fresh-fork | <a href="https://hugo-fresh.vercel.app">Demo</a> | <a href="https://stefma.github.io/hugo-fresh">Documentation</a> ✨ </h1>
<p align="center">A Fresh Fork of the Fresh theme for Hugo</p>


**Fresh** is a theme for the [Hugo](https://gohugo.io) static site generator adapted from the gorgeous, [Bulma](https://bulma.io)-based theme of the same name from [CSS Ninja](https://cssninja.io/product/fresh). You can find a live demo of the original theme [here](https://fresh.cssninja.io/) and a live demo of the Hugo theme [here](https://hugo-fresh.vercel.app).

## Fresh Fork for more Freshiness

The original fresh theme did not provide the look and feel of the desired result, and it did not provide
all the desired features either. Due to the fresh theme's flexibility of modularity, it was forked
and customized to suit our needs.

### Reording Sections

Below is an index for reference of the reordering of sections

| Original | Old Custom | New Listing |
| ---------| -----------| ------------|
|  1       | 1          | 1           |
|  8       | 8          | 2           |
|          | 2          | 3           |
|          | 6          | 4           |
|          | 7          | 5           |
|          | 3          | 6           |
| N/A      | timeline   | timeline    |
|          | 9          | 7           |
| 4        | 4          | N/A         |
|          | 5          | 8 (N/A)     |

```html
	<!-- Old section 1 -->
    {{ partial "section1" site.Data.section1 }}
    <!-- old section 8 -->
    {{ partial "section2" site.Data.section2 }}
    <!-- old section 2 -->
    {{ partial "section3" site.Data.section3 }}
    <!-- old section 6 -->
    {{ partial "section4" site.Data.section4 }}
    <!-- old section 7 -->
    {{ partial "section5" site.Data.section5 }}
    <!-- old section 3 -->
    {{ if .Site.Params.section6 }}
    {{ partial "section6.html" . }}
    {{ end }}

    {{ partial "timeline.html" site.Data.timeline }}
    <!-- old section 9 -->
    {{ partial "section7" site.Data.section7 }}

    <!-- {{ if .Site.Params.section4 }}
    {{ partial "section4.html" . }}
    {{ end }} -->
    
    <!-- old section 5 -->
    {{/*  {{ if .Site.Params.section8 }}
    {{ partial "section8.html" . }}
    {{ end }}  */}}
```

![Fresh theme logo](images/screenshot.png)
