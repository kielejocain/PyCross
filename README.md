PyCross
=======

Description
-----------

This is a quick script that can be used to solve many simple puzzles
known by many names; nongrams, picross, oekaki, japanese crosswords, etc.
For a further description, see the [wikipedia article](http://en.wikipedia.org/wiki/Nonogram).  For a collection of puzzles to test or solve, see [puzzle-nonograms.com](http://www.puzzle-nonograms.com/).

Requirements
------------

The script runs in base Python 2.7.  I may eventually try to get it to run    
in 3+ as well, but that is low priority for me.

Usage
-----

Upon running the script, you will first be asked to imput the number of rows and columns.
You will then be asked to enter each row and each column.  We'll use the example puzzle
on the wikipedia page as a demonstration.

                          1 1
                          1 1   3   3
                      3 2 1 3 2 3 5 1 2 3   2 2
                1 2 2 1 1 2 1 6 9 3 2 1 3 2 1 2 2
              2 2 3 3 1 1 2 3 4 1 2 2 7 2 4 2 1 2 1 1
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
            3| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
            5| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          3 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          2 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        3 3 4| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        2 2 7| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        6 1 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        4 2 2| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          1 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          3 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
            6| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          2 7| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        6 3 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
    1 2 2 1 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
      4 1 1 3| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        4 2 2| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
        3 3 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          3 3| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
            3| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
          2 1| | | | | | | | | | | | | | | | | | | | |
             +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

As this puzzle is 20x20, you would enter 20 for the rows and 20 for the columns.  When asked for the rows, you would enter `3`, then `5`, then `3,1`, and so on.  For the columns, you would enter `2`, then `1,2`, then `2,3`, and so on.

Once all rows and columns have been computed, the script will work to solve the puzzle until it has finished or it cannot make further progress.  It will output the grid periodically and at the end.
