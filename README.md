# open-data-certificate-help
Help for the Australian localisation of the ODI [Open Data Certificates](https://certificates.theodi.org).

This help text is pasted into the [ODI Queensland](http://queensland.theodi.org) Wordpress site. This repository was created as there is no way to keep track of changes in Wordpress and as a way for people to make contributions (via [issues](https://github.com/ODIQueensland/open-data-certificate-help/issues)) and pull requests.

If you're not comfortable with Github, you can discuss your ideas for open data certificates on [Ask ODI Queensland](https://ask.theodi.org.au/c/projects/certificates).

There are 4 help pages:

- [Introduction](http://queensland.theodi.org/home/services/certificates/help/) (not managed here).
- [Rights](http://queensland.theodi.org/home/services/certificates/help/rights/) (code [rights.html](https://github.com/ODIQueensland/open-data-certificate-help/blob/master/rights.html))
- [Licencing](http://queensland.theodi.org/home/services/certificates/help/licensing/) (code [licensing.html](https://github.com/ODIQueensland/open-data-certificate-help/blob/master/licensing.html))
- [Privacy](http://queensland.theodi.org/home/services/certificates/help/privacy/) (code [privacy.html](https://github.com/ODIQueensland/open-data-certificate-help/blob/master/privacy.html))

They are structured to mimic the online questionnaire so they could be used for training as well as supporting people completing the questionnaire.

## Components

The open data certificate help pages contained here are made up of a number of components.

### Question

Repeated from the online questionnaire.

1. Question text
2. Question description (optional)

### Answers

Repeated from the online questionnaire.

1. Answer text
2. Answer description (optional)
3. What question to ask next if this answer is selected

### Extra Help

Each question in the survey can contain a link to extra guidance outside the questionnaire:


## Formatting

Each of the above components are formatted in a specific way. Examples are shown below. Some of these may appear strange from a normal html formatting approach but there are a set of constraints imposed by using a Wordpress site that we don't have full administration rights to.

### Question text

This text should match the online questionnaire.

Add a horizontal line with an id so when the internal link is followed the Question text appears at the top of the page.
Add strong to `<h2>`. Yes, I know, CSS, but constraints :-(

    <hr id="publisherrights" />
    &nbsp;
    <h2><strong>1. Do you have the rights to publish this data as open data?</strong></h2>

### Question description

This text should match the online questionnaire. The text doesn't need to be wrapped in `<p> </p>` as Wordpress applies these automatically. Add links to the glossary as required.

    You should have a clear legal <a href="/glossary#rights">right</a> to publish this data. If your organisation didn't originally create or gather this data then you might not have the right to publish it. If you’re not sure, check with the <a href="/glossary#rights-holder">rights holder</a> (owner) because you will need their permission to publish it.

### Answer text

    <h5>Yes</h5>

### Answer description

    You have the right to publish the data as open data if you collected all the data yourself.

### What question is asked next

The `title` is the wording of the next question.

    <p align="right"><a title="Was all this data originally created or gathered by you?" href="#publisherorigins">Next: Question 2</a></p>

### Help text

This is the text that provides the extra help or links to resources. There are some different classes that adjust the formatting:

- `note` and `note-title` are used to wrap the text in a green box
- `example` and `example-title` are used to wrap the text in a yellow box
- `warning` and `warning-title` are used to wrap the text in a red box

    <div class="note">
    <div class="note-title">Note</div>
    If you are unsure, the Open Data Certificate questionnaire will lead you through a series of questions to help you determine if you have the rights to publish this data. It will ask if all the data was gathered by you and if not, what were the sources of the data and if they are openly licensed.

    </div>
