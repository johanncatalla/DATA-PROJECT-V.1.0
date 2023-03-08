# Project Description

A simple text editor using Tkinter utilizing Object-Oriented Programming (OOP) that lets the user create a new file (CREATE), open (READ), save (UPDATE), and delete (DELETE) files. The program also has a search functionality (REGEX) that matches input word/s to a sentence.  

![text editor](.docu/2.jpg)

# Project Details 

The program uses the Tkinter, filedialog, messagebox, regex, and os modules. The class includes the root container, which contains the menus and the three frames:
    The top frame at the top;
    The buttons frame in the middle and;
    The display frame at the bottom.

The top frame contains the main text editor with a scrollbar, which lets the user open, create, save, and delete a file. The text editor is also bound to certain keypress events which are:
    "CTRL+O" for opening a file;
    "CTRL+N" for creating a new file;
    "CTRL+S" for saving and;
    "CTRL+D" for deleting. 
    
The middle frame contains the buttons and functionalities, namely, the open file shortcut button, search bar and search button, case-sensitive or case-insensitive options for search, and clear search results button.

The display frame contains the text editor with a scrollbar for displaying search outputs and the export searches button, which saves the results in the desired directory. 

Furthermore, the menu bar in the root container has three menus: the File menu, the Action menu, and the Edit menu. The file menu has five options, namely, "Open File...", "New Text File," "Save," "Save as...," and "Delete File." The action menu only has one option: "close window." Lastly, the edit menu has three actions, namely, "Cut," "Copy," and "Paste."

The search functionality has the following properties:
    It can be case-sensitive or case-insensitive;
    Multiple Words in the search bar are considered separate.;
    The keywords are matched to the sentences that contain them, regardless of the keyword's position in the sentence.;
    Statements with new lines separating them and having no punctuation are considered one sentence.;
    It does not match words with prefixes or suffixes that are digits or alphabets.;
    It matches words with prefixes or suffixes that are special characters or punctuations.;
    The search function returns the following to the text editor in the display frame:
        the number of sentences matches,
        the number of matches per keyword in the text and,
        the sentence matches.
