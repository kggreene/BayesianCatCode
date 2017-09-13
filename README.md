# BayesianCatCode
code for blending Bayesian statistics and cats in a Twitter chatbot

### Functionality
Mad Libs - replaces words in Bayesian sentence with cat words (and other way around) based on part of speech. 

### Bayesian Mad Libs Examples
Starting with:
A Bayesian network is a graphical model that encodes probabilistic relationships among variables of interest. (Nouns to replace: network, model; plural nouns to replace: relationships, variables) 
 
Example replacements:
A Bayesian laser pointer is a graphical scratching post that encodes probabilistic fish among socks of interest. 

A Bayesian scratching post is a graphical fish that encodes probabilistic birds among salmon treats of interest. 

A Bayesian bird is a graphical feather toy that encodes probabilistic cat beds among flattened ears of interest. 

### NLP/POS automated noun identification
In Bayesian Cats Mad Libs, parts of speech of words to replace are manually chosen and stored with each sentence. Initially I used Stanford's core nlp http://corenlp.run/ to replace nouns but found that the results for automating noun identification were inferior for humor. Subject and the humor in mixing the two subjects were both conveyed much more effectively by choosing which nouns to replace and by often replacing them with an adjective noun pair, e.g. using 'scratching post' rather than just a noun, e.g. 'post'. It also became apparent that there are additional distinctions between subcategories of nouns that affect which noun can correctly take another's place with no other modifications to the sentence. One simple example is whether a singular noun starts with a vowel or not when the word before it is 'a' or 'an'.   

### twitter bot
http://twitter.com/bayesiancats

##### Bri's GitHub with full BayesianCats code
https://github.com/bmchorse/bayesiancats
