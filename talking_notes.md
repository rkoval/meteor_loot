# Setup: 
- Browser at localhost:3000
- Browser left side of screen, vim right side of screen with meteor_loot.html and meteor_loot.js in a vsplit
- Terminal in another space
- `git checkout master~#`
- Robomongo started up to tasks DB
- Make sure all collections are empty


# Demo procedure and talking notes:

1. Talk about install
  - `meteor create meteor_loot` is what you'd run
  - Walk through directory generate
1. step 1 - startup lame app
  - mention spacebars syntax; similar to handlebars or angular... mention data binding
  - Talk about `<head/>`, `<body/>`, and `<template/>`
  - Everything inside any <head> tags is added to the head section of the HTML sent to the client, and everything inside <body> tags is added to the body section, just like in a regular HTML file.
  - Everything inside `<template>` tags is compiled into Meteor templates, which can be included inside HTML with `{{> templateName}}` or referenced in your JavaScript with Template.templateName.
1. step 2 - adding some styling
  - demonstrate hot-reload
1. step 3 - actual mongo querying
  - mention internal `meteor mongo`
  - run insert in Mongo and demonstrate reactive add
    - `db.tasks.insert({ text: "Hello world!", createdAt: new Date() });`
1. step 4 - add form
  - walk through code
  - add tasks and show them in mongo
1. step 5 - CRUD
  - talk about how "this" is set within the #each
1. step 6 - hide completed
  - talk about Session helper object
1. step 7 - ios
  - `meteor install-sdk ios`
  - `meteor add-platform ios`
  - `meteor run ios`
1. step 8 - added UI widgets and password
  - `meteor add accounts-ui accounts-password`
  - default password encryption scheme uses bcrypt
  - `meteor add accounts-facebook`
1. step 9 - remove insecure module
  - `meteor remove insecure`
  - added methods - real latency compensation
1. step 10 - remove autopublish
  - `meteor remove autopublish`
