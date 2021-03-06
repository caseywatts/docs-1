---
title: "Fetching Exercises"
slug: "fetching-exercises"
category: "process"
ordinal: 2
---

First log in to the command-line client:

```bash
$ exercism login
```

You will be asked for your API key, which can be found in your account settings.

To fetch your current exercises, issue the command:

```bash
$ exercism fetch [language]
```

Or you can fetch all languages:

```bash
$ exercism fetch
```

The program will download the exercises to the configured project directory.

Note that the code will be put in that directory even if you are somewhere else on the filesystem when calling `exercism fetch`.

To start working on an exercise, go find the downloaded files.

```bash
$ cd path/to/exercism/project # or whatever
```

You can work on them using your usual editor, tools, and environment. Read the <a class="link-side-menu" href="#sidr">getting started guide</a> of your language to find out how to run the tests.

As soon as you have submitted code to an exercise, `exercism fetch` will provide you with access to the next exercise.

<a class="secondary-button" href="submitting-exercises.html">Submitting Exercises</a>
