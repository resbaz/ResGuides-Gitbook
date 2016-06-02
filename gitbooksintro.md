# Creating your own lessons


#### Follow these instructions to create you own `ResGuides` lesson using this book as a template. 


##Step 1: github

* Create a __copy__ of this repository using the github [importer](https://github.com/new/import). You want to paste this link in to `Your old repository’s clone URL`: https://github.com/resbaz/ResGuides-Gitbook.git

* You will also need to choose an owner for the new (copied) repository, make this [the ResBaz github acccount](https://github.com/resbaz) (if you have access).

* Finally, Make sure to give your new lesson a new name, e.g. `ResGuides: Data Science with Python`


##Step 2: gitbook

Go to [gitbook.com](https://www.gitbook.com), and then click `new book`. This bit is __important__: in the new book window make sure you choose the github option in the top menu. Then scroll down and select the new github repository you set up.

Nice work. This should have set up the webhooks needed to update your gitbook from github. Let's check that by adding some content.


##Step 3: Remove superfluous content

There are a files in the `data` and `examples` directory of this repository that you may want to get rid of (they were included mainly because github doesn't register empty folders).


##Step 4: Adding content

We've created a couple of markdown files to demonstrate a few markdown tricks as well as gitbooks plugins.

##Step 5: Getting started with markdown

[Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)


##Step 6: Book layout 

Your book will automatically have file called SUMMARY.md and place it in the docs directory. This is what dictates the contents tree of the book (or autogenerate). It looks a bit like this:

```
# Table of content 
* [Getting Started](docs/getting-started.md)
* [API Reference](docs/api-reference.md)
```

We have created a flat structure i.e. all pages (markdown files just appear one after the other), but you can have nested contents, i.e. chapters, sections...

##Step 7: Plugins

When you are in the online editor on gitbook.com, there is a dropdown icon at the far riht of the screen. Click on this an then on `plugins store`. Selecting a plugin will add the plugin you selected by pasting the required json snippet into the book.json file. 

* Note that plugins are a common source of gitbook build errors. If stuff starts acting weirdly after you activated a new plugin, consider deactivating that plugin as a first check (deactivate the plugin from the same plugins store)


```json
{
    "plugins": ["mathjax"]
}

```

##Step 8: When builds go wrong

coming soon


###Links, blogs, resources

[useful blog post](https://medium.com/@gpbl/how-to-use-gitbook-to-publish-docs-for-your-open-source-npm-packages-465dd8d5bfba#.acdr3enfr)




