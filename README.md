# Scraping Data: Game Title Info
The purpose of this project was to collect information about past videogame consoles. We attempted to scrape information like release date, publisher, developer, review scores, and description on over 11,000 titles.

Of those 11K titles, we were able to collect information about 79% of them using knowledge graphs. The following consoles were collected:
 - 3DS
 - Dreamcast
 - Gameboy
 - Gamecube
 - Gameboy Advance
 - Gameboy Color
 - Genesis
 - N64
 - Nintendo DS
 - Nintendo Entertainment System
 - SNES
 - PS1
 - PS2
 - PSP
 - Wii

## Our Process
In order to collect information on these games, we first had to collect console and title info. We were able to pull this information from a popular game preservation website and wikipedia. This process can be seen in the **Console Collection** notebook.

After collecting the console and titles, formatted as CSVs, we could then pull information from Google's knowledge graph using SerpApi. This process is found in the **Data Collection** notebook. After collecting said data, it was necessary to merge into one cohesive file, so we decided to utilize json to do so. After reading in both the console and data CSVs, it was possible to combine them and format them into an easy to navigate dictionary using the **Final Data** notebook. 

Finally, we checked our work using the **Error Checking and Statistics** notebook.

## The Data
Our data can be found in the project repo, named **final.json**. If you'd like to review our data, we suggest using [this online json editor.](https://jsoneditoronline.org/) Just paste the entire file contents while "code" is toggled in the top left, and then switch to "tree" mode. You'll then be able to easily explore the data.

## Acknowledgments
All work was done by myself [Janam](https://github.com/janampatel15) and [Ambrose](https://github.com/ajkarella). [SerpApi](https://serpapi.com/), and their generous 15 day trial, was a big help as well.
