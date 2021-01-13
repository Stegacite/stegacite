<!--
**Stegacite/stegacite** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile. -->

## Overview ##
"Stegacite" is a means to translate base64, such as would be used with a URL shortener, to English words.  
It is NOT a program and it is NOT a method of encryption or sending secret codes.  
Think of it as a CAPTCHA for social media moderators ... a means of "complying" with social media Terms and Conditions.

The goal is to make it possible to share information in a way that is complex, obscure, making sense to the human reader.
With a flexible syntax that can be explained in accompanying text, it should be more difficult for a machine to see what information
is being transmitted.  This should discourage internet tech companies from trying to block people from exchanging news sources.
If someone posts four words that sound odd on social media - maybe he is giving you a way to find something.  Who knows?

## Implementations ##
Any matrix should be usable by the "gold standard method": printing out the matrix PDF file and using it by hand.
This is not very difficult, and is meant to challenge any future effort to prevent people from running their own software.

An easier way to use a table like SOUTH Matrix is to open the spreadsheet file in LibreOffice and search for the words you need to find.

You CAN automate word matrix lookup - even I can write such programs - but these are only conveniences.  Stegacite is an idea,
not a program.

## Matrix tables ##
In the repository, the Matrix files are ways to translate base64 to other terms.  Each matrix is named after its encoding for the two letters "St".

### [SOUTH Matrix](https://github.com/Stegacite/stegacite/blob/main/SOUTH%20Matrix%20v0-2.pdf) ###
In this matrix the most common words because the first 14000 words in https://en.wiktionary.org/wiki/Wiktionary:Frequency_lists
for TV scripts were worked down into a 4-letter 12-bit lookup table.
As I used it the letter on top comes first and the letter on the side second for each pair.
The SOUTH Matrix used above is definitely not MEANT to be unique.  I've put it on the table in a spiral to avoid "lock-in"...
yes, there is a simpler way to arrange it with an uninspired alphabetical order - DO that if you want, or something else.

The word list in SOUTH Matrix was casually censored but not everything that might stand out to social media has been found.  
More revision is planned - ideally, the words should not stand out for scrutiny at an individual level or as randomly permuted,
but that is a complex manual process that can only go so far.

However, in SOUTH Matrix, every word in the table starts with a different four letters - ONLY those count.
So you could write _geeky passion hinkers unbelief_ in a posting, and the reader would still look up the first four letters only.

A [demonstration of SOUTH Matrix](https://github.com/Stegacite/stegacite/blob/main/SOUTH%20Matrix%20illustration%20v0-2.html) is provided 
to make it easier to get a feel for how this method works.  (That file is a standalone .html file - save it to your desktop 
and enable Javascript to try it out)

#### Sample use ####
The New York Post recently published an article that was banned from Facebook and Twitter.
People could not send this link to one another through their social media accounts.
I used TinyURL to translate the URL to an 8-digit base64 code ( y5zr43pm ).
Looking up y5, zr, 43, and pm on the SOUTH Matrix word table (PDF or Javascript), this translates this to _geek pass hinky unbelievable_.

#### Use your creativity! ####
For further obfuscation in a social context, you might say "Our team is up by 3 so far cups parole federal unauthorized".
In that case the last 4 words are down 3 from the real lookup, so if the reader goes up 3 he gets them.

The result from the 4 words is NOT actually a link - you'd have to assume it's on TinyURL because they're the first best known shortener.
Maybe you could put the word "tiny" somewhere in your post to make it ultra clear, or "bit" if it's bit.ly.
But this could also be used for plain text.

### [FEARING SYMPATHY Matrix](https://github.com/Stegacite/stegacite/blob/main/FEARING%20SYMPATHY%20Matrix.pdf) ###
The FEARING SYMPATHY Matrix is more peculiar.  It produces one word per character.  The matrix is based on the ancient Chinese Yi Jing system.
The Yi Jing is interesting in its own right, an "invention machine" that seeks to permit analysis of all possibilities from any given situation.
In the FEARING SYMPATHY matrix, each term is not a word to be used directly, but an idea to be referenced by a sentence, header, title, etc.
This means that a web link can be transmitted in a form that is independent of the use of any particular string, or even any particular language!

For example, the original New York Post tinyurl link is y5zr43pm - which can be looked up on the table as Crisis, Honesty, Politeness, Alienation,
The underground, Discretion, Punishment, The problem solver.  The link might be coded (sorry for the lack of inspired prose) as:
_Global warming is a problem.  Coal miners are good upstanding people.  They should be addressed with respect.  Some people just get disgusted with the climate situation and don't care about anything.  There is a network of opposition where people trade crazy ideas.  The government doesn't know how to handle them and is holding off action.  But there are things they could be charged with.  But there are methods for carbon sequestration that will set everything straight._
Sure, it's a bit of a loopy comment ... but what machine will recognize it as a WEB LINK? 

To produce the FEARING SYMPATHY Matrix, I went over the standard hexagrams to make some more mundanely comprehensible.  I was only able to do that
after first realizing that each of the six lines of a Yi Jing hexagram represents a desired condition in military science.  I realized that the lines,
from bottom to top, represent MASS (concentration of forces), bold ACTION, PRESERVATION of forces, KNOWLEDGE (intelligence, realistic assessment),
COORDINATION (command and control, communications), and SECURITY (privacy, stealth, withholding information from the enemy, perhaps with a touch of confidence
that information will not be used against one).  Given this understanding, the relationship and boundaries of the hexagrams became much clearer, at least in a
very "Yang"-heavy interpretation.  Perhaps these ideas would help to improve accuracy of recovery of information from this system - it is still experimental and
I can't say how well the information is preserved.  I have a little rat's nest of notes in a [LibreOffice spreadsheet](https://github.com/Stegacite/stegacite/blob/main/FEARING%20SYMPATHY%20Matrix%20with%20lengthy%20notes%20on%20derivation.ods) (it also works in Excel with some griping)

### [KC3 QB6 Matrix](https://github.com/Stegacite/stegacite/blob/main/KC3%20QF6%20Matrix.pdf) ###
This matrix can show up to 12 non-repeating charactes as a chess position.  A Wikipedia edit link is given which can be used to quickly 
make an image out of the position, or a text based description can be used
