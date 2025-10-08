📚 Sheetrock-Based Link Collection HTML Page
A lightweight and flexible HTML+PHP-based system to maintain and display categorized web link collections using a Google Sheets backend and the Sheetrock.js library.

🔧 Features
Links are managed via Google Sheets using a Gmail account.

Frontend uses Sheetrock.js to fetch and display data from Google Sheets.

Links are organized by theme, shown as a collapsible table with three columns.

Easily update, add, or remove links without touching the code—just update your spreadsheet.

No database required. Everything is live from Google Sheets.

📁 Structure
Each theme (or category) is a separate tab (worksheet) in a single Google Sheets document. Each worksheet contains:

Column A (1st)	Column B (2nd)
Link Text	URL

You can also add more data (e.g., notes or tags) in extra columns if needed for styling or metadata.

🧠 How It Works
Create a Google Sheet with multiple tabs—one for each link category (e.g., poetry, electronics, recipes, etc.).

Share the sheet with "View access to everyone" (read-only).

Use the gid number of each tab (found in the URL after #gid=) to connect it with your PHP/HTML frontend.

Example URL:

bash
Copier
Modifier
https://docs.google.com/spreadsheets/d/6yN7Tv2HfqysV9RmTilGLAr_XaKOX2RvxXWg9Qp5xDiY/edit#gid=123456789
The number 123456789 is the gid for the respective tab.

In your PHP config, define the themes as an array:

php
Copier
Modifier
$themes = array(
    array("poetry", 123456789),
    array("electronics", 987654321),
    ...
);
When the page is loaded, each theme is shown as a collapsible row. Clicking it reveals the list of links under that theme.

🔗 Dependencies
Sheetrock.js by Chris Zarate
Sheetrock is used to fetch public Google Sheets data via JavaScript.

🔐 Permissions
You must make the Google Sheet publicly viewable for Sheetrock to access it.

Only the account owner (you) can edit it.

No authentication or login is required on the frontend.

💡 Motivation
Browser bookmarks are clunky and hard to sync across browsers or devices. Plus, bookmarks don't scale well or allow flexible categorization. With this system:

You can manage all your bookmarks in a single Google Sheet.

They’re accessible from any browser and device.

You can quickly update outdated links or add new ones on the fly.

Google search results are inconsistent over time; this system helps preserve good resources before they vanish.

📸 Screenshot
<img width="1385" height="149" alt="image" src="https://github.com/user-attachments/assets/9e702683-f019-4800-8df1-9d677737c2cf" />


🚀 Getting Started
Clone or download this repository.

Set up your Google Sheet with appropriate tabs and links.

Configure your PHP file with the correct gids.

Upload everything to your web server (e.g., Apache or Kapsi.fi).

Done! Open the page and start organizing.


![Visitor Count](https://komarev.com/ghpvc/?username=ReinhardLenz&repo=sheetrock_based_link_collection_html_page&color=green)
