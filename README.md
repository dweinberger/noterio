Note: This is a version of the about.html page.

It is important to recognize that I am a hobbyist who writes _embarrassing_ code. I am doing the best I can.

_David Weinberger_
self@evident.com

# Noter.io

## Type your research notes into The Cloud

### What is Noter.io? 

Noter.io is a prototype of a service for researchers who take notes on what they read. Upload your notes to Noter.io and they'll be turned into a database that Noterio lets you sort, cluster, filter, and make sense of. 

### Prototype? 

Yes. That's an important weasel word. Noterio was written by a non-developer at the Harvard Library Innovation Lab initially for his own use. I am an amateur. The actual developers at the Library Innovation Lab are highly skilled professionals who do rock solid work. I am not and do the opposite of that. So, we put this forward as an example of what might be a useful service. Don't invest too heavily in it. On the other hand, because it requires that notes be taken using a simple text editor, and since those notes are perfectly humanly readable, at the very worst you'll end up with a well-ordered set of notes. Could be worse. 

### How about a list of features? 

Good idea! Here's what you can do: 

  * Create notes by using any editor that creates plain text, using a dead simple syntax
  * Create a project
  * Batch upload notes for that project
  * See a sortable list of all the books, articles, etc., for which you've uploaded notes
  * That resource list is viewable as a table, or as a graphical representation of a stack of books
  * See and edit the bibliographic information for each uploaded resource file 
  * Click on a resource to see a sortable list of notes
  * Rate and tag resources
  * Edit notes in place
  * Create a scratchpad of notes (including their bibliographic info) that can be copied and pasted or exported as an RTF file that can be read by any word processor
  * Organize notes by dragging them into topic boxes
  * Search all notes within or across projects by tag or full text
  * See a tag cloud of all the tags you've used within or across projects
  * Generate (poorly) formatted bibliographies from the bibliographic information in your note files

### How do I create notes in the first place? 

So, there is a little catch. Noterio expects you to use a plain old text editor to take your notes. And you have to use a little bit of syntax so that Noterio can make sense of what your notes mean. 

### So, no Word, Pages, or LibreOffice? 

You can use them so long as you save the files as plain old text files. So you might as well use something lighter weight, like BBEdit or TextWrangler for a Mac, or UltraEdit on a PC. Any text editor will do. 

### What's this syntax you keep talking about? 

A Noterio notes file has two parts: A bibliographic section that contains the normal sort of bibliographic data, and a notes section that consists of your notes on that work. 

The bibliographic section is a list of self-explanatory keywords followed by an equals sign. You'll want to create a template of this section. You can get one [here][1], or you can copy and paste the following: 
    
    :: BIBLIO
    
    TITLE= 
    AUTHOR= 
    PUB= 
    DATE= 
    CITY= 
    MISC=
    TAGS= 
    JOURNAL=
    VOL=
    ISSUE=
    PAGES=
    TRANSLATOR= 
    TYPE= 
    CONTAINER= 
    NICKNAME=
    URL=
    NOTE=
    ISBN=
    
    :: NOTES
    

Some explanation: 

  * All of these are free-text fields. Type in whatever will be useful to you.
  * TITLE is a required field.
  * TYPE is intended for you to indicate what type of medium it is, but can be used for any information you want to record.
  * CONTAINER is a place for you to indicate if the resource you're taking notes on is part of a larger entity, such as an article in an anthology. The container would be the anthology.
  * NICKNAME is a shorthand way to refer to the current resource. If you're taking notes on an article in an anthology, you might want to create a note file for the anthology itself, and give it a short nickname. You would then create a note file for each article in the anthology, and in the CONTAINER field type the nickname of the anthology. For example, if the anthology is _1968's Best Science Fiction_, you might create a note page for the anthology and called it "Best68" in the Nickname field. Then, for each story you're taking notes on, you'd put "Best68" in as the container.

Please note that the ":: BIB" and ":: NOTES" are required so that Noterio can tell where one begins and the other ends.

### How about the syntax for taking notes? 

Simple. After the ":: NOTES" marker, you create a note as follows:

> 15-16/ This is a note >> example, sample

The characters before the / are taken as page numbers. You can use whatever sort of notation you like; it's all just text to Noterio. You get 12 characters before the /; after that the slash is taken as part of the note. 

After the slash, you type whatever you want as your note. (If you want to indicate italics or bold, consider wrapping the words with an underscore an asterisk, you can use HTML markup.) 

If you want to tag a note, end with >> and separate the tags with commas. Using tags will let you cluster notes more efficiently in Noterio. 

If you want to apply the same tags to a consecutive string of notes -- let's say you're in the portion of an article that bears on "Pluto" and "planets" -- if you begin a line with ">>" and then tags separated by commas, Noterio will apply them to all subsequent notes until it encounters another ">>" at the beginning of a line. You can also attach unique tags to notes that are being automatically tagged; those notes will have both sets of tags. 

For example: 

> >> Pluto, planets  
  
15/Pluto was discovered in 1930 >> history

will create a note that is tagged with Pluto, planet, and history. To stop using one of those continuing tags, begin a line with ">>" and either leave the rest blank, or put in a new tag. 

### May I have a template, please? 

Sure: [Template][2]. In fact, have a [sample][3], too.

### Can I edit the notes I've imported from my text files? 

Yes. Double click on a note and you will be put into edit mode. Edits are automatically saved. The buttons at the bottom of the notes display table also let you delete notes and batch edit tags. 

Note also that the tags displayed to the right of the notes are hyperlinked. Clicking on one will show all notes with that tag. 

Clicking on the table headings sorts the table. 

### What are topic boxes? 

They're boxes full of notes. You'll find them toward the bottom of the page. Click on the "new" button to create a new one. Give it a title and click outside of the text box in order to create a new topic box. Drag in notes from the notes display table (i.e., the table where your notes are displayed). Drag from within the note itself. You can also drag notes from topic box to topic box. Noterio won't let you drag a note into a topic box that already contains that note. 

The symbols at the top of a topic box let you delete it, shrink or expand it, or show or hide the bibliographic data. Hover over the symbols to get a reminder of what they do. 

### What's the difference between a topic box and the scratch pad? 

Topic boxes are saved across sessions. The scratch pad is a place for you to assemble a set of notes and then copy them into your word processor. You can also save the contents of a scratch pad as an RTF file or display it as HTML. 

### Why does the bibliography that Noterio creates suck so bad? 

Because it's hard to do well and I'm a lazy sod. 

### Can I import from Zotero? 

I had this working at one point. If this matters to you, let me know. Cf. "lazy sod" in the index of this page. 

### Suppose I have a problem with Noterio, or an idea for an improvement? 

Let me know: self@evident.com 

   [1]: 
   [2]: noterio_template.txt
   [3]: noterio_sample.txt
   
## License

Dual licensed under the MIT license (below) and [GPL license](http://www.gnu.org/licenses/gpl-3.0.html).

MIT License

Copyright (c) 2013 David Weinberger

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

