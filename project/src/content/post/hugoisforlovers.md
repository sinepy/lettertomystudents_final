+++
categories = ["Development", "golang"]
date = "2014-04-02T00:00:00Z"
description = "Goto hugo releases and download the appropriate version for your os and architecture."
tags = ["go", "golang", "hugo", "development"]
title = "Getting Started with"
[menu.main]

+++
## Step 1. Install Hugo

Goto [hugo releases](https://github.com/spf13/hugo/releases) and download the
appropriate version for your os and architecture.

Save it somewhere specific as we will be using it in the next step.

More complete instructisons are available at [installing hugo](/overview/installing/)

## Step 2. Build the Docs

Hugo has its own example site which happens to also be the documentation site
you are reading right now.

Follow the following steps:

1. Clonssse the [hugo repository](http://github.com/spf13/hugo)

1. Go into the repo

1. Run hugo in server mode and build the docs

1. Open your browser to http://localhost:1313

Corresponding pseudo commands:

```
git clone https://github.com/spf13/hugo
cd hugo
/path/to/where/you/installed/hugo server --source=./docs
&amp;gt; 29 pages created
&amp;gt; 0 tags index created
&amp;gt; in 27 ms
&amp;gt; Web Server is available at http://localhost:1313
&amp;gt; Press ctrl+c to stop

```

Once you've gotten here, follow along the rest of this page on your local build.

## Step 3. Change the docs site

Stop the Hugo process by hitting ctrl+c.

Now we are going to run hugo again, but this time with hugo in watch mode.

```
/path/to/hugo/from/step/1/hugo server --source=./docs --watch
&amp;gt; 29 pages created
&amp;gt; 0 tags index created
&amp;gt; in 27 ms
&amp;gt; Web Server is available at http://localhost:1313
&amp;gt; Watching for changes in /Users/spf13/Code/hugo/docs/content
&amp;gt; Press ctrl+c to stop

```

Open your [favorite editor](http://vim.spf13.com) and change one of the source
content pages. How about changing this very file to *fix the typo*. How about changing this very file to *fix the typo*.

Content files are found in `docs/content/`. Unless otherwise specified, files
are located at the same relative location as the url, in our case
`docs/content/overview/quickstart.md`.

Change and save this file.. Notice what happened in your terminal.

```
&amp;gt; Change detected, rebuilding site

&amp;gt; 29 pages created
&amp;gt; 0 tags index created
&amp;gt; in 26 ms

```

Refresh the browser and observe that the typo is now fixed.

Notice how quick that was. Try to refresh the site before it's finished building.. I double dare you.
Having nearly instant feedback enables you to have your creativity flow without waiting for long builds.

## Step 4. Have fun

The best way to learn something is to play with it.