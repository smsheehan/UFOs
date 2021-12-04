# UFOs

## Overview of Project: Explain the purpose of this analysis.

The purpose of this analysis is to enable the end user to be able to filter a UFO sightings database across multiple search criteria (date, city, state, country, shape).  From a skills standpoint, we needed to take the website built in the module work and refactor the code to accomplish the following:
* html code: add additional search boxes
* html code: remove the search button
* javascript code: tell d3 to listen for change rather than a handleclick
* javascript code: create a new object to hold the filter criteria
* javascript code: write new code to filter the table and build a new table with only the rows matching the filter criteria

## Results: Describe to Dana how someone might use the new webpage by walking her through the process of using the search criteria. Use images of your webpage during the filtering process to support your explanation.

Upon first loading the page, the user is presented with the title of the page and a short article which provides insight into the purpose of the page and UFO database.
![image](https://user-images.githubusercontent.com/90977689/144717961-79ab5bed-7c7c-4366-ad0e-e355d0caa0c2.png)

Upon scrolling down the page, the user is presented with the UFO data table and 5 search fields on the left hand side of the page.
![image](https://user-images.githubusercontent.com/90977689/144718009-d2a7637d-33c6-4709-a9ba-288814f05657.png)

The search fields hold example text to inform the user of the format for entering search criteria.  To perform a search on singular category, the user just needs to fill in the search term and hit return or tab on their keyboard and the table is redisplayed with only rows containing the search criteria.  An example search on state is shown below:

![image](https://user-images.githubusercontent.com/90977689/144718385-3e466c0f-e8bc-493b-9db5-378c097d57c2.png)

If the user wants to search on multiple criteria, all they have to do is add another search term and hit the return or tab key on their keyboard.  An example two term search is shown below:

![image](https://user-images.githubusercontent.com/90977689/144718591-605a68f6-3729-4671-9bad-7986434f1945.png)

If the user wants to go back to the original table, all they have to do is delete the search terms from the search boxes and hit return or tab and they will see the full table displayed again.




## Summary: In a summary statement, describe one drawback of this new design and two recommendations for further development.

There are several drawbacks to the current design, but if I had to pick the most important to fix first it would be the fact that the search is case sensitive.  While the placeholder text does give the user the example of the correct format, many people are used to entering city names with the first letter capitalized and entering city initials with both letters capitalized.

My recommendations for further development would first be to enable the search terms to be insensitive to capitalization.  This would presumably by adding to the code a line that set all of the search terms to lowercase when putting them in the filters list object.  The next recommendation would be to enable the user to search for more than one item at a time in a given category.  For example, if a user wanted to search on multiple states or multiple shapes they should be able to do that.  Finally, stylistically, the color of the search text should be changed.  Currently it is hard to visually discern the typed in criteria (currently shown in black) vs the placeholder text (currently shown in gray).
