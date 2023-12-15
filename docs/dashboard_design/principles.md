# Key Principles


## Visual Hierarchy

Visual Hierarchy is the organisation of design elements by importance. It directs a user's attention to enhance their engagement of the information presented.
???+ tip "Visual Hierarchy"
    The first place your eyes go to is the **top of the screen**. 
    Place important information here for users to easily scan.

There are two primary [reading layouts](https://99designs.com/blog/tips/visual-hierarchy-landing-page-designs)
: Z pattern and F pattern.

A [Z-pattern layout](https://thenextweb.com/news/designing-websites-that-mirror-how-our-eyes-work-part-2) draws attention to the top-left corner first before moving to the top right, then down to the bottom left, with the bottom-right corner as the last stop. Each corner has a visual cue (like a logo) or CTA (like a contact button).

An [F-pattern layout](https://digital-freelancer.org/blog/f-shaped-pattern-explained), which follows a more crowded pattern leading visitors from left to right and back again, works well for text-heavy pages.

![Diagram of Z and F reading patterns](images/reading-layouts.png "Diagram of Z and F reading patterns"){data-title="Diagram of Z and F reading patterns" data-caption-position="top"}


## White Space

White space separates and groups elements in a dashboard.

It helps the eye to scan a page for information. Without it, your dashboard will be hard to read.

Adding white space reinforces the visual hierarchy of your dashboard. It puts the spotlight on the data in your dashboard.

Click [here](https://www.creatopy.com/blog/white-space-in-graphic-design/) for more examples of using white space in practice.



## Data-ink ratio

> Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away.

> **Antoine de Saint-Exupery**


**Definition**

The data-ink ratio is a concept introduced by Edward Tufte.
He refers to data-ink as the non-erasable ink used for the presentation of data.
If data-ink would be removed from the image, the graphic would lose the content.
The non-erasable portion of a graph is subjective, so Tufte follows up his principal of data-ink with the five laws of data-ink.

!!! danger "Five laws of data-ink"

        1. Above all else show the data
        2. Maximise the data-ink ratio
        3. Erase non-data ink
        4. Erase redundant data-ink
        5. Revise and edit


**Redesign of a bar chart**

The data-ink ratio on this chart can be reduced significantly by taking the following actions:

![Reducing data-ink](https://images.squarespace-cdn.com/content/v1/56713bf4dc5cb41142f28d1f/1450306653111-70K5IT30R69NWPDIE1ZJ/data-ink.gif){: width="70%" align=right}

- remove backgrounds
- remove redundant labels
- remove broders
- remove colours
- remove special effects
- remove bolding
- lighten labels
- lighten lines or remove lines
- direct label

Remember, 'less is more'



## Contrast

Contrast directs the user's attention to focal point in your dashboard, highlighting important information to achieve impact.

It is also crucial for practical reasons. For instance, text should have a [contrast ratio of at least 3:1](https://www.w3.org/TR/WCAG20-TECHS/G183.html) to ensure your dashboard is accessible to all users.

Contrast in size, shape and colour are all important to ensure your dashboard is successful in achieving its specific goal. With no contrast all, you'd just end up with a single colored block for a dashboard!


## Size and Scale

Size and scale are used in visual hierarchy to communicate prioritized information.

Size refers to the physical dimensions of an element, while scale defines its proportion relative to other elements on the page. Large elements generally attract more attention in the hierarchy, while smaller ones are secondary.

Manipulating the size and scale of your dashboard components creates a sense of perspective, guiding users to focus on the most important information first.



## Naming conventions

Naming of products is key, particularly in the context of an A-Z product list within the core platform.
We are aware from user research that discoverability of products is an issue.
Naming of products is a key aspect to be addressed to improve discoverability.
Alongside the name, the brief description is also valuable in helping the user find the data they are looking for.


!!! tip "Guidelines for naming new dashboards"

        1. Start with key word(s) eg Cancer, COVID, A&E
        2. Consider frequency eg daily, weekly, monthly
        3. Describe functionality eg monitoring, performance, forecasting, benchmarking


**Keep it simple and descriptive**

Avoid unnecessary words and especially at the start of the name where it affects the alphabetical listing.
Where possible avoid using acronyms.
If an acronym needs to be included in the product title, ensure it is also written out in full.
Eg Summary emergency department indicator table (SEDIT)


**Consider alphabetical listing**

Ensure the key word(s) is at the start of the sentence, this also ensures similar dashboards are grouped together.
Do not start the name with 'the'.
Eg 'The long stays' dashboard would appear under 't' in an alphabetical list, use 'Long stays' instead.

Avoid starting names with 'NHS' or 'national' for the same alphabetical clustering reason.
There may be exceptions eg 'NHS 111'


**Case Type**

Capitalisation is generally to be avoided in accordance with NHS style guidelines.
Titles should use sentence case as per the NHS England style [guidelines](https://nhsengland.sharepoint.com/sites/Content/SitePages/House-style.aspx?), capitalisation just like in standard English sentences, where only the first word of each sentence and proper nouns are capitalised.


!!! tip "Managing versions"
        If an updated version of a dashboard is released it should ideally replace the previous version and use the exisiting name.
        However if it is required for a new version to be added and the previous version to be still available then it should be clearly distinguishable
        eg 'A&E daily performance (new)' and 'A&E daily performance (2021).



## Dealing with data quality issues

Sharing known data quality issues can reduce misinterpretation of data.


**Data quality check list**

Unfortunately the data we use is not always 100% complete, or 100% accurate.
Adding a page to the dashboard or linking to a supporting web page to include information on data quality can be very useful for users.
Try adding information such as:

- Missing submissions
- Known missing or incorrect data
- Dates highlighting when new metrics were introduced or methodolgies were changed
- Known data quality issues



The data quality page and metric descriptions page can be combined into one metric information page.



??? info "_External Links Disclaimer_"

    *NHS England makes every effort to ensure that external links are accurate, up to date and relevant, however we cannot take responsibility for pages maintained by external providers.*

    *NHS England is not affiliated with any of the websites or companies in the links to external websites.*

    *If you come across any external links that do not work, we would be grateful if you could report them by raising an issue on our [Data Viz Community of Practice GitHub](https://github.com/NHSDigital/data-viz-community-of-practice).*