<img width="950" height="300" alt="Google Scraper tool" src="https://github.com/user-attachments/assets/7ac3e726-4ff9-424e-808b-f8f6816888ab" />

# Google Scraper
Scrape Google with a simple API. It includes Google Search, Google Maps, Google Shopping, and more!

We return the results in a nice, structured JSON. No more parsing, coding, proxy, or other web scraping headaches for developers.

<img width="1382" height="948" alt="Google Scraper Playground example" src="https://github.com/user-attachments/assets/aa91aea9-eaca-472e-9134-cf922caecfc2" />

## How to scrape Google?

Using a simple GET request, you can access all Google search engine results:

```
https://serpapi.com/search.json?q=Coffee&engine=google&api_key=YOUR_API_KEY
```

- Register for free at [SerpApi](https://serpapi.com?utm_source=github_google_scraper) and get your API Key
- Endpoint: `https://serpapi.com/search.json`
- If you don't define the `engine`, it defaults to `google`. You can replace the value with any engine you need. For example, `google_maps` for Google Maps scraper.
- Each of this engine have many optional parameters to refine your search.

## Available Google Search Engines

We provide different engines, like:
- Google Search API
- Google Maps API
- Google Shopping API
- Google Images API
- Google Videos API
- Google News API
- Google Autocomplete API
- Google Local API
- Google Scholar API
- Google Trends API
- Google AI Overview API
- Google AI Mode API
- Google Flights API
- Google Lens API
- Google Events API
- Google Hotels API
- Google Reverse Image API
- Google Finance API
- Google Patents API
- and more!

## Code examples
Here are some code examples based on your favorite programming languages.

### Python Integration Example

Preparation for accessing the SerpApi API in Python

- Create a new main.py file
- Install [requests package](https://pypi.org/project/requests/) with:
```
pip install requests
```

Here is what the basic setup looks like:

```
import requests
SERPAPI_API_KEY = "YOUR_REAL_SERPAPI_API_KEY"

params = {
    "api_key": SERPAPI_API_KEY, #replace with your real API Key
    # soon
}

search = requests.get("https://serpapi.com/search", params=params)
response = search.json()
print(response)
```

With these few lines of code, we can access all of the search engines available at SerpApi, including the Google Search API.

Here is how to scrape "Google Search" results.
```
import requests
SERPAPI_API_KEY = "YOUR_SERPAPI_API_KEY"

params = {
    "api_key": SERPAPI_API_KEY, 
    "engine": "google",
    "q": "coffee"
}

search = requests.get("https://serpapi.com/search", params=params)
response = search.json()
print(response)
```

### JavaScript Integration Example

Install the [SerpApi JavaScript package](https://github.com/serpapi/serpapi-javascript):
```
npm install serpapi
```

Run a basic query:

```
const { getJson } = require("serpapi");
getJson({
  api_key: API_KEY, // Put your API Key
  engine: "google",
  q: "coffee"
}, (json) => {
  console.log(json["organic_results"]);
});
```

### Other Programming Languages
While you can use our APIs using a simple GET request with any programming language, you can also see our ready-to-use libraries here: [SerpApi Integrations](https://serpapi.com/integrations?utm_source=github_google_scraper).

## Blog tutorial 
for advanced usages
- pagination
- ...

## Video tutorial
...

## Nocode method
We also offer no-code solutions for scraping Google.

- [NoCodeSerpApi](https://nocodeserpapi.com/)
- [n8n X SerpApi](https://serpapi.com/blog/tag/n8n/)
- [Make X SerpApi](https://serpapi.com/blog/tag/make/)
- [and more integrations](https://github.com/serpapi/serpapi-integrations/)

## Contacts
Feel free to reach out via `contact@serpapi.com`.


