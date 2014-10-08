**Know Your Computer**

---

#### Terminal Commands

**I do - you do**

Welcome to the command line. It's not much to look at. No pictures, no fancy art
or animation. Just some text. Let's explore this brand new space. Type `hello?`
and press enter.

```
$ hello?
```

The dollar sign is just to indicate that this is a command line command. It
should not be typed by you. You should only type what follows the dollar sign
(in this case, `hello?`).

Your terminal may have responded rudely.

```
-bash: hello?: command not found
```

This is the way your computer likes to tell you that it did not understand the
command that you typed in. Remember, we have left the GUI world behind us, so we
will no longer have pretty warning messages and alert boxes. Do not worry. In
due time, as we grow comfortable in this new environment, even these cryptic
messages will be just as beautiful, if not more beautiful, as any warning box
you'll ever see.

Go ahead, type this into your terminal.

```
$ Where am I?
```

Again, probably a rude response.

```
-bash: Where: command not found
```

Great. We've established that our command line does not understand plain English.
We will have to use commands that our command line can understand. Let's try
this one.

```
$ pwd
```

Whoa! It looks like our computer understood that one! It replied with a message.

```
/Users/corneliusfinch
```
What did we just do?

> The command `pwd` stands for "Print Working Directory".
> This command is used when we want the command line to tell us what folder (or
> directory) of our computer we are currently in.

Just like Finder, your command line interface places you in a particular folder
of your computer. `pwd` tells you where you currently are. Usually, when you
open the Terminal application, you start off in your "home folder", which is one
with the same name as your username on your computer.

If we were using Finder, we'd be able to see what things (files and folders) are
present in this folder. In a CLI however, if we want to see what files and
folders exist at current location, we need to ask for it with another command.
Let's find out what's in this folder that we're in.

```
$ ls
```

Lo and behold, the contents of the folder you are in.

```
Applications       Desktop          Documents
Downloads          Library          Movies
Music              Pictures         Public
```

> The `ls` command, which loosely stands for "list", lists the contents of a
> folder.

It looks like there are some folders in here. Let's find out what's inside our
`Documents` folder. In order to do so, let's first navigate to the Documents
folder.

```
$ cd Documents
```

We have now navigated to the Documents folder.

> The `cd` command, which stands for "change directory", is used to navigate to
> a particular folder on your computer.

This is equivalent to double-clicking the Documents folder in Finder to "go
inside it". We can check that we're in the right place by using `pwd`.

```
$ pwd
/Users/corneliusfinch/Documents
```

Excellent! Now let's find out what's in here, using `ls`.

```
$ ls
funny_cat_picture.jpg
office_stuff
world_domination_checklist.txt
```

It looks like the `Documents` folder contains a JPG file of a funny cat, a folder
full of "office stuff", and a text file that supposedly contains a checklist for
world domination. Your `Documents` folder probably contains something different.

Now that we've investigated our `Documents` folder, let's go back up to our home
folder. Since the home folder contains the `Documents` folder, we can say that
the home folder is the "parent directory" of the `Documents` folder.

```
$ cd ..
```

> `..` (two periods, or "dot-dot") is how we say to our command line "parent
> directory".