# WriteOn
## A.k.a. The Most Dangerous Vim Anti-Writers-Block Script
A script you can add to your .vimrc that will clear the buffer (and the undo register) when you hesitate for a few seconds while writing. Based on the excellent Most Dangerous Writing App, which deserves all the credits for the concepts. 

When the script is in your .vimrc, open een new buffer, and enter the command `:WriteOn <sec> <min>` where <sec> is the number of seconds that you are allowed to hesitate before losing *all* of your buffer, and <min> the number of minutes that you want the ordeal to go on.

Note that when you fail (i.e. you hesitate longer than allowed) you lose the entire buffer content *and* the undo register is cleared, so you will have really lost your (lazy) work.

This was competely vibe coded, except for the echo messages. Usually vibe coding gets me nowehere, but in my experience, this script works fine, at least in MacVim (I didn't test it elsewhere).

**Use at your own risk. Always invoke only in a new buffer.**
