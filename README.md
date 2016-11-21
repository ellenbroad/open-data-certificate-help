# open-data-certificate-help
Help for the Australian localisation of the ODI [Open Data Certificates](https://certificates.theodi.org).

This help text is pasted into the [ODI Queensland](http://queensland.theodi.org) Wordpress site. This repository was created as there is no way to keep track of changes in Wordpress and as a way for people to make contributions (via [issues](https://github.com/ODIQueensland/open-data-certificate-help/issues)) and pull requests.

If you're not comfortable with Github, you can discuss your ideas for open data certificates on [Ask ODI Queensland](https://ask.theodi.org.au/c/projects/certificates).

There are 4 help pages:

- [Introduction](http://queensland.theodi.org/home/services/certificates/help/) (not managed here).
- [Rights](http://queensland.theodi.org/home/services/certificates/help/rights/) (code [rights.html](https://github.com/ODIQueensland/open-data-certificate-help/blob/master/rights.html))
- [Licencing](http://queensland.theodi.org/home/services/certificates/help/licensing/) (code [licensing.html](https://github.com/ODIQueensland/open-data-certificate-help/blob/master/licensing.html))
- [Privacy](http://queensland.theodi.org/home/services/certificates/help/privacy/) (code [privacy.html](https://github.com/ODIQueensland/open-data-certificate-help/blob/master/privacy.html))

## Components

The open data certificate questionnaire is made up of a number of components. Some of these are repeated in this help.

### Question

1. Question text
2. Question description
3. Question help (as shown in the questionnaire)

### Answers

For each possible answer to a question:

1. Answer text
2. Answer description
3. Answer help
4. What question to ask next if this answer is selected

### Extra Help

The extra help can contain:

1. Guidance text
2. Examples

## Formatting

Each of the above components are formatted in a specific way. Some of these may appear strange from a normal html formatting approach but there are a set of constraints imposed by using Wordpress and a site we're not in complete control of that cause these.

### Question text

Add a horizontal line with an id so when the internal link is followed the Question text appears at the top of the page.
Add strong to `<h2>`. Yes, I know, CSS, but constraints :-(

    <hr id="publisherrights" />
    &nbsp;
    <h2><strong>1. Do you have the rights to publish this data as open data?</strong></h2>
    You should have a clear legal <a href="/glossary#rights">right</a> to publish this data. If your organisation didn't originally create or gather this data then you might not have the right to publish it. If you’re not sure, check with the <a href="/glossary#rights-holder">rights holder</a> (owner) because you will need their permission to publish it.

### Question description

### Question help

### Answer description

### Answer help

### What question to ask next if this answer is selected

### Guidance text

### Examples
