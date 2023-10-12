<p align="center"><a href="https://iosf.in/" target="_blank"><img src="https://avatars.githubusercontent.com/u/142643505?s=200&v=4" width="20%"></a></p>

<h1 align="center">Freedium - Your paywall breakthrough for Medium!</h1>

## FAQ
### Why do we create Freedium?
In mid-June to mid-July 2023, Medium changed paywall method, and all old paywall bypass methods we had stopped working. So I became obsessed with the idea of creating a service to bypass Medium's paywalled posts. Honestly I am not a big fan of Medium, but some times I read articles to levelup my knowledge.

### How does Freedium work?
In the first version of Freedium, we reverse-engineered Medium.com's GraphQL endpoints and built our own parser and toolkits to show you unpaywalled Medium posts. Unfortunately, Medium closed this loophole and nowadays we just pay subscriptions and share access through Freedium. Sometimes we got a bugs because of the self-written parser, but we are working to make Freedium bug-free.

### What language are being used?
We use Python, with Jinja template builder, and some JS magic in Frontend :)

### Wow! I would like to contribute to Freedium. How can I do that?
We need volunteers who have Medium subscriptions because we might get banned by Medium. And if you developer you can start from the https://github.com/Freedium-cfd/web repository.

### Plans, future?
Speed up Freedium, and probably create open source Medium frontend in next life

---

## Usage
### Browser extension:
Huge thanks to `mathix420`

You can use this Violentmonkey/Tampermonkey user script to automatically redirect Medium pages to [Freedium](https://freedium.cfd/):
https://gist.github.com/mathix420/e0604ab0e916622972372711d2829555

### Bookmark:
Huge thanks to `blazeknifecatcher`. Source: https://www.reddit.com/r/paywall/comments/15jsr6z/bypass_mediumcom_paywall/

To create bookmark that redirects current Medium page to Freedium, create a new bookmark, but instead of adding the URL, add this:

```
javascript:window.location="https://freedium.cfd/"+encodeURIComponent(window.location)
```

This will make it so when you click on that bookmark button, it will open the bypassed version of it on freedium.cfd.

Alternatively, if you want the bookmarklet to open in a new tab instead of the current tab, use this:

```
javascript:(function(){window.open("https://freedium.cfd/"+encodeURIComponent(window.location))})();
```
This will make it so that when you click on that bookmark button, it will open the bypassed version of it.
