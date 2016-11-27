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

Each question in the survey can contain a link to extra guidance found inside these help pages. This extra guidance is formatted to make it stand out from the elements copied from the questionnaire.

## The questionnaire

The Australian questionnaire is being drafted at https://github.com/Stephen-Gates/open-data-certificate/blob/staging/prototype/jurisdictions/certificate.AU.xml

Once complete is will be merged into [Staging](https://github.com/theodi/open-data-certificate/blob/staging/prototype/jurisdictions/certificate.AU.xml).

And eventually [Production](https://github.com/theodi/open-data-certificate/blob/master/prototype/jurisdictions/certificate.AU.xml).

## Answering questions automatically
If your data is published in a CKAN portal, some questions should have been automatically answered by reading the metadata available via the CKAN API. The following CKAN fields are read by Data Kitten to attempt to answer questions automatically

- title
- description
- publishers
- maintainers
- contributors
- rights
- licenses
- update_frequency
- keywords
- issued
- modified
- temporal
- distributions
- title
- description
- access_url
- extension
- open
- structured
