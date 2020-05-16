# F5 Solutions Engineering GitHub Page
This repository hosts the F5 Solutions Engineering GitHub Page.  This page is used to store information on the repositories hosted within the F5 Solutions Engineering Organization. 

# Contributing
To contribute to this repository please issue a pull request.

## Development Requirements
This GitHub page uses Jekyll so you will need:
 * Ruby 2.6+
 * Jekyll 4.x+
 * pyspelling

To install Jekyll, please reference the official (installation guide)[https://jekyllrb.com/docs/installation/]: 

Run the following command to test your changes locally:
```bash
jekyll clean && bundle exec jekyll serve --incremental
```

### Spell Checking
Please use pyspelling to ensure all words are spelled correctly.  If the spell check needs a new word, add it to the wordlist.txt file.
``` bash
pyspelling -c spellcheck.yaml
```