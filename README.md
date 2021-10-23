# pa11y-tool

A tool for running Pa11y against URLs in bulk

-   Run `npm install`
-   Add the list of urls you want to test to `data/input.json`
-   Run `npm start`
-   The output should be in the `data/output.json` file.

# The output file will be an structured as follows:

```
{
    "Here is an issue": [
        "url that breaks this issue"
    ],
    "Duplicate id attribute value \"google\" found on the web page.": [
        "https://www.google.com",
        "https://www.example.com"
    ]
}
```

TODO:

-   Show warnings by default and get this working
-   Display the results nicely
-   Ability to ignore certian rules
-   Add element reference the issue was discovered on
-   Add reference to related WCAG guideline
