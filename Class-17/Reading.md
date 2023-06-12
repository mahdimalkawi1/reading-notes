# Read: Class 17

## Web Scraping:

### Q1. What are the key differences between scraping static and dynamic websites?

Static websites have fixed content, while dynamic websites generate content on the fly. Static websites have predictable HTML structures, while dynamic websites have complex and changing structures. Scraping static websites involves retrieving pre-generated HTML, while scraping dynamic websites requires simulating user interactions and executing JavaScript. Scraping static websites is generally simpler and more stable, while scraping dynamic websites is more complex and prone to changes.


### Q2. Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.

1- Respect "robots.txt" to avoid restricted areas.

2- Introduce a delay between requests to mimic natural browsing behavior.

3- Rotate IP addresses and user agents to prevent detection.

4- Implement session management for authenticated websites.

5- Crawl politely and responsibly, avoiding overwhelming servers.

6- Monitor and adapt to changes in website structure or anti-scraping measures.

### Q3. What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

Playwright is a powerful Node.js library for browser automation and web scraping. It supports multiple browsers, provides automation capabilities, and excels at handling dynamic websites. A beneficial use case for Playwright is scraping data from JavaScript-heavy Single Page Applications (SPAs).

### Q4. Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.

XPath is used in web scraping to locate and extract specific elements from HTML. For example, the XPath expression //h1[@class='title'] selects an h1 element with the class attribute "title".