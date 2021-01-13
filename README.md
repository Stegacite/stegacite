<!--
**Stegacite/stegacite** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile. -->

## Overview ##
"Stegacite" is a means to translate base64, such as would be used with a URL shortener, to English words.  
It is NOT a program and it is NOT a method of encryption or sending secret codes.  
Think of it as a CAPTCHA for social media moderators ... a means of "complying" with social media Terms and Conditions.

## Basic usage ##
For example, the New York Post recently published an article that was banned from Facebook and Twitter.
People could not send this link because the companies didn't like it and reinterpreted their policies.
TinyURL was able to translate the URL to an 8-digit base64 code ( y5zr43pm ) for me just now.
Looking up y5, zr, 43, and pm on a word table (SOUTH Matrix) translates this to _geek pass hinky unbelievable_.

## Matrix tables ##
In the repository, the Matrix files are ways to translate base64 to other terms.  Each matrix is named after its encoding for the two letters "St".

### [SOUTH Matrix](https://github.com/Stegacite/stegacite/blob/main/SOUTH%20Matrix%20v0-2.pdf) ###
The SOUTH Matrix used above is definitely not MEANT to be unique.  I've put it on the table in a spiral to avoid "lock-in"...
yes, there is a simpler way to arrange it with an uninspired alphabetical order - DO that if you want, or something else.

The word list in SOUTH Matrix was casually censored but not everything that might stand out to social media has been found.
Remember you can change any part of the word after the first 4 letters!  But more revision is needed.  There are MANY unused words.

The list is heavy on the most common words because the first 14000 words in https://en.wiktionary.org/wiki/Wiktionary:Frequency_lists
for TV scripts were used.  These were heavily revised, with most proper names removed and only one word with a given first 4 letters
can be used in the table.

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
This matrix can show up to 12 non-repeating charactes as a chess position.  A Wikipedia edit link is given which can be used to quickly make an image out of the position, or a text based description can be used.

## Advanced social usages ##
In SOUTH Matrix, every word in the table starts with a different four letters - ONLY those count.
So you could write _geeky passion hinkers unbelief_ in a posting, and the reader would still look up the first four letters only.

Will social media ban posts of those four words?  It's conceivable.
But then you can say "Our team is up by 3 so far cups parole federal unauthorized".
In that case the last 4 words are down 3 from the real lookup, so if the reader goes up 3 he gets them.

The result from the 4 words is NOT actually a link - you'd have to assume it's on TinyURL because they're the first best known shortener.
Maybe you could put the word "tiny" somewhere in your post to make it ultra clear, or "bit" if it's bit.ly.
The goal is to make it possible to share information in a way that is complex, obscure, making sense to the human reader.
The social media thinks a bad post is a billion times more bad than a good post is good, and they want a machine
that can read a billion posts they don't think are worth reading.  Can they do that if people share links like this?
If someone posts four words that sound odd on social media - maybe he is giving you a way to find a source.  Who knows?

## Alternate information sources ##
Stegacite is meant to be a broad idea for a language that evolves and changes as need be to help people stay out of trouble.
The scheme can be modified to send whole bytes by capitalizing or otherwise marking the first 4 letters to share 4 extra bits
(two letters of base64 = 12 bits, two bytes = 16 bits).  This is less subtle but you can send an IP4 address as 2 words.
Using raw IP or unique tags that can be searched for is a means to make do when the link shorteners are closed down.

Stegacite can also be used to transmit nucleotide sequences - for each nucleotide there are four possibilities, so a three-nucleotide CDS codon can
be turned into a single base64 letter and back again, and the table used normally.  This is perhaps best represented as a matrix file; that file can also
be used to translate web addresses to nucleotide sequence (Todo - this is very simple)

## Implementations ##
The "gold standard method" is printing out the matrix PDF file and using it by hand.  This can be done easily, and it can be done even if the company that owns
your computer, which in exchange for your cash offers you a license to use it under certain conditions, decides to stop accepting software unless they approve it.

An easier way to use a table like SOUTH Matrix is to open it in LibreOffice and search for the words you need to find.
As I used it the letter on top comes first and the letter on the side second for each pair.

You CAN automate word matrix lookup - even I can write this as a tiny program - but I want it to be extremely clear that this is an IDEA, not a PROGRAM.
A [demonstration of SOUTH Matrix](https://github.com/Stegacite/stegacite/blob/main/SOUTH%20Matrix%20illustration%20v0-2.html) is provided to make it easier to get a feel
for how this method works.  (That file is an .html file - you can save it to your desktop and enable Javascript to try it out)
