---
layout: post
title: "Why I Use Firefox"
author: Pudo
categories: [ software, productivity ]
---
# Why I Use Firefox

  So I'm one of *those* people that uses Firefox instead of some derivative of
  Chromium. Here's why.

## The Power of Bookmarks

Bookmarks on Firefox are far more powerful on Firefox than on their Chrome
counterparts. One of the main features that I use multiple times per day is the
**keyword** feature for bookmarks. This allows you to access commonly visited
sites using the keyboard, instead of having to look through your bookmarks bar
or browser history for a webpage. For instance, you could have the short string
`yt` redirect you to the YouTube homepage, or `sub` to take you directly to your
subscriptions.

<p align="center"> <img width = "900"
src="https://raw.githubusercontent.com/poweruserdo/poweruserdo.github.io/main/_posts/2021-02-17-firefox/yt.gif">
</p>

This is great if you just want to access a few basic sites with your keyboard,
but most search engines are already good enough at predicting where you want to
go within a few keystrokes. What sets bookmarks in Firefox apart from other
browsers is the fact that they are also very *extensible*. Just like functions
in any programming language, bookmarks can take *parameters* and change their
behaviour accordingly. 

For example, if I search the phrase `yt 3b1b`, I don't just get taken to some
arbitrary search result. Firefox will take the `3b1b` from my search query and
actually *pass it in as a search term* to YouTube, taking me to the following
page:


<p align="center"> <img width = "900"
src="https://raw.githubusercontent.com/poweruserdo/poweruserdo.github.io/main/yt3b1b.gif">
</p>

As you can see, this is a tremendously useful tool, saving time in comparison to
waiting for pages to load, finding that particular website's search bar, and
then fielding a query. 

How can you create these bookmarks yourself? Simple, just visit the site that
you want to implement this on, find the search bar, and right click. A drop-down
menu should appear---click "Add a Keyword for this Search". This will
automatically create a new bookmark for you, with the `%s` already put in the
right spot for you.

The way that this is implemented is actually ridiculously simple---Firefox just
finds the `%s` tag and replaces it with your parameter string. In the previous
example, when you search `yt 3b1b`, Firefox takes the `3b1b` out and passes that
into YouTube's own search engine.

Note: If your site does not necessarily have a search bar, you can still "guess"
where the `%s` should go. It is usually prefixed by `?q=` or `?s=`, which mean
"query" and "search".

Note 2: If you want to be able to pass more than one parameter into your
bookmark, you'll [need to know a bit of JavaScript](https://outline.com/uVzXLq).

Another major plus for Firefox bookmarks is the ability to hide them away.
Having 50 different bookmarks for snippets and search macros can clutter the
bookmarks bar, which isn't great. Chrome does have folders, which can reduce
this clutter, but it's incomparable to Firefox's bookmarks sidebar. By pressing
`Ctrl-b`, you open a sidebar that gives you much more space and versatility in
comparison to only having folders.

<p align="center"> <img width = "400"
src="https://raw.githubusercontent.com/poweruserdo/poweruserdo.github.io/main/bookmarksbar.png">

Finally, as you can see in the above image, the bookmarks sidebar has its own
search bar. What is this for? It allows you to filter and sort through your
various bookmarks, which brings me to another feature of Firefox
bookmarks---tagging. By tagging bookmarks, you can assign them to searchable
categories that will help you find things faster. For instance, I use bookmarks
to keep track of articles that I have read, and tag them to be able to go back
and filter them by topic and author. 

Obviously there are plenty of use cases for Firefox's powerful bookmarks, from
speeding up searches to helping you keep track of resources. They're an
effective tool for bettering the browsing experience and something that I can't
live without.

## Firefox Containers

Tired of always logging in and out of personal/work accounts? In come Firefox's
[Multi-Account
Containers](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/),
an add-on that compartmentalizes your browsing information to groups of tabs. By
isolating cookies, cache, and other data, containers allow for simultaneous
logins on any site. They even include nice color-coding by default so you can
tell which container your tab belongs to at a glance.

## Reopening Tabs in Private Mode

You can press `Ctrl-Shift-t` to open the most recently closed tab, even while in
private mode. That is all.

## Better Adblock Support

I use uBlockOrigin for a speedy, ad-free internet experience. It just so happens
to [work best on
Firefox](https://github.com/gorhill/uBlock/wiki/uBlock-Origin-works-best-on-Firefox).

## Bonus: Default Private Mode for Links

On Android, there's a setting for Firefox to open links in a private window by
default. This can be useful for many things, for instance opening stupid
videos/websites that your friends send you, without having it all saved to your
browser history. You can even set specific URLs to open in specific containers!

As far as I can tell, there's no "official" way to set this up on Windows, so
you'll have to go through with some registry editing to make this happen. [DO
THIS AT YOUR OWN RISK](https://bugzilla.mozilla.org/show_bug.cgi?id=1626644)!
