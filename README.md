# Machine_Learning
Set of files in which I use machine learning algorithms 

 ## 1.  SUDOKU GENERATION PLUS MACHINE LEARNING TEST

    In this notebook, my aim is to use Machine Learning algorithms to distinguish if a given matrix of numbers is, or not, 
    a sudoku. For doing that, I divide the notebook into two sections:

    1.The first section is devoted to the creation of a database of sudokus and non-sudokus with their respective labels 
      for future Machine Learning algorithms.

    2. In the second section, I will use some Machine Learning algorithms for trying to predict the "sudokuness" of a table 
        of numbers.
        
        1. Firstly with a Decision tree, and later, Random forest classifiers. They seem natural to me in the process of 
        creating rules for classification of sudokus.
        
        2. Secondly, I use an MLP neural network with one hidden layer. I believe this should be enough for my purpose.

    Sudokus are not the typical example when someone wants to use Machine Learning models (as far as I know) but they have 
    special characteristics that made me think this could be a cool example.

    There are deterministic rules to distinguish a sudoku from a non-sudoku. Could a Machine Learning algorithm learn the 
    rules we are all thinking or would find some other ways?

    Sudokus has a nice structure that make them invariant whenever swapping elements. For example, if in a sudoku one 
    permutes all 1's by 2' and vice-versa, one finds another sudoku. Furthermore, one could imagine (as it was my case 
    before checking my results) that whenever one has a sudoku, for being "fair" with the model, one should feed it with 
    all possible permutations so that it can "understand" that the actual numbers appearing are not important, but the structure 
    behind (a sudoku could be made by nine different symbols without any mathematical intrinsic meaning). The total number of 
    new sudokus one obtain permuting elements from just one sudoku is $9! = 362.880$ . Which is quite a big number for just 
    one "real sudoku". How would a Machine Learning model distinguish between sudoku and non-sudoku if one does not use 
    billions of training examples?

