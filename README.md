# WriteOn
## A.k.a. The Most Dangerous Vim Anti-Writer's-Block Script
A script you can add to your .vimrc that will clear the buffer (and the undo register) when you hesitate for too long while writing. Based on [The](https://www.squibler.io/dangerous-writing-prompt-app) excellent [Most Dangerous Writing App](https://www.squibler.io/dangerous-writing-prompt-app), which deserves all the credits for the concept. 

Once the script is added to your .vimrc, open a new, empty buffer, and enter the command `:WriteOn <sec> <min>` where `<sec>` is the number of seconds that you are allowed to hesitate before irretrievably losing what you just wrote, and `<min>` the number of minutes that you want this creative ordeal to go on.

Note that if you fail, i.e. you hesitate longer than you allowed yourself to, the buffer will be cleared *and* the undo register, too, so there is no turning back. Try again!

**Doing things in normal mode doesn't count as typing.** So don't jump around. Write now, and edit later.

**Saving is prohibited** and will trigger a 'failure' outcome. A file may seem to be written, but it is not. 

The script will refuse to run on a non-empty or named buffer.

When the session time has passed (whatever you set `<min>` to) you will be praised curtly, after which you may yank the contents of the buffer (`ggyG`) to use elsewhere.

This was competely vibe coded, in ten iterations or so, except for the echo messages, which I wrote myself. Usually vibe coding gets me nowhere, but this seems to work well, at least in MacVim (I didn't test it elsewhere, but you are welcome to).

**Use at your own risk. When you hesitate for too long, or try to write (save) the buffer, your work will be irretrievably lost.**

Let me repeat that.

**Use at your own risk. When you hesitate for too long, or try to write (save) the buffer, your work will be irretrievably lost.**

_Note that there is no need to type frantically, unless you set `<sec>` to something below 5 or so. Just keep writing. Think as you write (fuse thinking and writing into a single praxis). You will edit everything to near-perfection later. Welcome time passing like you would a fair wind in your sails: neither a feeble breeze nor a storm -- trust it to be just right. And stay the course, skipper!_
