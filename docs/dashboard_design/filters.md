# Filters & buttons

![Filters](../../images/filters.png){ data-title="Filters" data-description=".custom-desc1" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc1">
Filters example
</div>

## Filters

!!! tip "Good practice"
    - Try to apply filters to all the views in one dashboard unless there is a strong reason to have seperate filters for each view. Users should not have to search around the page to cancel previous choices.

    - Make sure the values in the quick filter are ordered in a way that makes sense for your data. You can specify the order of a quick filter by setting the default sort order for that field.

    - If your user can make multiple selections within a filter dropdown the use an 'apply' button. This stops visualisations refreshing whilst the user is still choosing their selections.

    - Slider filters are great for date and numerical values, while list filters are better for categorical data. If your filter is continuous it may show date and times when published to prod, you can avoid this by making your date filter discrete with Day(Date), Month(Date) etc.

    - Discrete date filters can be set to the latest date value in the data source.

    - If your users require start and end date on the slider filter, this will not automatically update when new data comes through. To avoid this, instead of filtering on a range of dates, choose 'all dates' on the 'special' tab and turn the filter into a slider, as per the image below.
    

![Filters](../../images/all_dates_filter.png){ data-title="Filters" data-description=".custom-desc2" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc2">
Selecting all dates in filter settings
</div>



### Filters summary

- The filters on a dashbord should span across the width of the navigation line left aligned to the dashboard.
- Maximum of two rows (10 filters) should display on a dashboard. If more filters are required, then they should be included in the 'advanced filters' container.
- Filters should always show a reset link, which resets all of the filters applied including the advanced filters.
- When adding filters to a dashboard do not change the font colour and size on the worksheet. The font colour will be set in the template.
- Advanced filters button is optional and should be added only if there are more than 10 filters.

### Filters size, padding and colours

- All filters should be in equal width
- The filter card should be a white container with 16px inner padding and a 2px shadow (refer to <a href="dashboard_design"> cards page</a> for further details)
- The filters should be in a horizontal container within the card with a background colour of #d8dbdc
- The inner padding of each filter should be 16px left (apart from the further left filter) and 16px right
- Each filter should have a white background
- The outer padding of each filter should be 1px left (apart from the furthest left filter) to give the break lines
- The filter title should be arial, bold and size 11
- There can be any number of filters on a dashboard but a maximum of five should display in a row.

![Filters size](../../images/filters.png){ data-title="Filters size" data-description=".custom-desc3" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc3">
Example of size of filters
</div>

**Filters - empty slot:**
- If there are <5 filters on a dashbouard, then the rest of the filter container slots should be left as empty and set a vairable width similar to the other filter containers

### Filter layout (two rows)
- Filters should always show a reset link, which resets all of the filters applied including the advanced filters.
- Only five filters should appear in a row for desktop, for 10 filters they have to split into two rows.
- When adding filters to a dashboard do not change the font colour and the size on the worksheet. The font colour will be set in the template.
- 'Advanced filters' button is optional and should only be added if there are more than 10 filters.

![Filters two rows](../../images/filters_2_rows.png){ data-title="Filters two rows" data-description=".custom-desc4" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc4">
Example of filters with two rows
</div>

### Filters with controls
Dashboards may require extra Controls along with the filters. The purpose of the controls is to change the way the measures are being calculated. Eg: Absolute values, 7 day rolling average, Population rates.

Note: Controls and filters will both work in conjunction to refine the data.

![Filters with controls](../../images/filters_controls.png){ data-title="Filters with controls" data-description=".custom-desc5" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc5">
Example of a filter with controls
</div>

### Filters with radio buttons & sliders
- Based on the data we populate on the dashboard, it may be required to use radio buttons and sliders as filters.

![Filters with radio buttons & sliders](../../images/filters_radio.png){ data-title="Filters" data-description=".custom-desc6" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc6">
Example of filters with radio buttons & sliders
</div>

### Filters in context
- If any filters are applicable only for a certain vizualisation then those filters should sit within its card layout, as shown below.


### Advanced filters  - No information required
This set of advanced filters does not require any information to explain all/any advanced filter.

![Advanced filters - No information required](../../images/advanced_filters_no_info.png){ data-title="Advanced filters - No information required" data-description=".custom-desc7" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc7">
Example of advanced filters with no information required
</div>

### Advanced filters  - Short information required
This set of advanced filters requires short information to explain all/any filter. The info should be shown in a tooltip should be shown in a tooltip when user clicks on the (i) icon.

![Advanced filters - Short information required](../../images/advanced_filters_short_info.png){ data-title="Advanced filters - Short information required" data-description=".custom-desc8" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc8">
Example of advanced filters with short information required
</div>

### Advanced filters  - Long information required
This set of advanced filters requires long information to explain all/any filter

![Advanced filters - Long information required](../../images/advanced_filters_full_info.png){ data-title="Advanced filters - Long information required" data-description=".custom-desc9" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc9">
Example of advanced filters with long information required
</div>


## How to add a button on the dashboard

Tableau has an inbuilt button object used to navigate from one page to another within a dashboard.

1. You can use the 'navigation' object on the bottom left hand side.

2. Drag it to the dashboard like any other object.

3. Click the 'edit button' to define its attributes.

4. You can add this button as an image or as a text box.

5. test it in the presentation mode to make sure it is working correctly.

![Button](../../images/dashboard_button.png){ width="300px" data-title="Button" data-description=".custom-desc10" data-caption-position="left" data-gallery="filters"}
<div class="glightbox-desc custom-desc10">
Dashboard button
</div>

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