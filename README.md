# wats1030-manipulating-text
An assignment based on editing text using command line text editors.

For this assignment, you must use three different text editors from the command
line of your Digital Ocean Droplet. (You should still have the Droplet from the
previous assignment. The instructions here will assume you are using an Ubuntu
14.04 server to complete this work.)

## Pre-Requirements

In order to complete the Basic Requirements below, you will need to verify that
all three editors are available to you. For this assignment you will need to
complete the basic requirements in each of the three editors.

### Nano
Nano is generally considered the easiest command line editor to use. There are
only a few commands available and it is based on the editor that was
included with the popular email software, Pine (which people used to use on
Unix servers to check their email).

To check for `nano`, try to run it:

`nano`

If `nano` is not there, you can install it by running:

`apt-get install nano`

--useful tips on nana for me
to open a new item or create a new writing type - " nano + path and file name you want to create and edit"

-sudo ( gives you permission to Write on the file )
--sudo !! copies prevoius input so as shortcut for previous path and give you permission 

- nano my-file -- creates new blank file 

-- Helpful shortcuts working on *** command LINE **

 the Meta key, displayed as M; or the Escape (Esc) key.

 
Ctrl + a ( beginning on line )  OR Ctrl + e ( End of line )

escape + space bar ( moves BACK by word)

Ctrl + space bar   ( moves FORWARD by word )

escape + shift + m = mouse enable 

escape + i = ( auto indentation ) 
 
ctrl + shift + underscore (-) = ( jump to line ) 
--OR ctrl + /

if you enter : 2, 10   = ( line 2, columen 10)

Ctrl + m + c =  current line & column position 


Ctrl + home = top of file

Ctrl + end = bottom of file 

Ctrl + k =  Cut 

Ctrl + u = paste 

--Ctrl + 6 = copy ( Mark Set)

then highlight what you want to copy 

then escape + 6 == to COPY

and paste is still Ctrl + u---


Escape + r  == Find and Replace 

Ctrl + w = Search   

--- *note in search you can do Ctrl + r and do search and replace .....

Ctrl + o = Save AS or append 

Ctrl + t = files category 

---------------------------

Ctrl + r == Open File 

escape + f = add new buffer ( for using more than 1 files at the same time )

---- you can just press "enter key" to just open a new buffer 

escape + , = left buffer switch 

escape + . = right buffer switch 

ctrl + z - suspension ( to work on COMMAND LINE AGAIN)

fg = returns back 

escape + u = undo


### Emacs
Emacs was created with an eye towards "editor macros" (hence the name), and it
remains strong with many macros available to tie emacs in to all sorts of
systems and processes. It is a very flexible editor, with an idiosyncratic
interface that is not like any other application.

To check for `emacs`, try to run it:

`emacs`

If `emacs` is not there, you can install it by running:

`apt-get install emacs`

### Vi
Vi is a "mode-based" editor, meaning that it starts looking at files in "view"
mode and you must switch into "interactive" mode to edit them. Vi is also designed
to keep your fingers on the home row as much as possible, and fans of Vi love
that they can use all sorts of keyboard shortcuts to navigate precisely within
files. Like Emacs, Vi is not at all like any other text editor you've probably
used.

Vi should be included in your system already, but you can check for it and
install it just like the other packages. Check for it by trying to run it:

`vi`

If `vi` does not work, then install it:

`apt-get install vi`

------------------------------------------------------------------------
shortcuts 

 shift + zz =write + exits file 
 
:wq then enter  = write + exit file

:q! OR :q then enter =  exits file 

:w + name of new file == Save AS different name.....

----------------------------------------------

COMMAND MODE 

k = move up 

j = move down 

l = move right 

h = move left

space bar = move right 

backspace = right 

- = start of line 

[Number + movement ]

Ex:  10 + l = move right by 10


i = Inster MODE

escape = leave insert mode 

-------------------------------------------------
moving by words / sentences / paragraphs 

w = forward a word 

b = backward a word 

e = forward to end of current word 

( = back a sentence 

) = forward a sentence 

} = forward a paragraph 

{ = backward a paragraph 

-------------------------------------------------
moving by lines 

^ = beginning of line

$ = end of line 

1G = first line of file  ( 1 + Shift + g )

     #G any line you choose 
     
G = lst line of fie  ( Shfit + g )

% = jump between brackets []  or ()

-------------------------------------------------------

PROMPT MODE 

escape twice terminates command 

:w = write without quitting  ( save as of DIFF FILE NAME )

:vi = edit another file 

:n = go to next file 

:n! force into next file without saving 

:N = go to previous file 

:r = read file into the THIS ONE

ctrl + g = line # and file #

------------------------------------------
scrolling 

Ctrl + e = scroll down line 

Ctrl + y = scroll up line

Ctrl + d = scroll down half screen 

Ctrl + u = scroll up half screen

Ctrl + f = scroll down full screen

Ctrl + b = scroll up Full screen 

------------------------------------------------
Insert Text 

i = insert cursor 

I = insert at beginning of lin e

a = append after cursor 

A = append at end of line 

o = open a new line below 

O = open a new line above

escape = exit insert mode 

---------------------------------------------
Deleting text 

x = delete character 

dd = curent line 

dw = current word 

de = to end fo word 

d^ = beginning of line 

d$ = to end of line

d + any command deltes certain line word area

------------------------------------------------
changing text 

r = current character but in command mode 

s = replace current character but in insert mode 

cc = delets current line and goes into insert mode 

cw = current word 

c^ = change to beginning of line 

c$ = change to end of line 

C = change current area to end of line 

---------------------------------------------------
u = undo command ( if you repeat u continues to undo previous command )

Ctrl + r = redos last change ( undo the u command )

U =  undoes all changes to current line 

. = repeats last change 


-----------------------------------------------------

Delete yank put 

dd = delete line ( cut)

yy = yank (copy ) line 

yw = yank word 

y( = 

y) = 

yd = yank line ?

3yy = py three lines 

p = put  below( paste) after cursor

P = put above ( paste ) before cursor

-------------------------------------------------------
Searching 

/ + text = search Forward  for text 

? + text =  search Backward for text

n = repeat previous search 

N = repeat prevous search in opposite direction 

/[.] =  search for anything with brackets 

/^ = search for at beginning of line 

/$ = search for at end of line 

/se*m = search for any word with sm + any number of e

---------------------------------------------------------------

Search and REPLACE 

:s/ old / new / replace old with new 

:s/ old / new /g = replace every old with new on CURRENT LINE

:%s/ old / new / = replaces FIRST old with new on every line 

:%s/ gold / new /g = replace ALL gold with new on EVERY LINE 


--------------------------------------------------------


## Basic Requirements
Once you have all of your editors available on your Droplet, you can begin
working on the tasks outlined below. There are three directories in this repo:

```
emacs/
nano/
vi/
```

You will work through this set of tasks in each of the three directories,
allowing you to experience the differences between these three editors. Files
have been copied into each directory already, so you have fresh files to work
with in each directory. As you work through the tasks, be sure you are editing
files in the correct directory.

* Create a new file called `unix_philosophy.txt` and type in the text from the
`unix_philosophy.pdf` file.

* Open the file `power_of_unix.html` and remove all of the HTML tags. Save the
file with a new filename: `power_of_unix.txt`. (Hint: You can zap those pesky
comments with a "delete line" command in some editors...)

* Open the file `gancarz_unix_philosophy.txt` and correct the typos of
`beautiflu` and `effishingly`. Save and close the file when you're done.

* Open the file `17_rules.txt` and remove all of the bracketed footnote numbers
left over from the copy/paste of text. (The footnote numbers look like this:
`[12]`. They are sprinkled throughout the file. You could probably use some
kind of search or find function to get them all...)

* Update `example.httpd.conf` to have the following settings:

```
<VirtualHost *:80>
DocumentRoot /www/unix
ServerName www.unix.com
</VirtualHost>

<VirtualHost *:80>
DocumentRoot /www/linux
ServerName www.unix.org
</VirtualHost>
```

* In the short story "The Machine Stops" (contained in the
`the_machine_stops.txt` file), the main characters are Vishta and Kuno. How many
times does the word "Vishta" show up in the short story? How many times does the
word "Kuno" show up in the short story? Add your word frequency counts to the `wordFrequency.json`
in each of the working directories. (Be sure to count the unique `the_machine_stops.txt` file in 
EACH directory -- they are not the same!) 2 , 

* Create a file in the root of this repository (the same level as this `README.md` file) called 
`favorite.md` and write a statement about which editor you prefer. Be sure to discuss what you like
and dislike about the editor, and give some sense of your evaluation compared to the other text
editors you've tried in this project. (Obviously, you should use your favorite editor to create,
edit, and save this file. Please also feel free to use Markdown formatting and links to enhance
your text.)

## Stretch Goals

* Play Tetris in Emacs. Add a screenshot of you playing Tetris in Emacs to this repository (possibly using SCP to transfer the file, or uploading the file in another way).
* How do you turn on line numbering in Vi? Emacs? (Type your answer here.)
* Explore the Emacs file browser mode. Describe how it works here.
