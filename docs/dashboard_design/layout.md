## General layout
> Layout done perfectly, will be invisible to the user. Layout done badly may be the only thing they see.

The following page template is used across the product, particularly for report pages. it is best practice to use a Z-formation, like how you would read a book.
For more details see the [principles page](principles.md#visual-hierarchy).

![Z layout examples](images/z_layout.png){data-title="Z layout examples"  data-caption-position="top" data-gallery="z"}

!!! danger "General rules"


    - 32px margin on all sides of the dashboard as per <a href="https://www.england.nhs.uk/nhsidentity/identity-guidelines/nhs-logo/">NHS England identity guidelines.</a>

    - 16px padding on top, bottom, left and right of cards. For further information visit the [cards page](cards.md).

    - 32px spacing between cards on the dashboard.

    - Minimum font size 11px or 11pt.

    - Utilise various weights to establish a hierarchy. Be consistent in size, boldness and colour.

    - All text should be sentence case.

    - Dashboard background colour #F0F4F5 (NHS Grey 5).

    - If the viz is going to show more data (more lines/bars) use the full width card so it helps the user to digest information quickly.


???- tip "Example dashboard layout annotated with padding and spacing"
    ![Finished layout](images/full_page_layout.png){data-title="Full page layout" data-caption-position="top" data-gallery="full"}

### Header
- The top of the page should be split into two main sections.
- In Tableau, these two sections would each be in a separate container sat within an overall top of page horizontal container.
- On the left should be the dashboard title, subtitle if used, a brief dashboard description and an alert/message banner if needed.
This section should be no more than 1200px.
- On the right should be the NHS logo and any data refresh information. This section should be a fixed width of 300px.


![Page layout dimension](images/page_layout_dimensions.png){ data-title="Page header example" data-description=".custom-desc-page" data-caption-position="left" data-gallery="page"}

<div class="glightbox-desc custom-desc-page">Header example</div>

!!! tip "Useful tips for header section"

    1. Use either tabs or buttons for navigation purposes. Not both. This repetition makes the header look busy.

    2. Do not use the 'Hide note' functionality in the header section.

    3. Avoid using icons/images in the header area to redirect users to different dashboards.

        - Clicking on icons without labels is not intuitive.

        - Multiple icons increases visual clutter.

        - Instead move the icons next to relevant / related visualisations outside of the header section.
    
    4. Add links to related dashboards and supporting webpages to an 'information & guidance' page or a 'related dashboards' page.

    ![Header section tips](images/header_tips.png){ data-title="Page header example" data-gallery="header"}

      See the [Download templates page](download_templates.md) for details on how to download and use the templates.


### Titles and subtitles

For easy identification and navigation, every tab should show the workbook title (NHS Grey1, 24pt, Arial, sentence case), and the subtitle which matches the tab name (Black, 24pt, Arial, sentence case), with a black hyphen with spaces either side between the two names. A brief description of what the tab is showing can be added.

### Data refresh date

The data refresh date should be shown to the left of the NHS logo in dashboards using the web wrapper. For dashboards not using the web wrapper the data refresh should be to the right of the page underneath the navigation bar(s).

### Margins

Left, top and right margins should be 32 pixels. The bottom of each page should show an NHS Blue line (height = 2 pixels) and contact information.
Additional information on latest data available is an optional extra.

### NHS identity 

See the [icons & logos page](icons.md) for details on the NHS logo

### Text and image alignment

All text and images should be left aligned to improve accessibility.



## Dashboard sizing & device layouts

- Tableau provides different types of **sizing** for dashboards which are fixed, range and automatic. 
- Tableau provides different **device layouts**, which display a different layout of the dashboard depending on what device is viewing the dashboard such as desktop, tablet or phone.


### Fixed, range & automatic sizing

???+ tip "Fixed sizing (Default recommended option)"
    ![Fixed layout](images/fixed_layout.png){: height="100px" data-title="Fixed layout" data-caption-position="top" data-gallery="layout" align=right}

    - [x] The dashboard remains the same size, regardless of the size of the window used to display it.
    If the dashboard is larger than the window, it becomes scrollable.

    - [x] Lets you specify the exact location and position of objects, which can be useful if there are floating objects which are often used for "show/hide" implementations where dynamic zones are not suitable.

    - [x] These will load faster because a fixed width dashboard can be cached on Tableau server.

    - [x] Less development work and testing is required as you do not have to test multiple screen sizes and monitors to ensure the dashboard appears and functions as expected.

    - [x] When using the recommended 1200px width, there will be no horizontal scroll bar for the vast majority of common screen sizes.

???- tip "Range sizing (Valid use case under the right conditions)"

    ![Range layout](images/range_layout.png){: height="100px" data-title="Range layout" data-caption-position="top" data-gallery="layout" align=right}

    - [x] The dashboard scales between minimum and maximum sizes that you specify.

    - [x] If the window displaying the dashboard is smaller than the minimum size, scroll bars are displayed.
    If it is larger than the maximum size, white space is displayed.

    - [x] Use this setting when you are designing for two different display sizes that need the same content and have similar shapes - such as small and medium sized browser windows. 1200 to 1920px range width is recommended in these use cases. For larger monitors certain charts will be wider and be easier to read and interpret.

    - [ ] Developers must ensure that the dashboard displays correctly at all screen sizes, this requires more development work and testing.

    - [ ] These will load slower as they are unable to use a cached version on the server.

    - [ ] Floating containers cannot be used effectively, restricting certain features for users.

???- tip "Automatic sizing (not recommended)"

    ![Automatic layout](images/auto_layout.png){: height="100px" data-title="Automatic layout" data-caption-position="top" data-gallery="layout"  align=right}

    - [x] The dashboard automatically resizes to fill the window used to display it.

    - [x] Use this setting if you want Tableau to take care of resizing. For best results, use a tiled dashboard layout.

    - [ ] This setting is not recommended



### NHS England recommendation on which sizing to use


???+ success "Default recommended option: 1200px fixed width dashboard"
    - [x] Suitable for a wide range of screen sizes used by a diverse user base
    - [x] Enables better feature development using a full range of Tableau functionality (e.g floating containers for show/hide)
    - [x] Speed improvements in dashboard performance
    - [x] Less development and testing required

???- warning "Valid use case under the right conditions: 1920px fixed width dashboard"
    - [x] Where the user base is entirely analytical
    - [x] Where all screen sizes are known or dashboard is designed for a permanent screen (e.g a control room)
    - Note that users accessing dashboards with smaller monitors will have a horizontal scroll bar and may omit elements of the dashboard. It is recommended to add an information note on the dashboard to explain that it is best viewed on a wide screen monitor (i.e 1920px width at 100% display scaling).


???- warning "Valid use case under the right conditions: 1200px to 1920px width range dashboard"
    - [x] Where the user base is entirely analytical
    - [x] Where a wide range of screen sizes is used by different users
    - This will allow certain visuals such as line charts and bar charts to expand to monitors that are wider. This benefit must be weighed against the performance trade off of slower load times, more development/testing and reduced Tableau functionality in responsive range dashboards 





### Device layouts

Dashboards can be designed to show different views based on the device that is viewing the dashboard. For dashboards that are viewed directly on server, Tableau applies the following rules to display each device layout. 


| If the smallest iframe dimension is... | This device layout appears... |
|----------------------------------------|-------------------------------|
| 500 pixels or less                     | Phone                         |
| Between 501 and 800 pixels             | Tablet                        |
| Greater than 800 pixels                | Desktop                       |

![Selecting Tableau device layout](images/tableau_device_layout.png){: width="20%" data-gallery="tableau_layout" align=right}

These different views are created in Tableau using the device preview button.

 - The default view is the full sized view that is designed by default. 
 - Adding in tablet and phone views will allow your dashboard to be viewed correctly by those devices. 
 - The templates have default (desktop), tablet and phone views included already. 
 - Anything created or amended in the default view should be checked in the tablet and phone views afterwards before publishing
 - This is recommended to be done at the end of the development process to avoid rework across all three views.




??? tip "Desktop (range above 800 pixels)"

    - If the user is looking at the dashboard in a browser that is less than 1200 pixels width then a horizontal scroll bar should appear.

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
    It is advisable to complete you dashboard before setting this functionality up, otherwise each time you make changes to the dashboard, they need to be done in both views.

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

    - The example below, shows how complex tabular data can be simplified for mobile devices. Rather than showing multiple days in the table, we could give an option for the user to select a day in additional filters.

    ![A desktop table](images/desktop_table.png){: width="43%" data-title="An example desktop complex table" data-caption-position="top" data-gallery="visualisation" align=left}
    <span style="font-size:900%;">&#8594;</span>
    ![A mobile table](images/mobile_table.png){: width="35%" data-title="Simplified mobile table" data-caption-position="top" data-gallery="visualisation" align=right}

    <br style="clear:both; mso-break-type:section-break" />

    - Further simplifications could be to limit charts to the top three by default with the option to show all.

    ![A desktop chart](images/desktop_chart.png){: width="43%" data-title="An example desktop long chart" data-caption-position="top" data-gallery="visualisation" align=left}
    <span style="font-size:900%;">&#8594;</span>
    ![A mobile chart](images/mobile_chart.png){: width="35%" data-title="Simplified mobile top 3 chart and expanded view" data-caption-position="top" data-gallery="visualisation" align=right}



???+ warning "Avoid scroll bars"

    In general you should try to avoid scroll bars in your products. However, where the use of a scroll bar is necessary, ensure that there is only one scroll bar on your dashboard either vertical or horizontal.

    Not two vertical scroll bars (one applied for the browser and the second one applied to a component within the dashboard).

    ![Example scroll bars](images/scroll_bars.png){: width="35%" data-gallery="scroll"}




