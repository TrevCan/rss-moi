# rss-moi
iOS shortcut to fetch RSS feeds from files, select articles to read and open them in a web browser.

*[view](/media/demo.gif) in action!*

# features
- works with almost any URLs you can share!
- can fetch feeds form remote url.
- can automatically copy from clipboard.
- set default feed.
- choose which articles to read and open them.

# install
- Make sure you have enabled the *untrusted shortcuts* option in `Settings -> Shortcuts`.
- Make sure to have the [dependencies](#dependencies) installed.
- See the [latest](https//github.com/trevcan/rss-moi/releases) 
release. Access the icloud link, then click on the [icloud](https://www.icloud.com/shortcuts/4ced91389cea45738998d5ca9e177d49)
link. Open it with the Shortcuts app, scroll down and click on add shortcut.

## usage
- you can either:
	- a) give it a file or a text selection and choose which feeds to view, or
	- b) launch it from the homescreen and be prompted to type the feeds.
	- c) automatically use the clipboard.
- have a list of rss/atom feeds, either in a text file, in your notes,
or somewhere you can select text. (see [demo](/media/demo.gif)
  - select the list of urls and click on *share*, then select the `RSS-moi` shortcut.
  - you will be asked to select which feeds you want to use.
- **for each feed, you will have to select at least one article to read. After going through all your selected feeds, the URLs open in Safari.**
- You can also run the shortcut with no entry info, meaning you can invoke it [from your home screen](https://support.apple.com/guide/shortcuts/add-a-shortcut-to-the-home-screen-apd735880972/ios).
  - if you do this, you will be prompted to write the URLs, you can paste links of course.
  - **if you'd like to use the clipboard**, you can edit the shortcut configuration (simply change the `paste` key to `true`. It is located inside the dictionary, below the comments at the top.)
- you can also retrieve the list of feed URLs from a remote URL (e.g. from a raw gist)
  - to enable this, simply change the `get_from` key in the dictionary to any URl of your choice that
  hosts your list of URL feeds. *Note that any non-valid RSS feeds might cause the app to break (see: [known-issues](#known-issues))*


### dependencies
- iOS Shortcuts App. [install here](https://apps.apple.com/us/app/shortcuts/id915249334)
  - make sure to have the option 'untrusted shortcuts' in the settings app (-> Shortcuts) enabled. More info [here](https://support.apple.com/en-us/HT210628)

### FAQ
- how did I export the iOS shortcut to a file ?
  - I followed [this article's instructions](https://www.addictivetips.com/ios/save-iphone-shortcut-offline/).
  - Although it didn't work at first, I **removed** the last instruction and added one that saved the Resulting element to a file.
  - [here is my modified version of the shortcut exporter](https://www.icloud.com/shortcuts/cde4969f06b14a47ab6a6df46d404326)
  - *note: to import shortcuts you **must first** move them to your iCloud Drive.*


### known issues
- you have to select- *at least* - for each feed, **one article.**
- any urls that are not RSS links can break the Shortcut.



# license
Licensed under the MIT License. see the [license](/LICENSE) file.
