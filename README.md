# pa11y-tool

A tool for running Pa11y against URLs in bulk

## Install and run

-   Run `npm i`
-   Run `npm start` (bulk)
-   Run `npm run pa11y` (single url)

## Running

### Bulk

-   Add the list of urls you want to test to the array in `data/input.json`
-   The output should be in the `data/output.json` file

### Single

-   Add the url you want to test in the `pa11y` script command in the `package` file (after the `URL=` parameter)
-   The output should be shown in the terminal

## Example output:

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

## TODO

-   Show warnings by default and get this working
-   Display the results nicely
-   Ability to ignore certian rules
-   Add element reference the issue was discovered on
-   Add reference to related WCAG criteria
-   Add ability to pass the url into the single task command

## Credit

Adapted from - https://github.com/mmacartney10/pa11y-child-processes-super-quick by Matt Macartney.
