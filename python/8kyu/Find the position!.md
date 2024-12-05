When provided with a letter, return its position in the alphabet.

Input :: "a"

Output :: "Position of alphabet: 1"

Note: Only lowercased English letters are tested

```
def position_in_alphabet(letter):
    # Получаем позицию буквы в алфавите (1 для 'a', 2 для 'b' и т.д.)
    return f"Position of alphabet: {ord(letter) - ord('a') + 1}"
print(position_in_alphabet("a"))
``` 
