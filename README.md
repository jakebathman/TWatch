# TWatch: Twitch Chat Watcher

Ever wanted to be alerted when you're @mentioned, when one of your friends posts a message, or when someone mentions a giveaway?

This will play a sound and show a popup alert (both optional) for any of those, and is customizable for the users or words you want to watch in any Twitch chat window.

If you have any problems of suggestions, open a new issue: https://github.com/jakebathman/TWatch/issues

Happy streaming!

## Settings backup

### OH MY GOD WHERE DID MY SETTINGS GO?!!

If you updated this script from an older version, the "config" section below might not have your stuff anymore.

This is a crappy side effect of Tampermonkey scripts, and there's not a very good way to handle it.

BUT: We might be able to get them back. Follow these steps:

1. Go to twitch.tv
2. Open up DevTools Console by pressing F12 or right-clicking the page and selecting "Inspect"
3. Click the "Application" tab at the top (it might be hiding behind the >> icon)
4. Expand the "Local Storage" section
5. Find the "Key" called "TWatchSettings:v1.0.0" (if there are multiple, find the highest version number)
6. Copy the "Value" next to that key and paste below into the "config" section, like this:

```
    var Twatch = {
      config:
      {
        // Paste it here, removing any duplicate keys like "watchTheseUsers" that already exist
      },

      ...
    }
```

Hopefully this works, and I'm sorry if it didn't. Again, there's not a very good way to handle user configs when a script needs updating.

If you have trouble, find me on Twitter @jakebathman or open an issue on GitHub at https://github.com/jakebathman/TWatch/issues
