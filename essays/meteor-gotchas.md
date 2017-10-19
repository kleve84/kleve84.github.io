---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-10-19
labels:
  - Software Engineering
  - Meteor
---


## Problem Uno

Working with Meteor hasn't been easy. There are many concepts and files to look for when working with the provided templates. My first problem during the development of the digits application was import statements, such as:

```
import './list-stuff-page.html';
import './list-stuff-page.js';
```

Forgetting to use the aformentioned code caused my application to not display any data, causing me to question if my implementation was correct as it was common to copy another file and forget to update the import statements. I solved this by always changing the import statements in the javascript file and index file when I created a new file. This has dramatically cut down on the time I used to spent searching for the missing import statement.


## Problem Dva

A second problem I encountered was using the spacebar templates in the digits application. I know that we use spacebars to create custom helpers, such as:

```
{{header}};
{{footer}};
```

Still, I have trouble using spacebars to iterate through a collection or check the validity of a statement. This is due to the fact that much of our digits application so far has been using the template of another file, reducing the need to know what spacebars are capable of. I am working on this issue by doing a workout without copy and pasting so it becomes second-hand knowledge.

