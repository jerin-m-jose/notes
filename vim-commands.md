
# Vim commands 

### whole file

> copy file content to clipboard:   
> :%w !pbcopy   
> 
> To copy the current line, in command mode type:     
> "*yy    
> 
> To copy the whole file/buffer, in command mode,     
> first go to the beginning via gg, then type :   
> "*yG      

   
  
### for movement

> When using movement commands, you can put a number in front of them to make Vim complete a command multiple times.  
> For example, 5h will move your cursor five spaces to the left, and 90j will put your cursor at the beginning of the 90th line down from where your cursor currently is. 

- h - Moves the cursor to the left
- l - Moves the cursor to the right
- j - Moves the cursor down one line
- k - Moves the cursor up one line
- H - Puts the cursor at the top of the screen
- M - Puts the cursor in the middle of the screen
- L - Puts the cursor at the bottom of the screen
- w - Puts the cursor at the start of the next word
- b - Puts the cursor at the start of the previous word
- e - Puts the cursor at the end of a word
- 0 - Places the cursor at the beginning of a line
- $ - Places the cursor at the end of a line
- ) - Takes you to the start of the next sentence
- ( - Takes you to the start of the previous sentence
- } - Takes you to the start of the next paragraph or block of text
- { - Takes you to the start of the previous paragraph or block of text
- Ctrl + f - Takes you one page forward
- Ctrl + b - Takes you one page back
- gg - Places the cursor at the start of the file
- G - Places the cursor at the end of the file

***

### for editing

> Those who use Vim tend to use the term "yank" where most people would use the terms copy and paste.  
Therefore, the command for copying a word is yw, which stands for yank word, and the command for pasting whatever has been copied is p, meaning put.  
If you look up additional commands in the future, it can be confusing if you don't know what yank and put mean when using Vim.  
You also have two options for how to select text.   
You can either use commands like dd, which deletes a single line, and yy, which copies a single line, or you can highlight text and then copy it to the unnamed register.   
The paste commands work the same whether you've highlighted text or used a command to automatically copy it.  
As with movement commands, putting a number in front of the command can increase the number of times a task is completed.   
For instance, putting a number in front of yy will increase the number of lines copied, so 5yy will copy five lines.  
> 


- yy - Copies a line
- yw - Copies a word
- y$ - Copies from where your cursor is to the end of a line
- v - Highlight one character at a time using arrow buttons or the h, k, j, l buttons
- V - Highlights one line, and movement keys can allow you to highlight additional lines
- p - Paste whatever has been copied to the unnamed register
- d - Deletes highlighted text
- dd - Deletes a line of text
- dw - Deletes a word
- D - Deletes everything from where your cursor is to the end of the line
- d0 - Deletes everything from where your cursor is to the beginning of the line
- dgg - Deletes everything from where your cursor is to the beginning of the file
- dG - Deletes everything from where your cursor is to the end of the file
- x - Deletes a single character
- u - Undo the last operation; u# allows you to undo multiple actions
- Ctrl + r - Redo the last undo
- . - Repeats the last action

***

### for search

- /[keyword] - Searches for text in the document where keyword is whatever keyword, phrase or string of characters you're looking for
- ?[keyword] - Searches previous text for your keyword, phrase or character string
- n - Searches your text again in whatever direction your last search was
- N - Searches your text again in the opposite direction
- :%s/[pattern]/[replacement]/g - This replaces all occurrences of a pattern without confirming each one
- :%s/[pattern]/[replacement]/gc - Replaces all occurrences of a pattern and confirms each one

---
