# HAPAN_MGP_PA1

## Alphabet Soup Problem - Create a function that takes a string and returns a string with its letters in alphabetical order

//Sort the text
    
    def alphabet_soup(word):
    letters = list(word)
    letters.sort()
    
    result = " "
    for als in letters:
        result = result + als

    return result
    
//print text

    print(alphabet_soup("hello"))
    print(alphabet_soup("hacker"))

## Emoticon Problem - Create a function that changes specific words into emoticons.

    def emotify(sentence):
    words = sentence.split()

//Use if, elif, and else statement to align the word and emoticon

    for e in range(len(words)):
        if words[e] == "smile":
            words[e] = ":)"
        elif words[e] == "grin":
            words[e] = ":D"
        elif words[e] == "sad":
            words[e] = ":(("
        elif words[e] == "mad":
            words [e] = ">:("

    result = " "
    for e in range(len(words)):
        if e == 0:
            result = words[e]
        else:
            result = result + " " + words[e]
            
    return result

//Print given phrase which will result as word to the assigned emoticon

    print(emotify("Make me smile"))
    print(emotify("I am mad"))

## Unpacking List Problem - Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element.

//define the list

    def unpacking_list(ulp):
    first = ulp[0]
    last = ulp[-1]
    middle = []

    for n in range(1, len(ulp)-1):
        middle.append(ulp[n])

//Create automated phase then add the variable for printing

    print("first:", first)
    print("middle:", middle)
    print("last:", last)

    unpacking_list([1,2,3,4,5,6])
