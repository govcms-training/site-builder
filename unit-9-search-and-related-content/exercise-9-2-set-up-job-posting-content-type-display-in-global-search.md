# Exercise 9.2: Set up Job posting content type display in global search

Try to conduct a search for a published Job posting content type. You’ll notice that it appears differently to other content types:

<table>
  <thead>
    <tr>
      <th style="text-align:left">
        <p>
          <img src="../.gitbook/assets/146 (1).png" alt/>
        </p>
        <p>Standard page search results</p>
      </th>
      <th style="text-align:left">
        <p>
          <img src="../.gitbook/assets/147.png" alt/>
        </p>
        <p>Not configured Job posting search result</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

This is because the search index isn’t configured to display the right View mode for the Job posting content type and it shows the same content as the full-page view.

Let’s change that, by activating Search view mode in the Job Posting content type and then configuring the search to use it.

1. Go to Structure → Content types → Job Posting → Manage display.
2. Under the _Custom display settings_, enable the **Search** view mode. Save the changes.
3. Click the Search link at the top \(in the secondary tabs\) to navigate to the Search view mode.
4. Under the **Select a layout** field, select **Search** and save the changes. You’ll notice that the fields table below now shows multiple regions, such as:
   1. Title
   2. Info
   3. Summary
   4. Tags
   5. Disabled
5. Rearrange fields \(drag-and-drop\) to match the screenshot. Move the remaining fields into the disabled region. Focus on making the Title field a link and trimming the Job description down to 300 characters. 

    ![Image of rearranged fields](../.gitbook/assets/148%20%281%29.png)
    
    Now, as we created and customised the Job posting view mode for Search, let’s make the search page to use it. Our search page is made as a View, although it’s set to use the Search API functionality. We’ll explore how to create a Search API view later. 
    
7. Go to **Structure** → **Views** and edit the _Search_ view. 

    ![Image of edit Search view](../.gitbook/assets/149%20%281%29.png)
    
8. Under **Format** → **Show**, click on the **Settings** link: 

    ![Image of Settings link](../.gitbook/assets/150%20%281%29.png)
    
9. Locate the “**View mode for datasource** _**Content**_**, bundle** _**Job Posting”**_ and change it to use the **Search** view mode created earlier 

    ![Image of use Search viee mode](../.gitbook/assets/151%20%281%29.png)
    
9. Apply your changes and save the view.
10. Repeat search for a job posting and confirm if the display looks similar to other content types.

    <table>
  <thead>
    <tr>
      <th style="text-align:left">
        <p>
          <img src="../.gitbook/assets/152.png" alt/>
        </p>
        <p>Search result for Job posting</p>
      </th>
      <th style="text-align:left">
        <p>
          <img src="../.gitbook/assets/153 (1).png" alt/>
        </p>
        <p>Search result for Standard page</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

11. You may return to the Search view mode in the Job posting content type and change it further, to test how your changes affect the search results display widget.
