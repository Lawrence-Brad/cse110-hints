# Hints for the Loops assignment
## Word Guessing Game

<details><summary>I'm confused about how to get the letter in the same position from both words</summary>

Remember that the index represents the position of a character in a string.
<details><summary>Hint #1</summary>

```python
word = "donut"

# You can access the first letter using the index of 0
# To do this, you use the string or variable containing a string followed by square brackets with the index inisde of it. Like:
print(word[0])          # Output: d

# You can also store that character in a separate variable if you would like
letter = word[0]
print(letter)           # Output: d
```

<details><summary>Hint #2</summary>

The index doesn't have to be specified, it can be in a variable

```python
index = 0
word = "donut"
letter = word[index]
print(letter)           # Output: d

# The word "example" has 5 letters in it. We can discover the number of letters using the len function
length = len(word)
print(f'{word} has {length} letters')

# Because the index starts counting at 0, to get the last letter we use the index of 4
last_letter = word[4]
print(last_letter)      # Output: t

# Note that if you try to access the letter at position 5, the code will throw an error.
# last_letter = word[5] will throw an index out of range error.
```

<details><summary>Hint #3</summary>

```python
# Use the range function together with a for loop to access the index of each letter in a word

# If you don't remember the range function review the preparation material for week 8

# When you give the range function one parameter, then it will count up from 0 to the number before the number provided. So we can use the len function to get the right number of letters in the word.

# Put them all together and each letter will be printed on a separate line.
word = "donut"
for index in range(len(word)):
    letter = word[index]
    print(letter)
```

<details><summary>Hint #4</summary>

Because you are requiring the user's guess to have the same number of letters as the secret word, index in the loop above can be used to get the letter at the same position in both the guess and the secret word.

</details>
</details>
</details>
</details>
</details>
