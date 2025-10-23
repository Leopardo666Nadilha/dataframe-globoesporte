# Globo Esporte - Homepage Scraper

This project is a Python script built to practice web scraping and data extraction. It scans the main homepage of the Brazilian sports site "Globo Esporte" (`globo.com/ge`).

The script automatically finds all news posts on the page, extracts their key information, and organizes this data into a clean, structured table (a Pandas DataFrame).

### 💻 Tech Stack
* **Python**
* **Pandas:** Used to create and display the final DataFrame.
* **BeautifulSoup4:** Used to parse the website's HTML.
* **Requests:** Used to fetch the HTML content from the website.

### ✨ How it Works
1.  The script sends an HTTP request to the Globo Esporte homepage.
2.  It parses the HTML response to find all `div` elements with the class `feed-post-body`.
3.  For each post, it extracts the following data:
    * `manchete` (Headline)
    * `descricao` (Description)
    * `link` (URL)
    * `secao` (News Section, e.g., "Futebol")
    * `time_delta` (Time since posted, e.g., "há 2 horas")
    * `hora_extração` (The exact timestamp of when the script ran)
4.  Finally, it compiles all this data into a Pandas DataFrame for easy viewing, analysis, or export.
