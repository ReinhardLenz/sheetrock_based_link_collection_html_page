# sheetrock_based_link_collection_html_page
Page to collect publicly links, links are administrated via gmail googlesheets account links get old, new links should be quickly added, and a theme directory for keeping links in order. The connection between html page and gmail account is thought sheetrock routine. The link directory is shown as a collapsible table with three columns. By clicking on a theme, the respective theme opens up and shows the links of the theme. A new theme can be added simply by adding a new table in the gmail googlesheet table, the tab on the lower edge of the google isheet is given a name like "poetry", and a new "gid number" is created on the googlesheet. (the last 9 digits in the browser input bar.)

https://docs.google.com/spreadsheets/d/1yN7Tv3HfqysV1RmTilGLAr_XbLOX0RvxXWg9Qp0xDiY/edit#gid=123456789

gid=123456789
gid number  is taken down

 added to the php file a new row like this
...
array( "poetry",  123456789),
...

Link to the sheetrock repository:

https://chriszarate.github.io/sheetrock/
