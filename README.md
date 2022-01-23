# UFOs

## Overview

Using JavaScript, HTML, and CSS build webpages to display a table organizing UFO sightings data.

### Purpose

Using the tools mentioned above, a dynamic webpage will be built in which the data concerning UFO sightings can be stored, displayed visually, and be interative (able to filter based on search criteria). Having a dynamic website allows the data to be visually appealing and easy to access for everyone. Sifting through data manually in a table or array can be tedious but having a interactive website allows data access and understanding to be attainable to everyone.

## Results

UFO Sightings:

![static/images/we.png](static/images/we.png)

Filters and the table:

![static/images/b.png](static/images/b.png)

Using the filter search, you can filter by any combinations of the search criteria. For example: you can search only by date or by every category. The search criteria corresponds with the columns of the table. All but the last two columns, 'Duration' and 'Comments,' are available to filter. 

![static/images/f.png](static/images/f.png)

Example of a filtered search:

![static/images/filter_search.png](static/images/filter_search.png)

## Analysis

There are a few drawbacks to the designed webpage.
- Case-sensitive search field: The table will not filter properly if the cases are not matched in the search box and in the table itself. There is also no instruction on how to enter the information into the search field. If the user mistakenly uses upper case when it should be lower case, they may not know why they aren't getting data returned or believe there to be no data at all for that search.
- No partial entries: the search criteria must be filled out in it's entirety or there will be no return of data in the table. This potentially causes the same issue stated above.
- There is no live data source connected to this data. The table will not update as more sightings are reported. 
- The filters require a previous understanding of the data in the table. The user must know the specific date, city, or shape to search. Some shapes might not be intuitive.
- Whitespaces: this ties with the first two drawbacks listed. The data MUST be entered exactly how the table has the data stored. If there is an extra space that was not intended by user error, there will be no output

Recommendations:
1. Add a trim function to clear out white spaces
2. Create a function to standardize the entries as all upper case or lower case so despite how the user enters the data, it will be transformed to match the data in the table
3. Create a date range filter. Being able to see all the data from one month could be beneficial in tracking activity between different months
4. Add a live data source so the table can continuously update as new sightings are reported

