# HAPAN_MGP_PA1

##Alphabet Soup Problem
def alphabet_soup(word):
    letters = list(word)
    letters.sort()
    
    result = " "
    for als in letters:
        result = result + als

    return result

print(alphabet_soup("hello"))
print(alphabet_soup("hacker"))

##Emoticon Problem
def emotify(sentence):
    words = sentence.split()

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

print(emotify("Make me smile"))
print(emotify("I am mad"))

##Unpacking List Problem

