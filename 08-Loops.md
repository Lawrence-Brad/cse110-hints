# Hints for the Loops assignment
## Word Guessing Game

### Using a loop to generate the initial hint
<details><summary>Hint #1</summary><p>

Use a loop to print one underscore for each letter.
For more guidance on generating hints refer back to the Team Activity for Week 8. NOTE: If the class has not completed the team activity yet, do not read through it until after the team activity has been completed.

</p></details>

### I'm confused about how to get the letter in the same position from both words

<details><summary>Hint #1</summary><p>
Remember that the index represents the position of a character in a string.

```python
word = "donut"

# You can access the first letter using the index of 0
# To do this, you use the string or variable containing a string followed by square brackets with the index inisde of it. Like:
print(word[0])          # Output: d

# You can also store that character in a separate variable if you would like
letter = word[0]
print(letter)           # Output: d
```

<details><summary>Hint #2</summary><p>

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

<details><summary>Hint #3</summary><p>

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

<details><summary>Hint #4</summary><p>

Because you are requiring the user's guess to have the same number of letters as the secret word, index in the loop above can be used to get the letter at the same position in both the guess and the secret word.

<details><summary>Hint #5</summary><p>

You don't need multiple for loops to make this work. One for loop using `for index in range(len(word)):` gets you the index. You will use that index inside this one for loop to retreive the letter for the guess, and use the same index again to get the letter from the secret word.

</p></details>
</p></details>
</p></details>
</p></details>
</p></details>

### Example from class for "a" or "an" based on the word provided.

<details><summary>See Example</summary><p>

```python
vowels = "aeiou"
noun = input("Please enter a noun? ")
article = 'a'
letter = noun[0]
print(noun[0])
if letter in vowels:
    article = "an"
print(f'You chose {article} {noun}')
```

</p></details>

### General Help

If you get stuck, it might be good to refer back to the preparation material for weeks 7 and 8 and consider which of those skills will help you accomplish the tasks for the assignment.

The prove activities also showcase important skills for these assignments. But be sure to wait until after the class has completed the team activity before reviewing it for help.
