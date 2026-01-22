# WriteOn
## A.k.a. The Most Dangerous Vim Anti-Writer's-Block Script
A script you can add to your .vimrc that will clear the buffer (and the undo register) when you hesitate for a few seconds while writing. Based on [The](https://www.squibler.io/dangerous-writing-prompt-app) excellent [Most Dangerous Writing App](https://www.squibler.io/dangerous-writing-prompt-app), which deserves all the credits for the concept. 

When the script is in your .vimrc, open a new buffer, and enter the command `:WriteOn <sec> <min>` where `<sec>` is the number of seconds that you are allowed to hesitate before losing *all* of your buffer, and `<min>` the number of minutes that you want this creative ordeal to go on.

Note that when you fail (i.e. you hesitate longer than you allowed yourself to) you lose the entire buffer content *and* the undo register is cleared, so you will have really lost your work. 

Doing things in normal mode doesn't count as typing.

Note that there really is no need to type *frantically*, unless you set `<sec>` to something below 10 or so. Just keep writing. You can edit later. Try to feel the pressure like wind in your sails. 

When the session time has passed (whatever you picked for `<min>`) you will be praised, and can proceed to yank the contents of the buffer (`ggyG`), to use elsewhere.

This was competely vibe coded, except for the echo messages. Usually vibe coding gets me nowehere, but this seems to work fine, at least in MacVim (I didn't test it elsewhere, but you are welcome to).

**Use at your own risk. Always invoke only in a new buffer.**

Let me repeat that.

**Use at your own risk. Always invoke only in a new buffer.**

And let me once more point out that... **when you hesitate for too long, the contents of your buffer will be irretrievably lost.**
