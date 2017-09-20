# phrasal_verbs
Code to mine for the most common phrasal verbs in corpora

### Introduction
Adult learners of English have trouble acquiring phrasal verbs.  Phrasal verbs are those that consist of a verb and an associated preposition or adverb. For example, in the sentence '_Bob will come home and take off his shoes_', **take off** is a phrasal verb. There are a couple of reasons that phrasal verbs are difficult for learners.  

First off, the meaning of these verb+preposition combinations is opaque - the combination creates a totally different meaning than the sum of the parts.  There are also multiple meanings per combination.  Examples include:
>* bring up (_raise \(i.e. a child), mention a topic for the first time in conversation_)
>* take off  (_leave quickly_, or _remove_)

Secondly, these phrasal verbs don't all behave the same syntactically.  Some can take a direct object, and some can't:
>* The rocket took off.
>* The rocket took off the shield (very different meaning)
>* Don't **bring up** the topic at dinner tonight.

and some can put that direct object in between the verb and the preposition/adverb. Others can only do it...pronouns explanation here.

>  Don't **bring** the topic **up** at dinner tonight.  
>  Don't **bring** it **up** at dinner tonight.  
>  \*Don't **bring up** it.  (Terrible)

Linguists have all sorts of fun debating [how to best describe these verbs](https://www.linguisticsociety.org/sites/default/files/e-learning/42.%20SyntacticAmbiguity_TheyDecidedOnTheBoat.pdf), and whether there are in fact multiple types of verbs - those that are truly 'particle' verbs, and those that are just a verb and correlated preposition.  

### Purpose
This code will help English language learners by helping them concentrate on learning the most common phrasal verbs first.  It will run over the corpora (TBD) and extract the verbs with corresponding prepositions, and order them in rank of prevalence/frequency.

#### Foreseen Problems

* The fact that many times the verb and particle will be separated.  Luckily, there seems to be at least some sort of bias in language preventing chunks from getting too big and verbs from getting toooo far separated from their particle.  There will be a range limit.  
* Distinction between a true phrasal, a particle, and a correlation.
* Finding the corpora.
