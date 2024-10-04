# SWAG LaTeX Template
Template in LaTeX for SWAG content. It's not as accurate as the inDesign template, but it's free :)

For the purpose of copyright/fair use/etc., consider anything that might be "mine" to be public domain. The specifications of the layout and the art all belong to Pinnacle. Refer to their site for information here: https://peginc.com/swag-savage-worlds-adventurers-guild/

# How to Use

You will need to either get a LaTeX editor or use an online one like Overleaf (free if you're a student). If you use an online editor, SAVE YOUR TEXT SOMEWHERE ELSE FIRST! It can be a google doc, a back of a napkin, whatever. 

I use TeXWorks, but it doesn't really matter as long as it can compile LaTeX as LuaLaTex.

Then, download the swag_template.tex file and the images folder. You will also have to find SWAG_logo.png from DTRPG or Pinnacle's website and place it in the folder. You may need the fonts in this repository as well: otherwise, they are in Pinnacle's indesign template on DTRPG.

Then, open up the swag_template file in your LaTeX editor. Make sure you are compiling using LuaLaTex (TeXStudio defaults to PDFLaTeX) and compile this to test your setup.

Finally, you can start switching out the Lorem Ipsum text and headers with your own content.

# Macros

I have a few macros set up to make things easier:

    {\noind 
    A paragraph of text. 
    }

The \noind macro just removes an indentation from a paragraph. By default, LaTeX indents all paragraphs.

    \bighdr{INTRODUCTION}
 
 The \bighdr macro creates the large red headers
 
    \medhdr[SMALL HEADER]
    \smlhdr[SMALLER HEADER]
 
The \medhdr and \smlhdr macros create the other headers. \medhdr is the underlined one (with the horizontal rule). Note that these place the text in square brackets [] instead of curly brackets {} like \bighdr.

There are a few other macros I use (\desc stores description of the document, \myfont makes text Fira Sans, etc.) but these are the main ones you should know.

# Other

If you want rounded tables as well, please see pan-mroku's fork here: https://github.com/pan-mroku/swag-latex-template/tree/feature/table_annotations
And if you're able to fix the header-squash issue, definitely feel free to contribute!
