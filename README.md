# crosswordpuzzle
Simple crossword puzzle using a library to position the words and another to render it.

Refer to the open-source [Crossword Layout Generator library](https://github.com/MichaelWehar/Crossword-Layout-Generator/tree/master) for more details about generating Crossword Puzzle layout. Essentially, we need an input JSON and the library will output an output JSON and a grid in the form of a HTML string.
Note: Depending on whether the words are able to be fitted, the output JSON might not use all the words that are provided.

We then parse the HTML string to form an array which is fed into [jCrossword](https://github.com/trutex/jCrossword/tree/master) jQuery plugin. The plugin also requires an 2 input arrays (one for clues running across and another for clues running down). Both 'across' and 'down' clues need to be provided from top to bottom based on how they appear on the grid. By sorting and manipulating the output JSON, we can obtain these 2 arrays.
