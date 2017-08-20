# hello-world

I am an English teacher at a university in China, trying to learn Chinese. I have found some good apps online, but none of them have random Chinese sentence generators. They are all pre-written. 


Random Chinese sentence generator

My goal for now is to create a complete application that generates random sentences from a specific topic. The sentences are Chinese simplified and pinyin. 

My level of programming experience is very, very low. I did a course on Java on Khan which I thought was really great, but I couldn't install Java properly. Since then, I've downloaded Python and SQLite: they both work! Yesss....

So, my goal here is to create a learning tool for Chinese. I am about 1/2 way through a beginner's course. As I mentioned, I was going through an excellent Java course, at the same time, and I thought that what I learned through that course I could apply to creating a learning tool using Java. Of course, Java wouldn't install properly, even after following all the directions and fiddeling... but I think what I learned there is probably doable with the Python language. 

I am here because someone recommended it.

So... here is the pseudocode and pseudotables:

=====

sentenceStructure table:
integer unique
simpleSentence = subject(topic)noun + subject(topic)verb + object(topic)
complexSentence = subject(topic)noun + subject(topic)verb + conjunction + object(topic)
compoundSentence = ...
complexCompoudSentence = ...
// The topic would be chosen as a user event while the key would be used to determine what kind of sentence would be constructed

topic(noun) table:
integer unique
English word
Chinese word
Timesused = Timesused + 1 // local variable)

topic(verb) table:
integer unique
English word
Chinese word
Timesused = Timesused + 1

topic(object) table:
integer unique
English word
Chinese word
Timesused = Timesused + 1

dictionary table containing a complete list for the topic tables to reference:
integer unique (key)
Englishword
Chineseword
topicswordisusedin
partofspeech
determiner // boolean
if boolean determiner = true, then a reference to the determiner(s) // example The/a

// some topics would be basics, animals, food, directions, etc. Each topic would have certain key words, and some general words. Subjects such as I, he, you, we, and some specific verbs *eat, drink*, to go with specific objects ie,  *eat fish* *drink milk* etc. 

Python psuedocode for making a random sentence

user selects topic
random number between 0 and sentenceStructure(length).
// example, random number is 0 which is a simple sentence
random number for pronoun
// chooses a pronoun subject from the pronoun subject list. Again, rolls a 0 which is the pronoun I.
random number for verb
// chooses a verb from topicverb
random number for object
// chooses a random object from topicobject

output: I drink water (in Chinese)

Pseudocode for adding a topic or adding to a topic

add the English word, Chinese word, part of speech, choose name for topic, determiner required yes/no, (date added automatically), difficulty rating

-------

So where am I now.. I am trying to figure out how to fill out the tables with data, but unsure how to do that with SQLiteStudio. Should I build a part of the application... if so, how do I create the event to do it. So I need to learn the GUI stuff behind Python to do so I think. So that is what I think I need to do now.
