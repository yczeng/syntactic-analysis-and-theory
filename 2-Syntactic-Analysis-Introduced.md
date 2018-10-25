# 2. Syntactic Analysis Introduced

One way to examine language is to look at the linguistic "input" and "output" - the physical properties o flinguistic signals.
For example, there is no acoustic boundary between stems and affixes. So these must be inferred by some kind of analysis of the linguistic input that we can perform.

stimulus -> process S + representation R -> observed response O

### 2.1 Word order

How do we account for the fact that only certian linear orders of words are acceptable?
What is it that speakers know, perhaps tacitly, uncounsciously, that explains this?

* First idea: people remember patterns.
     * Rebuttal: There are infinitely many well-formed phrases in language. All strings ould not be stored in memory because we need infinite storage capacity and humans are finite discrete creatures with finite memories.
* Second idea: phrases that humans could speak or understand are bounded in length. Humans can have in mental storage all the strings used in their lifetimes.
     * Rebuttal: The number of sentences that people produce is very large, so that if you count all the sentences people sya, well over half of them are sentences that will only ever be spoken or written once.
     * "Penn Treebank 2" has more than 1 million words of text, mainly from the *Wall Street Journal*. Here, more than 99% of the sentences occur only once.
* Third idea: What is humans memorize sequences such as D N V D N and D N V D N P D N?
     * Not true that all following sequence D N C D N is acceptable. For example "Those air put a compliments" makes no sense. What seems to be required as a minimum is the hypothesis that linguistic knowledge involves recursive rules that are not sensitive to properties like pength. 

Syntax has to do with the order of words and morphemes in phrases.

### 2.2 Constituency

Languages are chunky: organized into chunks or blocks or units that "rules" can manipulate as blocks.

Definition: a *constituent* is a string that speakers can manipulate as a single chunk.
Questions:
* What are the constituents and how do we determine what they are?
* What are the basic elements of syntax, the "syntactic atoms"?
* How do we go about deciding?
* Do constituents cluster into subgroups, and how do we determine subgroup membership?

### 2.3 Substitution

Experiment: replace constituents with words that have no internal structure (so, roots).

For example: The girl in the red coat will put a picture of Bill on your desk befroe tomorrow. "The girl in the red coat" can be replaced with "she" or "Mary".

We can find that constituents belong to the same category and share some property, for example some distributional property. 

There are some negative results. For example, "She will put a picture of Bill on your desk before tomorrow" cannot be "Bill will put a picture of she on your desk before tomorrow" (she should be her). We cannot draw strong conclusions from negative results (this is like the exceptions that we learned in class (for rules)!)

However, sometimes we replace chunks in sentences and the resulting grammar is correct, but the category of the chunks are different and the meaning of the sentences have changed dramatically. "This girl will put a picture of Bill on your desk before *tomorrow*." and "This girl will put a picture of Bill on your desk before *Monday because it is important*.". 

Summary points:
* Substitutions replace a substring by a word where that word plays the same role in the sentence as the original string did.
* Strings that can be manipulated as chunks under substitution are constituents.
* Substitution of a string by a word seems to indicate consituency
     * Substitution by a pronoun indicates that the constituent may be a DP
     * Substitution by *one* or *ones* can indicate that the constituent may be a NP
     * substitution by *do* or *do so* indicates that that the constituent may be a CP
     * substitution by *there* in its locative sense can indicate that the constituent may be a PP
* String usbstitution failure is not a test for non-constituency
* Substitution by a string longer than one word is not necessarily one that preserves constituency
* The pronunciation of certain elements depends on their surroundings.