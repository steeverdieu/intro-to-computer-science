## How Computers understand Informations 
The machine language is binary. Computers can only speak and understand ***0*** and ***1***. Any informations given to a computer, wheter it's a number, a text, an image, a video, a sound, an emoji or something else, has to be first translated into binary in order to be understood by the computer.

### How Computers understand Numbers
As computers only speak binary, to understand a number, this number has to be first converted into binary. Which is a set of ***1*** and ***0***.

For example, if you give the number **3** to a computer, this number is converted to ***1 1***, which is the binary equivalent of the number ***3***.

In a set of ***1*** and ***0***, each ***1*** or ***0*** is called a digit (precisely a ***binary digit***). In Computer Science jargon, a binary digit is called a ***bit***. For example :
- To convert the number ***3*** into binary, we need ***2 bits***  : ``3 -> 1 1`` *(A set of two **1**)*
- To convert the number ***4*** into binary, we need ***3 bits***  : ``4 -> 1 0 0`` *(A set of one **1** and two **0**)*
- To convert the number ***128*** into binary, we need ***8 bits*** : ``128 -> 1 0 0 0 0 0 0 0`` *(A set of one **1** and seven **0**)*

### How Computers understand Text
As you know now, a computer can only understand binary digits. Only set of ***0*** and ***1***. That means any letter given to a computer has to be converted into binary, so the computer can understand it.

Here is the process of how a letter is converted into binary :
1. A letter is given to a computer `The letter "A", for example`
2. This letter is first of all converted into a number `In the present case, the letter "A" is converted into the number "65"`
3. This number is converted into binary `The number "65" is converted into "0 1 0 0 0 0 0 1"`

#### But... Why ***A*** is converted to ***65*** ??
There is a standard mapping that sets a specific number to each letter of the Alphabet. This standard is called **ASCII**. It defines a numerical representation for both, Lower case and Upper case letters.

For capital letters, i.e from ***A*** to ***Z***, the numerical representation goes from ***65*** to ***90*** :
- The number that represents ***A*** is ***65***
- The number that represents ***B*** is ***66***
- The number that represents ***C*** is ***67***
- ...
- The number that represents ***Z*** is ***90***

For capital letters, i.e from ***a*** to ***z***, the numerical representation goes from ***97*** to ***122*** :
- The number that represents ***a*** is ***97***
- The number that represents ***b*** is ***98***
- The number that represents ***c*** is ***99***
- ...
- The number that represents ***z*** is ***122***

The ASCII standard has also the numbers that represent all the ponctuations. You can look at the entire ASCII Table [here](https://theasciicode.com.ar/). Unfortunately, this standard doesn't include numbers that represents special characters of orther languages, like the special character `é` in French.

### So how we represent those orther special characters
For this, we use another standard. This one is called ***Unicode***. It includes all the ASCII numbers, and in addition the numbers that represent the orther special characters. You can have a look at the ***Latin Unicode*** Table [here](https://www.ssec.wisc.edu/~tomw/java/unicode.html#x0080).

## How Computers understand Colors
Colors are commonly represented by a system called `RGB`. This system is a mix of three primary colors ***(Red, Green, Blue)***. In `RGB`, we have :
- `R` for `Red`
- `G` for `Green`
- `B` for `Blue`

To define a specific color by using the RGB system, we have to set an amount of red, an amount of green, and an amount of blue. The number that represent the amount of each color goes from ***0*** to ***255***.

For example, to represent the color `green yellow`, we have to write this RGB code:  `(173, 255, 47)`. This means that in `green yellow`, we have ***173 amount of Red, 255 amount Green, and 47 amount of blue***.

Because computers can only understand binary, when we give to a computer this formula `(173, 255, 47)`, each number is converted into a *8 digits* binary.
- `173` for the amount of Red becomes `10101101`
- `255` for the amount of Green becomes `11111111`
- `47` for the amount of Blue becomes `00101111`
Then after converting each numbers, they are all mixed together. So :
- `(173, 255, 47)` becomes a mix in binary of the amount of Red, Green and Blue :  `101011011111111100101111`
This is the process how computers understand colors.

## In a nutshell
- Computers can only understand binary. Anything you put in a computer, wheter it's a number, a text, a picture, a color, etc. It is converted into a bunch of ***0*** and ***1***. In other words, into binary.