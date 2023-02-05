# SimpsonsGPT: AI to Write Episodes of the Simpsons

## The idea here was to use episode titles as prompts in order to generate 'episodes' of The Simpsons. This was a great exercise for understanding the strengths and limitations of decoder architectures.

## Notes on Output: GPTs are spectacular at generating realistic text. The jig is up quite quickly though, when it becomes clear that GPT output contains limited internal logic. Yes, this technology is amazing. Also yes, the hype is excruciating.

## Try it here [Jupyter notebook]() for a more thorough explanation of this project.


### SAMPLE OUTPUT: 

```
EPISODE TITLE: Tales of Ancient Springfield

EPISODE SUMMARY: 

 The students gather in front of the statue, listening to Homer speak.

 Bart reads a book on ancient humanism.  He notices that most people have never been to
 see such a thing before.  They start to discuss their religions with each other.  
 ``What religion are you talking about?'' asks Apu.
 ``The Hindu faith,'' replies Lisa, who looks up ``a new religion''.  
 ``This is my `new religion', so I guess it's fair game.''  
 
 So they read some scriptures...
 
 Marge finds the word `gifts' on the cover.  At first, she says it doesn't rhyme, but
 when her friends look at it and sigh, they notice it as though it were an old comic book.  (``Oh, no!'' concludes Maggie)

 Smithers takes Burns' books away from his mouth and puts them under a microscope.
```

### This is cool!

Despite being plotless and nonsensical, the model does seem to be able to create representations of the Simpsons universe.

### Why can't GPT make a whole coherent episode?

Well, the context window is always going to be limited. In other words, there are limitations in the model's ability to look backwards 'in time' when generating text. Maybe at some point, the GPUs will become powerful enough to allow for a much larger context window. In the meantime, any text generation is going to meander quite a bit. We are far from an era when AI can generate entire novels without significant human intervention. 

# Notes on this Project:

- I scraped the episode summaries from [this website](https://www.simpsonsarchive.com/episodes.html). It appears that real scripts from The Simpsons aren't readily available, so I made do with this rather messy compendium. 
- The output is a great lesson in the weaknesses of GPT insofar as it's clear that the model doesn't understand the familial relationships between the Simpsons characters, resulting in some highly unfortunate innuendo at times. This is thus a perfect example of how production-grade NLP models need to be carefully analyzed and tested before deployment. GPT doesn't know anything -- it's just a probabilistic word model, which is cool, but not intelligent.


