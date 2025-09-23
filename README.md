# HAPAN_MGP_PA1

## Alphabet Soup Problem

**We need a function that takes a string and returns the letters in alphabetical order.**
- We need to convert the string into a list of letters so we can sort them.
- We use .sort() to arrange the letters alphabetically.
- We use a for loop to join the sorted letters back into a single string.
- Output: The function returns the given word with letters arranged alphabetically.

```Python
def alphabet_soup(word):
    letters = list(word)       # Convert the string into a list of characters
    letters.sort()             # Sort the letters alphabetically

    result = ""                # Create an empty string to store the result
    for als in letters:        # Loop through each letter in the sorted list
        result = result + als  # Add each letter to the result string

    return result              # Return the final alphabetized string

print(alphabet_soup("hello"))  # Output: 'ehllo'
print(alphabet_soup("hacker")) # Output: 'acehkr'
```

## Emoticon Problem 

**We need a function that converts certain keywords into emoticons.**
- We use .split() to break the sentence into words.
- We use if-elif-else to replace specific words with assigned emoticons.
- We use a loop to rebuild the sentence with updated words.
- Output: A sentence where words like "smile" or "mad" are replaced with their corresponding emoticons.

```Python
def emotify(sentence):
    words = sentence.split()           # Split the sentence into words

    for e in range(len(words)):        # Loop through each word
        if words[e] == "smile":        # Replace "smile" with :)
            words[e] = ":)"
        elif words[e] == "grin":       # Replace "grin" with :D
            words[e] = ":D"
        elif words[e] == "sad":        # Replace "sad" with :((
            words[e] = ":(("
        elif words[e] == "mad":        # Replace "mad" with >:(
            words[e] = ">:("

    result = " "                       # Rebuild the sentence with spaces
    for e in range(len(words)):
        if e == 0:
            result = words[e]
        else:
            result = result + " " + words[e]
            
    return result                      # Return the updated sentence

print(emotify("Make me smile"))        # Output: "Make me :)"
print(emotify("I am mad"))             # Output: "I am >:("
```

## Unpacking List Problem

**We need to unpack a list into three parts: first, middle, and last.**
- We use indexing to get the first and last elements.
- We use a for loop to collect all middle elements.
- We print the three parts separately.
- Output: Displays the first, middle, and last values from the list.
```Python
def unpacking_list(ulp):
    first = ulp[0]                 # Get the first element
    last = ulp[-1]                 # Get the last element
    middle = []                    # Initialize an empty list for middle elements

    for n in range(1, len(ulp)-1): # Loop from the 2nd element to the 2nd-to-last
        middle.append(ulp[n])      # Add each middle element to the list

    print("first:", first)         # Display the first element
    print("middle:", middle)       # Display all middle elements
    print("last:", last)           # Display the last element

unpacking_list([1,2,3,4,5,6])
```

VERSION 2
