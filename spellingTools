#this module will provide basic programs to analyse, regolarise and check spellings. It will also provide basic analytic tools for general text analysis

numbers = "0123456789"
alphabet_lower = "abcĉdefgĝhĥijĵklmnoprsŝtuŭvz"
alphabet_upper = alphabet_lower.upper()
alphabet = alphabet_lower+alphabet_upper

alphabet_special_lower = "ĉĝĥĵŝŭ"
alphabet_special_upper = alphabet_special_lower.upper()
alphabet_special = alphabet_special_lower+alphabet_special_upper

def computerSpelling(world):
    # computer spelling for EO repleces the special characters with diptongs
    # composed by a base letter (c, g, h, j, s, u) and x 
    word_CS = ""
    for letter in word:
          if letter in alphabet_special:
              letter += "x" if letter in alphabet_special_lower else "X"
              word_CS += letter
    return word_CS
  
  def canonSpelling(word):
      word_canon = ""
      for index in range(1, len(word)):
          if word[index] in ['x', 'X']:
              letter = alphabet[alphabet.index(word[index]-1]
              word_canon += letter
          word_canon += word[index]
       return word_canon
