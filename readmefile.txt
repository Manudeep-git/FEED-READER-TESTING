<title> Feed reader testing documentation</title>
->step by step procedure
    ->RSS FEEDS TEST
        -> In the First test i have made sure that all the "urls" and "names" mentioned in "allFeeds" variable
        are not empty and created seperate test suites for "feed defintion" and their "names" and "urls" 
        respectively.
        ->I used ".length" property to check they are not empty
        ->
    ->MENU TEST
        ->In this i have tested whether html body contains "menu-hidden" initially and used body.className property 
          check it and wrote a test that expected it to be true 
        ->The second test expects to show the menu when clicked on the menu icon and it is done based on the 
          avaialbility of"menu-hidden" element i.e when clicked on the "menu-icon-link" the "menu-hidden" should not 
          be present in the body and if we click it again ,it should me made avaialable and i used body.className 
          property here also.
    ->INTIAL ENTRIES TEST
        ->For this asynchronous tests i used before each function to make sure that test is executed after loading 
          and by selecting element using jquery i made sure that there is atleast one entry before loading as required
        ->I also made sure that there is a link starting with http or https for each of entires by looping through the
          entries 
    ->NEW FEED SELECTION TEST
        -> Again i used before each function that ensures content changes from intial load and wrote a test case that expects 
          initial feed selection is not equal to new feed selection