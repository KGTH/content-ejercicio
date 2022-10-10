# Content

## Types of content:

This list of contents is just a draft, some can be deleted or more can be added.

  1. Lessons: Long articles explaining big concepts like: HTML, JS Events, CSS Selectors, etc.
  2. Error: Explanation of a particular error that typically occurs when coding, for example: "Cannot do map of undefined".
  3. How To: Small articles/videos on different shot how to's, like: How to start a new react.js project.

##  Tagging content:

Contents can be tagged on the header of the markdown file; you can add as many tags as you want and later people will be able to search by tag.

There are two types of tags: Technology and Category.

## Command Line Interface:

A small command-line tool has been developed to help manage the lessons.

```
$ node ./src/utils/cli.js update_lesson --slug all --statusTo draft --statusFrom null
$ node ./src/utils/cli.js update_lesson --slug learn-html --statusTo draft --statusFrom null
$ node ./src/utils/cli.js download_images --slug python-syntax --type external_images
$ node ./src/utils/cli.js localize_images --slug python-syntax --type external_images
$ node ./src/utils/cli.js sanitize_lesson --slug all
```

### Method: sanitize_lesson

Will try to clean and fix any possible issues on the lessons, for example: Date formats

### Method: update_lesson

| PARAM         | DESCRIPTION |
| ---------     | ----------- |
| --slug        | Every lesson has a slug that identifies it, you can pass `all` if you want to update all at once |
| --statusTo    | change the status of one or all the lessons to a particular one |
| --statusFrom  | only apply changes to lessons with specified status |

### Method: download_images 1

| PARAM         | DESCRIPTION |
| ---------     | ----------- |
| --slug        | Every lesson has a slug that identifies it, you can pass `all` if you want to update all at once |
| --type  | external_images or uploadcare |

### Method: localize_images


### Method: download_images download_images` 2

| PARAM         | DESCRIPTION |
| ---------     | ----------- |
| --slug        | Every lesson has a slug that identifies it, you can pass `all` if you want to update all at once |
| --statusTo    | change the status of one or all the lessons to a particular one |
| --statusFrom  | only apply changes to lessons with specified status |
