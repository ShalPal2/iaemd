# Illustrated, Animated, English-Malayalam Dictionary. 

What's the malayalam word for 'wave'? Depends on which wave we are talking about!

This dictionary was built as an exploration of the tricky connections between words in translation. Between the multiple meanings of a word in one language, the many connections it forges with sister words in the other language,and the many meanings of those words- looking up a word in this dictionary can be a joyride of discoveries.

**Here is a quick map to explore ahead:** 
1. You can read more about the logical structure of this dictionary [here](#This-dictionary-is-a-labyrinth).
2. You can read about the design decisions here.
3. **_look up a word, or explore the dictionary [here]._**

## This Dictionary is a Labyrinth
When building the structure of this dictionary, my primary concerns were:
1. How can I make sure the user finds the relevant entry with the least amount of on-screen parsing?
2. How can I make make it possible for them to go on a rabbit-chase of adjacent words?

To elaborate on the first concern, let us say we came across the sentence "She waved at her". Unfortunately, we do not know what 'waved' means! So, we drop into IAEMD, and search for 'waved'. 
What if the result that you got was this (tldr; the bold text is our relevant entry):
> ### **Wave**
> the rise and fall of fluids;പഗിനി കതിലു കാരദിപി.
>

The first consideration is  **What is the skeletal language of the content?**
There are two possibilities: English("en"), Malayalam("ml"). The deciding factor is the language the user is approaching the dictionary from.