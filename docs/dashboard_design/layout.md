# Setting up layout & navigation


Where NHS England dashboards are embedded into web pages it is best to make use of the existing web wrapper, this makes use of the 'showing sheets as tabs' Tableau navigation function.
Where this web wrapper is not available, it is best to use Tableau navigation buttons instead.


## Web wrapper

Our web wrapper
![Web wrapper](images/web_wrapper.png){data-title="Web wrapper" data-caption-position="top" data-gallery="wrapper"}

Our Tableau developers should build their dashboard pages from beneath the web wrapper navigation tabs. In the image below, the top part in grey overlay is the web wrapper, the rest is built in Tableau.
![Web wrapper meets Tableau](images/wrapper_meets_tableau.png){data-title="The web wrapper meets Tableau" data-caption-position="top" data-gallery="wrapper"}


## Navigation


**Tabs as navigation**

Including default tabs is the quickest, easiest way to allow users to navigate the dashboard. They are used in many products so users will be accustomed to using them naturally and they maximise space simply. We would advise this method. It is ideal not to have more than eight tabs.


**KPIs / Visualisation as navigation**

Users should be able to navigate through dashboards by clicking on the KPIs or on any areas within the visualisations.


**Hyperlinks**

Add hyperlinks to websites with more information (such as the HES Data Dictionary or published data on the NHS England website) or on the cover/about page.


**Buttons as navigation**

Buttons could be used as a navigation, but we recommend using tabs wherever possible.

> ![Adding a button steps](images/button_steps.png){: width="25%" data-gallery="button" align=right}

> **How to add a button on the dashboard**

> You can use the 'button' object on the bottom left hand side

>  1. Click and drag it to the dashboard canvas.
>  2. Click the 'edit button' to define its attributes.
>     Such as which page will be navigated to on clicking this button.
>  3. You can add this button as an image or as a text.
>  4. Test it in the presentation mode to make sure it is working correctly.

!!! note "Useful links"

    - For more info on Buttons
[comment]: <> (need actual links to add in!!)



## Page layout

Layout done perfectly, will be invisible to the user. Layout done badly may be the only thing they see.

**Titles and subtitles**

For easy identification and navigation, every tab should show the workbook title (NHS Grey1, 24pt, Arial, title case), and the subtitle which matches the tab name (Black, 24pt, Arial, sentence case), with a black hypen with spaces either side between the two names. A brief description of what the tab is showing can be added.

**Data refresh date**

The data refresh date should be shown on the right side of the title and subtitle

**Margins**

Left, top and right margins should be 32 pixels. The bottom of each page should show an NHS Blue line (height = 2 pixels) and contact information.
Additional information on latest data available is an optional extra.

**NHS identity**

NHS logo should be 75 x 40 pixels, witha top and right hand side margin of 32 pixels.


<figure markdown>
  ![Page layout](images/page_layout.png){data-title="Page header layout" data-caption-position="top" data-gallery="page"}
</figure>


!!! note "Useful links"

    - Tableau template download link
[comment]: <> (need actual links to add in!!)



## Dashboard layout

The following page template is used across the product, particularly for report pages. it is best practice to use a Z-formation, like how you would read a book.

<figure markdown>
  ![Z layout examples](images/z_layout.png){data-title="Z layout examples" data-caption-position="top" data-gallery="z"}
</figure>

!!! danger "General rules"

    ![Finished layout](images/full_page_layout.png){: width="50%" data-title="Full page layout" data-caption-position="top" data-gallery="full" align=right}

    - 32px margin on left and right sides of the dashboard.

    - 16px padding on top, bottom, left and right of the card.

    - 32px spacing between cards on the dashboard.

    - Minimum font size 11px or 11pt.

    - Utilise various weights to establish a hierarchy. Be consistent in size, boldness and colour.

    - Workbook name should be in title case.

    - Filters should be in sentence case.

    - Place filters horizontally under the dashboard title if you only have a few.

    - Dashboard background colour #F0F4F5 (NHS Grey 5).

    - If we are using multiple cards in a single row (side by side) make sure they are of the same height.

    - If the viz is going to show more data (more lines/bars) use the full wifth card so it helps the user to digest information quickly.



## Adaptive webview or fixed view

**Fitting**

The sheet size that fits in a Tableau workbook during development is different from what it will look like once published, and may be different from how it will fit on screens with different resolutions.

| If the smallest iframe dimension is... | This device layout appears... |
|----------------------------------------|-------------------------------|
| 500 pixels or less                     | Phone                         |
| Between 501 and 800 pixels             | Tablet                        |
| Greater than 800 pixels                | Desktop                       |


**Scroll bars**

In general you should try to avoid scroll bars in your products. However, where the use of a scroll bar is necessary, ensure that there is only one scroll bar on your dashboard either vertical or horizontal.

Not two vertical scroll bars (one applied for the browser and the second one applied to a component within the dashboard).

<figure markdown>
  ![Example scroll bars](images/scroll_bars.png){: width="63%" data-gallery="scroll"}
</figure>


### Control overall dashboard size

**Fixed**

![Fixed layout](images/fixed_layout.png){: height="100px" data-title="Fixed layout" data-caption-position="top" data-gallery="layout" align=right}

- The dashboard remains the same size, regardless of the size of the window used to display it.
If the dashboard is larger than the window, it becomes scrollable.

- These dashboards let you specify the exact location and position of objects, which can be useful if there are floating objects.

- These will load faster because they're more likely to use cached version on the server.



**Range**

![Range layout](images/range_layout.png){: height="100px" data-title="Range layout" data-caption-position="top" data-gallery="layout" align=right}

- The dashboard scales between minimum and maximum sizes that you specify.

- If the window used to display the dashboard is smaller than the minimum size, scroll bars are displayed.
If it is larger than the maximum size, white space is displayed.

- Use this setting when you are designing for two different display sizes that need the same content and have similar shapes - such as small and medium sized browser windows.


**Automatic**

![Automatic layout](images/auto_layout.png){: height="100px" data-title="Automatic layout" data-caption-position="top" data-gallery="layout"  align=right}

- The dashboard automatically resizes to fill the window used to display it.

- Use this setting if you want Tableau to take care of resizing. For best results, use a tiled dashboard layout.


<br>


### Different device views on Tableau

Tableau gives you the option to create different views based on a user's device.

<figure markdown>
  ![Selecting Tableau device layout](images/tableau_device_layout.png){: width="70%" data-gallery="tableau_layout"}
</figure>


??? tip "Desktop (range above 800 pixels)"

    - If the user is looking at the dashboard in a browser that is less than 12000 pixels width then a horizontal scroll bar should appear.

    - If the user is viewing the dashboard in a browser that is wider than 1920 pixels, then the dashboard has to be centre aligned to the screen by leaving space on either side.

    - Based on the screen size, the width of the elements (filter dropdowns, KPIs) should change but not the space between them.

    - Five filters per row.

    - Six KPIs per row.

    ![Laptop range layout](images/laptop_resolution.png){: width="45%" data-title="Laptop range layout" data-caption-position="top" data-gallery="range" align=left}
    ![Desktop range layout](images/desktop_resolution.png){: width="45%" data-title="Desktop range layout" data-caption-position="top" data-gallery="range" align=right}


??? tip "Tablet (range between 501 - 800 pixels)"

    ![Tablet range layout](images/tablet_resolution.png){: width="45%" data-title="Tablet range layout" data-caption-position="top" data-gallery="range" align=right}

    - If the user is viewing the dashboard in a screen range between 501 - 800 pixels, then the tablet layout should be populated.

    - Three filters per row.

    - Four KPIs per row.

    - Please note, as users will not be able to do the hover on touch devices (mobile & tablet), avoid tooltips and hover actions.
    It is advisable to complete you dashboard before setting this functionality up, otherwise each time you make chnages to the dashboard, they need to be done in both views.

    - Based on the screen size, the width of the elements (filter dropdowns, KPIs) should change but not the space between them.


??? tip "Mobile (range under 501 pixels)"

    ![Mobile range layout](images/mobile_resolution.png){: width="35%" data-title="Mobile range layout" data-caption-position="top" data-gallery="range" align=right}

    - If the user is viewing the dashboard in a screen range of 500 pixels or fewer, then the mobile layout should be populated.

    - Three filters per row.

    - Four KPIs per row.

    - Although we have identified a few patterns/examples on how we can simplify and present the data on mobile devices, we should still look at each dashboard individually to suggest any recommendations or simplify further.

    - Because of the limited space on mobiles, wherever possible please present only key important information.
    If the user requires a deeper analysis we will ask them to visit the desktop version.

    - Do not put graphs side by side.

    - Please note, as users will not be able to use the hover on touch devices (mobile & tablet) avoid tooltips and hover actions.
    It is advisable to complete your dashboard before setting up this functionality, otherwise each time you make changes to the dashboard, they need to be done in both views.

    <br style="clear:both; mso-break-type:section-break" />

    - An example, shown below, for simplifying multiple visualisations with complex data for mobile layouts, is to show only the highest values in a tabular format rather than showing the visualisation.

    ![A desktop visualisation](images/desktop_visualisation.png){: width="63%" data-title="An example desktop complex visualisation" data-caption-position="top" data-gallery="visualisation" align=left}
    <span style="font-size:900%;">&#8600;</span>
    ![A mobile visualisation](images/mobile_optimising.png){: width="20%" data-title="Simplified mobile visualisation" data-caption-position="top" data-gallery="visualisation" align=right}

    <br style="clear:both; mso-break-type:section-break" />

    - The example below, shows how complex tabular data can be simplified for mobile devices. Rather than showing mulitple days in the table, we could give an option for the user to select a day in additional filters.

    ![A desktop table](images/desktop_table.png){: width="43%" data-title="An example desktop complex table" data-caption-position="top" data-gallery="visualisation" align=left}
    <span style="font-size:900%;">&#8594;</span>
    ![A mobile table](images/mobile_table.png){: width="35%" data-title="Simplified mobile table" data-caption-position="top" data-gallery="visualisation" align=right}

    <br style="clear:both; mso-break-type:section-break" />

    - Further simplifications could be to limit charts to the top three by default with the option to show all.

    ![A desktop chart](images/desktop_chart.png){: width="43%" data-title="An example desktop long chart" data-caption-position="top" data-gallery="visualisation" align=left}
    <span style="font-size:900%;">&#8594;</span>
    ![A mobile chart](images/mobile_chart.png){: width="35%" data-title="Simplified mobile top 3 chart and expanded view" data-caption-position="top" data-gallery="visualisation" align=right}
