# Read: Class 17

1. **What are the key differences between scraping static and dynamic websites?**

Key Differences Between Scraping Static and Dynamic Websites:

Static Websites: These websites deliver the same content to every user and are usually built with HTML and CSS. Scraping static websites is relatively straightforward, as the content is present in the HTML source code, and tools like BeautifulSoup can be used to extract information.

Dynamic Websites: Dynamic websites use client-side scripts (often JavaScript) to load content dynamically, altering the HTML after the initial page load. This makes scraping challenging, as the data you want might not be present in the initial HTML source. Selenium and Puppeteer are commonly used tools for scraping dynamic websites as they can simulate user interactions and capture dynamically loaded content.

2. **Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.**

Respect Robots.txt: Check the website's robots.txt file to understand which parts of the site are off-limits for web crawlers. Always abide by the rules specified in this file.

Use Headers: Mimic the headers sent by a web browser to appear more like a legitimate user. This includes setting a user-agent header to simulate a common web browser.

Rate Limiting: Avoid making too many requests in a short period. Implement a delay between requests to simulate human behavior and reduce the likelihood of being detected as a scraper.

3. **What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.**

Playwright: Playwright is a Node.js library that provides a high-level API to automate web browsers, including Chrome, Firefox, and WebKit. It allows for browser automation and is useful in web scraping tasks, especially those involving dynamic websites.

Use Case: Playwright can be beneficial when scraping websites that heavily rely on JavaScript to load and render content. It can interact with the page, wait for asynchronous actions to complete, and capture dynamically generated content. For example, scraping data from a Single Page Application (SPA) where content is loaded dynamically through JavaScript.

4. **Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.**

Purpose: XPath (XML Path Language) is used to navigate XML and HTML documents and is often employed in web scraping to locate and extract specific elements from the HTML structure.

Example Xpath Expression: 

Suppose you want to select the text inside a paragraph (<p>) with a specific class, e.g., <p class="example">Hello, World!</p>. The XPath expression would be: `//p[@class="example"]`

## `Things I want to know more about`
