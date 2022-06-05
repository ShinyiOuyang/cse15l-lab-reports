# Lab Report 5

## How I found Test Results

To find the tests with different results, I ran vimdiff on the result of running a bash for loop

[Here](https://github.com/ShinyiOuyang/markdown-parser/blob/main/test-files/201.md) is the link to test file 201.

[Here](https://github.com/ShinyiOuyang/markdown-parser/blob/main/test-files/41.md) is the link to test file 41.



# Test 1

For test 201, my implementation of markdown parser is correct while the provided implementation is wrong.
![difference1](lab5/vimDiff201.png)
![actual1](lab5/actual201.png)

## What is the cause of the bug?

The other implementation does not check the content in between the closing bracket and opening parantheses. The parser should not add the link if there is a <> in between.

![bug201](lab5/bug201OtherImplementation.png)

# Test 2

For test 41, my implementation of markdown parser is wrong, while the provided implementation is right.

![difference2](lab5/vimDiff41.png)
![actual2](lab5/actual41.png)

## What is the cause of the bug?

My implementation does not check the content of the links. My implementation should check for spaces in the link and not add the link if there is a space.

![bug41](lab5/bug41MyImplementation.png)


Thanks for reading!