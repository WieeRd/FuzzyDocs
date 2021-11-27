# FuzzyDocs
Discord Bot that can fuzzy search *ANY* document based on Sphinx.  
( = Every document in readthedocs.io)

## 1. Basic Usage
- Usage
```
?doc <name[/lang][/version]> <keyword>
?doc <url> <keyword>
```
- Example
```
?doc discordpy msg.ref
?doc discordpy/stable msg.ref
?doc discordpy/en/stable msg.ref
?doc https://discordpy.readthedocs.io/en/stable msg.re
```
The desired result of commands above would be [`Message.reference`](https://discordpy.readthedocs.io/en/stable/api.html#discord.Message.reference).

## 2. Adding Alias
- Usage
```
?alias <alias> <name/url>
?remove <alias...>
```
- Example
```
?alias dpy1 discordpy
?alias dpy2 discordpy/master

?doc dpy1 msg.re
?doc dpy2 ui.view

?remove dpy1 dpy2
```

## 3. Set Default
- Usage
```
?default <name/alias>
```
- Example
```
?default dpy2
?doc msg.re
```

## 4. Others
- Usage
```
?help
?list
?refresh
```
- Holy Shit
```
I can't believe it's already been 2 months since I came up with this project idea.
And I haven't even touched it. O_o
```
