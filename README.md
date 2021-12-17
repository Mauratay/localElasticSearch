# Full Text search

This template shows how to enable full text search on Firestore documents by using one of the followning hosted search services:


  * [Elastic](https://elastic.co)


## Functions Code

See file [functions/index.js](functions/index.js) for the code.

The dependencies are listed in [functions/package.json](functions/package.json).

## Sample Firestore Structure

As an example we'll be using a secure note structure:

```
/notes
    /note-123456
        text: "This is my first note...",
        owner: "FIREBASE_USER_ID"
    /note-123457
        text: "This is my second note entry...",
        owner: "FIREBASE_USER_ID"
        tags: ["some_category"]
```

Whenever a new note is created or modified a Function sends the content to be indexed.

## Setting up the sample

firebase init emulators [link](https://firebase.google.com/docs/emulator-suite/install_and_configure)

Enable: \n
functions \n
firestore \n
authentication

When going to index.html, refresh a couple of times before indexing.


