# Unduck (but google is better)
> yeah i just added a !ubgib bang that adds `&udm=14&num=50`

> it's also the default

DuckDuckGo's bang redirects are too slow. Add the following URL as a custom search engine to your browser. Enables all of DuckDuckGo's bangs to work, but much faster.

```
https://unduck.rosi.host?q=%s
```

## How is it that much faster?

DuckDuckGo does their redirects server side. Their DNS is...not always great. Result is that it often takes ages.

I solved this by doing all of the work client side. Once you've went to https://unduck.rosi.host once, the JS is all cache'd and will never need to be downloaded again. Your device does the redirects, not me.
