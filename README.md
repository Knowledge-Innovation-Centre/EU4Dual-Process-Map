# EU4Dual-Maps

HTML+CSS assets for the EU4Dual KPI dashboard. These files are embedded into the Zoho Creator app as embed widgets.

Config files used to append links to media items to corresponding SUB-SUB-PROCESSES

## Development

The HTML files fetch the list of documents/links from the corresponding JSON file using JavaScript Fetch API.

As a result, when opening the file locally (`file:///` URI), fetching works in Firefox but fails in Chrome, Safari, etc., due to CORS restrictions.

Workaround: do not open with a file URI but run a local server, e.g.:

```sh
docker run --rm -it -p 8080:80 -v /PATH/TO/LOCAL/REPO:/usr/share/nginx/html nginx:alpine
```

