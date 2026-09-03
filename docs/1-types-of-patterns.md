# Initial thoughts
In this file you can observe how I started thinking about this.

## Writing Style (read before you continue)
I use X to represent "don't care" if I am trying to show a pattern.
So these Xs can get different values.

## Note (read before you continue)
The docs are numbered as created.
I think this helps these being more clear and being able to be used as a tutorial as well

## What is compression?
Representing data in a concise way (without loss of data), avoiding repetition of a pattern.

## Types of patterns and repetitions:

### Gapless pattern:
Something just keeps on repeting.
e.g: 123123123123

### Fixed-gap pattern:
Something keeps on repeting, but there are fixed-size gap of data between each subsequent repetition that doesn't repeat.
e.g:123451238912301 (pattern: 123XX123XX123XX)

### Unfixed-gap repetition:
There are unfixed-size gaps between two subsequent repetition.
e.g: 12345whc12345sfdh12345sflksdfjj (pattern: 12345 repeats with unfixed-size gaps between each two subsequent repetition)

### Complicated unfixed-gap repetition:
An unfixed gap repetition with each block being a fixed/unfixed-gap pattern.

#### Examples:

+ Each block being a unfixed-gap repetition: 123123123XX123123123XXXX123123123XXXXX
+ Each block being an fixed-gap repetition: 123123123XX123123123XX

### Computational pattern:
There is a relation between the numbers (or objects/beings/etc) that is not a mere repetition.
There are no gaps.
I haven't really thought much about it since I am not going to compress these types of patterns in my algorithm; not yet at least.

### Others
Everything else!
Others do exist (a mix of a computational pattern and unfixed-gap repetition for instance).
I have already so much to do in my algorithm.
I may think of these later.
Obviously, these are not going to be compressed in our algorithm.

## Looking Back
As you see, I can't do anything with truly redundant data, since I don't know what is redundant and what isn't.
