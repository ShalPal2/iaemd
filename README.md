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
> **wave _noun_(WATER)** a raised line of water that moves across the surface of an area of water,especially the sea.
>--_wave breaks/crashes_ At night, I listened to the sound of waves breaking/crashing against the shore.
>**wave _noun_(BY A CROWD)** a wave-like movement made by a crowd watching a sports game, when everyone stands and lifts up their arms and then sits down again one after another. _The crowd did the Wave._
>**wave _noun_(ENERGY)** the pattern in which some types of energy, such as sound,light, and heat, are spread or carried. _Radio waves._
>**wave _noun_(LARGE NUMBER)** a larger than usual number of events of a similar, often bad, type happening within the same period. _A crime wave. **wave of-** The country was swept by a wave of protests._
> - **a new,second etc. wave of something** a numbe rof events of a particular type that happen again or are repeated after a pause. _A new wave of job losses is expected this year._
>**wave _noun_(STRONG FEELING)** a sudden strong feeling that gets stronger as it spreads. _A wave of panic swept through the crowd._
>**wave _verb_(MOVE)** to raise your hand and move it from side to side as a greeting, or to get someone's attention or give information. _She leaned out the window and waved goodbye. As soon as we showed our papers as journalists, the policeman waved us in._

If they were using a physical dictionary, the confusion of navigating this wall of text might be reduced by the grounding tactile experience of searching through a physical page. In the absence of it, on a screen, with the initial confusion of not knowing the meaning of a word you've come across- this is death by a paper cuts to the ones who need a dictionary most. 
It is important to serve the most likely word to the reader, at the earliest.

Now the second concern: the rabbit-chase of adjacent words. Suppose we recieved the same search: 'waved'. There is an important clue in this word- the tense indicates that it can only be related to **wave_verb_(MOVE)**. So we could return just this: 
>### **Wave**
> >**wave _verb_(MOVE)** to raise your hand and move it from side to side as a greeting, or to get someone's attention or give information. _She leaned out the window and waved goodbye. As soon as we showed our papers as journalists, the policeman waved us in._
...and leave it at that. But this is a missed opportunity to add extra value to the reader's experience. 

The first consideration is  **What is the skeletal language of the content?**
There are two possibilities: English("en"), Malayalam("ml"). The deciding factor is the language the user is approaching the dictionary from.