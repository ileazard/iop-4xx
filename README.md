# iop-4xx
PRG-160-3485 JavaScript repo for the iop-4xx project
https://ileazard.github.io/iop-4xx/

inside out project version 400-0
-added base code to index.html and added initial JavaScript to app.js page

inside out project version 401-1
-created the appData object
-moved the title & tag line variables in to appData and
-refactord the initializeApplication function

inside out project version 401-2
-added bootstrap to the index.html
-added a DOM injection of the progressbar in the app.js
-created the displayPB function in the app.js

inside out project version 402-0
-added style.css and linked in index.html
-added login form function and call after progress bar
-added minimal validateLogin function to check for blank

inside out project version 403-0
-index.html
  -updated all hrefs/links to passive protocol
  -moved style sheet link below animate and bootstrap to allow for custom styles to override all
-style.css
  -added styles for application interface - sidebar, wrapper, navigation, etc.
-app.js
  -added the aplicationuserinterface function wich defines the application user interface
  -added the buildmenu function which returns the navigation menu and will increase in dynamic navigation building
  -added the buildmain function which returns the primary content area and will evolve to return content dynamically
  -replaced document wrte with call to applicationuserinterface function in the validatelogin function
  -added the linkclicked function which is called by click events on anchor elements and returns dynamically driven results

  inside out project version 404.0

  -index.html
    -code changes https://www.diffchecker.com/oybNnzTY
    -removed comments and cleaned code
    -added script tag for quotes.js file
  -style.css
    -code changes https://www.diffchecker.com/114fW8QY
    -modified the sidebar and sidebar ul classes
    -added the auth and infoDiv classes
  -app.js
    -code changes https://www.diffchecker.com/oKMHtB1u
    -added the quotArr sort to the initializeApplication function
    -modified buildMenu function to dynamically build the menu from the array
    -modified linkClicked function to dynamically populate main content with array content
  -added the assets/data/quotes.js file
    -code changes https://www.diffchecker.com/YlRCv0UM

    inside out project version 405-0

-index.html
  -added script tag to pull in ajax.js file
  -code changes https://www.diffchecker.com/YvNo8ojf
-style.css
  -modifed .contStage by adjusting the (left: 180px;) - changed value to 80px to close gap between side manu and the content
  -clead up comments
  -code changes https://www.diffchecker.com/DO5umcE7
-app.js
  -lead up comments
  -added sideMenu array to the appData object to be used to call ajax to load the pages & posts from the me site
  -modified the displayPB() function - changed preloader time from 50 to 15 to speed up load during development
  -modified the buildMenu() function to accept menu items from appData object - removed call to quotes array
  -modified the linkClicked() function
    -added conditional to evaluate if the object clicked is in the menu array of the appData.sidemenu object
      added ajax call to grab posts/pages
  -code changes https://www.diffchecker.com/KBziC4iw
-added the assets/data/ajax.js file
  -code changes https://www.diffchecker.com/jVWFzAwU
