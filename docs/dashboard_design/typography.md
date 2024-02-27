Typefaces are an important element of the NHS identity. The consistent application of NHS typefaces creates a unified brand which patients and the public can trust.</p>

## Fonts
!!! info inline end "Did you know...?"
    Frutiger is the primary typeface of the NHS. However, **Arial should be used in all NHS data products** as Frutiger is not always available!

!!! danger "You must use Arial font"
    - Set your default font to be Arial before starting development
    - Font size should not be smaller than size 10
    - Use "<ins>T</ins>itle <ins>C</ins>ase" for dashboard titles. Else: use "<ins>S</ins>entence case" 


## Best Practices

???+ tip "Typography - Best practices"
    - [x] Use concise language, which is to the point and easy to understand
    - [ ] Avoid abbreviations, technical jargon and acronyms where possible
    - [x] If using acronyms, explain them the first time they appear (or in a tooltip)
    - [ ] Avoid using large blocks of text, especially when used in combination with charts
    - [x] Use contrast to **emphasise key information** and deemphasise what is less important
    - [ ] don't go into details of the methods, but perhaps highlight some of the key approaches described below

### Example dashboard with typography specification

![example dashboard layout with font specification](images/font-specification-example.PNG "Example dashboard layout with NHS Font specification applied")

## Font Specification

Here is a summary of the most important dashboard objects and their font specification that you must use in your dashboard:

| **Objects**                  | **Font** | **Weight** | **Size**    | **Colour**     | **HEX**      | **Alignment** |
|------------------------------|----------|------------|-------------|----------------|--------------|---------------|
| Dashboard title              | Arial    | Bold       | 24px / 18pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
| Chart heading / Card heading                | Arial    | Bold       | 16px / 12pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
| Filter title                 | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
| Description / Paragraph      | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px""></span>#4C6272</span>       | Left          |

To reveal the full font specification, please click the box below:

???- success "Full Font specification"

    | **Objects**                  | **Font** | **Weight** | **Size**    | **Colour**     | **HEX**      | **Alignment** |
    |------------------------------|----------|------------|-------------|----------------|--------------|---------------|
    | Dashboard title              | Arial    | Bold       | 24px / 18pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Tab name in title            | Arial    | Regular    | 24px / 18pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Description / Paragraph      | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px""></span>#4C6272</span>       | Left          |
    | Info / Warning Message       | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px""></span>#4C6272</span>       | Left          |
    | Date                         | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px""></span>#4C6272</span>       | Left          |
    | KPI heading                  | Arial    | Bold       | 15px / 11pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | KPI heading as link          | Arial    | Bold       | 15px / 11pt | NHS Blue       | <span class="inline-container-pill" style="--colour: #005EB8; background-color: white"><span class="inline-colour-square" style="--colour: #005EB8; height: 15px; width: 15px""></span>#005EB8</span>       | Left          |
    | Metric                       | Arial    | Bold       | 32px / 24pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Metric in brackets           | Arial    | Regular    | 24px / 18pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Metric decrease              | Arial    | Bold       | 15px / 11pt | NHS Dark Red   | <span class="inline-container-pill" style="--colour: #8A1538; background-color: white"><span class="inline-colour-square" style="--colour: #8A1538; height: 15px; width: 15px""></span>#8A1538</span>       | Left          |
    | Metric decrease in brackets  | Arial    | Regular    | 15px / 11pt | NHS Dark Red   | <span class="inline-container-pill" style="--colour: #8A1538; background-color: white"><span class="inline-colour-square" style="--colour: #8A1538; height: 15px; width: 15px""></span>#8A1538</span>       | Left          |
    | Metric increase              | Arial    | Bold       | 15px / 11pt | NHS Dark Green | <span class="inline-container-pill" style="--colour: #007F3B; background-color: white"><span class="inline-colour-square" style="--colour: #007F3B; height: 15px; width: 15px""></span>#007F3B</span>       | Left          |
    | Metric increase in brackets  | Arial    | Regular    | 15px / 11pt | NHS Dark Green | <span class="inline-container-pill" style="--colour: #007F3B; background-color: white"><span class="inline-colour-square" style="--colour: #007F3B; height: 15px; width: 15px""></span>#007F3B</span>       | Left          |
    | Controls heading             | Arial    | Bold       | 16px / 12pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | X-axis / Y-axis variables    | Arial    | Regular    | 13px / 10pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Centre        |
    | Value on bars (light colour) | Arial    | Regular    | 13px / 10pt | NHS Grey 5     | <span class="inline-container-pill" style="--colour: #F2F2F2; background-color: white"><span class="inline-colour-square" style="--colour: #F2F2F2; height: 15px; width: 15px"></span>#F2F2F2</span>       | Centre        |
    | Value on bars (dark colour)  | Arial    | Regular    | 13px / 10pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Centre        |
    | Caption                      | Arial    | Regular    | 13px / 10pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Filter title                 | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Filter body                  | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Table heading                | Arial    | Bold       | 16px / 12pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Table column heading         | Arial    | Bold       | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Table column sub-heading     | Arial    | Bold       | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Table row heading            | Arial    | Bold       | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Table body / rows            | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Tooltip heading              | Arial    | Bold       | 16px / 12pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Tooltip description          | Arial    | Regular    | 15px / 11pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | Button text                  | Arial    | Bold       | 16px / 12pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Hyperlink                    | Arial    | Regular    | 16px / 12pt | NHS Blue       | <span class="inline-container-pill" style="--colour: #005EB8; background-color: white"><span class="inline-colour-square" style="--colour: #005EB8; height: 15px; width: 15px""></span>#005EB8</span>       | Left          |
    | Chart heading                | Arial    | Bold       | 16px / 12pt | NHS Black      | <span class="inline-container-pill" style="--colour: #212B32; background-color: white"><span class="inline-colour-square" style="--colour: #212B32; height: 15px; width: 15px""></span>#212B32</span>       | Left          |
    | Legends                      | Arial    | Regular    | 13px / 10pt | NHS Grey 1     | <span class="inline-container-pill" style="--colour: #4C6272; background-color: white"><span class="inline-colour-square" style="--colour: #4C6272; height: 15px; width: 15px"></span>#4C6272</span>       | Left          |
    | X-axis / Y-axis labels       | Arial    | Regular    | 12px / 9pt  | NHS Grey 3     | <span class="inline-container-pill" style="--colour: #768692; background-color: white"><span class="inline-colour-square" style="--colour: #768692; height: 15px; width: 15px"></span>#768692</span>       | Centre        |
