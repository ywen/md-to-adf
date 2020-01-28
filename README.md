# Markdown to Atlassian Document Format (ADF) translation

Transform Wiki/Markdown text into Confluence/JIRA Atlassian Document Format (ADF) : 
the format use by JIRA and Confluence to describe complex formatted text. 

[![Build Status](https://github.com/b-yond-infinite-network/md-to-adf/workflows/test/badge.svg)](https://github.com/b-yond-infinite-network/md-to-adf/workflows/test/)
[![Codecov](https://codecov.io/gh/b-yond-infinite-network/md-to-adf/branch/master/graph/badge.svg)](https://codecov.io/gh/b-yond-infinite-network/md-to-adf)
[![npm downloads](https://img.shields.io/npm/dm/md-to-adf?style=flat-square)](https://www.npmjs.com/package/md-to-adf)


## Overview
When bridging tools between Github, Wikipedia and other Markdown-based wiki or document system, there's no tool to 
convert the formatted text into the equivalent syntax in JIRA or Confluence. This library does exactly that.
It allows you to take any markdown (Github focussed for now) and translate it into a JIRA/Confluence compatible ADF document.

## Motivation

While writing a Github Action to push Github Issues into JIRA Subtask, we ended up stuck unable to pass complex formatting
from the issue into JIRA, which rendered the interest of the tools much lower.
That's why we embarked on translating Github Markdown into a syntaxically correct ADF document.


## Getting Started

### Install Markdown To ADF

```
npm install md-to-adf
```

### Import/require the translate function:
* As a require
  ```javascript
  const fnTranslate    = require( 'md-to-adf' )
  ```
  
* As a module
  ```javascript
  import fnTranslate from 'md-to-adf'
  ```
  
  
### Pass it the Markdown (Github) formatted text and get the full ADF Document returned

```javascript
const translatedADF = fnTranslate( myJIRAFormattedTextContent )
```

### You're done!


## Additional Documentation 

//  * [](./docs/)
