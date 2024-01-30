# Filters & buttons

## Filters

!!! tip "Good practice"
    - Try to apply filters to all the views in one dashboard unless there is a strong reason to have seperate filters for each view. Users should not have to search around the page to cancel previous choices.

    - Make sure the values in the quick filter are ordered in a way that makes sense for your data. You can specify the order of a quick filter by setting the default sort order for that field.

    - If your user can make multiple selections within a filter dropdown the use an 'apply' button. This stops visualisations refreshing whilst the user is still choosing their selections.

    - Slider filters are great for date and numerical values, while list filters are better for categorical data. If your filter is continuous it may show date and times when published to prod, you can avoid this by making your date filter discrete iwth Day(Date), Month(Date) etc.

    - Discrete date filters can be set to the latest date value in the data source.

    - If your users require start and end date on the slider filter, this will not automatically update when new data comes through. To avoid this, instead of filtering on a range of dates, choose 'all dates' on the 'special' tab and turn the filter into a slider, as per the image below.
    
    <figure markdown>
    ![Adding a button steps](../../images/all_dates_filter.png){data-gallery="filter"}
    </figure>


### Filters summary

### Filters size

### Filter layout (two rows)

### Advance filters


## How to add a button on the dashboard

Tableau has an inbuilt button object used to navigate from one page to another within a dashboard.

1. You can use the 'navigation' object on the bottom left hand side.

2. Drag it to the dashboard like any other object.

3. Click the 'edit button' to define its attributes.

4. You can add this button as an image or as a text box.

5. test it in the presentation mode to make sure it is working correctly.

!!! warning "Note if you edit the background colour of the button it will appear unchanged unless in presentation mode or on server."

## To use buttons as filters

This functionality is not part of the default tableau button above. To implement a custom button you must instead create a worksheet that looks like a button.
For example you might want a button for each region to filter your visualisations.

1. Create a new worksheet using the square mark eg named 'region button'.

2. Format the square colour to what you want the button to be and increase size to the maximum. Fit to entire view.

3. You must add the field you want to filter other worksheets by as a mark eg detail mark. You can create several buttons on one worksheet by also adding the field to columns (image 1). Alternatively if you are only having one button per worksheet you can add the field to the filters area and preselect the value you want the button to filter other worksheets to (image 2).

4. To add text to your button use a label. This can be using the field or static text.

5. Add your button worksheet to your dashboard.

6. Create a filter dashboard action.


### Button to reset all filters in a dashboard

The method to use buttons as filters can also be used as a 'reset button'.

1. 


## Toggles (weighted data)