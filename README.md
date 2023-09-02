# sheetrock_based_link_collection_html_page
Page to collect publicly links, links are administrated via gmail googlesheets account. This is more flexible as links get dusty, new links should be quickly added, and a theme directory for keeping links in order. The connection between html page and gmail account is thought sheetrock routine. The link directory is shown as a collapsible table with three columns. By clicking on a theme, the respective theme opens up and shows the links of the theme. A new theme can be added simply by adding a new table in the gmail googlesheet table, the tab on the lower edge of the google isheet is given a name like "poetry", and a new "gid number" is created on the googlesheet. (the last 9 digits in the browser input bar.)
In the googlesheets, the address bar looks like this:
https://docs.google.com/spreadsheets/d/1yN7Tv3HfqysV1RmTilGLAr_XbLOX0RvxXWg9Qp0xDiY/edit#gid=123456789

gid=123456789
gid number  is taken down

Inside the googlesheet the table is structured with first colum as the link text, and the second column as the link <a> tag content itself.
![Capture](https://github.com/ReinhardLenz/sheetrock_based_link_collection_html_page/assets/71219487/2dd97339-898b-443a-9bf0-5ffffcd9a1c5)

 added to the php file a new row like this
...
array( "poetry",  123456789),
...

Link to the sheetrock repository:

https://chriszarate.github.io/sheetrock/

https://github.com/chriszarate/sheetrock

My motivation is that Browser bookmarks are not easy to keep structured, moreover, I use several browsers. I have no idea, how to extract and transfer bookmarks from one place to another. But still, I think bookmarks are quite important. The google search with the same words of today may lead to completely different result then the google search of tomorrow with exact the same words. 
