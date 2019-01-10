---
layout: post
title: "This is not a blog ..."
date: 2018-03-01 17:21:44 +0000
permalink: this_is_not_a_blog
excerpt_separator: <!--more-->
---

I want to write about Object Oriented Programming (OOP). This is where most people (including myself) get tripped up. I am by no means an expert, but the other day I felt something click.<!--more--> I was thinking about the videos and the lesson on the topic. The lesson contained an image of one of my favorite paintings by my favorite artist.

![](https://upload.wikimedia.org/wikipedia/en/b/b9/MagrittePipe.jpg)

I fell in love with René Magritte while a philosophy major in college. This is one if his most famous works entitled,_ La trahison des images_. The French title can be translated as either a “Treachery” or “Treason” of Images. The words in the painting translated from french are “This is not a pipe.”

My naive reaction to this painting was a mix of intrigue and bemusement. The intrigue, I would like to think, came from a sense that there was something more to this painting than an apparent contradiction. The bemusement came from a lack of understanding of the philosophical difficulty this work represents. Coming to terms with this philosophical difficulty is, I believe, the key to understanding OOP.

What does it mean? I think the best explanation comes from the man who painted it:

> “The famous pipe. How people reproached me for it! And yet, could you stuff my pipe? No, it's just a representation, is it not? So if I had written on my picture 'This is a pipe', I'd have been lying!”
>
> — René Magritte

My initial reaction which gave rise to the bemusement was, “Uh, of course that’s a pipe!” I think this reaction is what causes people to look at Surrealist art and roll their eyes. Grasping the deeper meaning, I believe, adds richness to our experience of art and life itself.

The name for the philosophical study of these concepts is metaphysics (specifically ontology). Even the names of the subject sound esoteric. I am not going to bore you or embarrass myself by trying to solve this philosophical puzzle in the space of this blog. My hope at this point is that I am not adding to the confusion.
The quote from Sir Tim Berners-Lee is what strikes me as particularly illuminating:

> “In an extreme view, the world can be seen as only connections, nothing else. We think of a dictionary as the repository of meaning, but it defines words only in terms of other words. I liked the idea that a piece of information is really defined only by what it's related to, and how it's related. There really is little else to meaning. The structure is everything. There are billions of neurons in our brains, but what are neurons? Just cells. The brain has no knowledge until connections are made between neurons. All that we know, all that we are, comes from the way our neurons are connected.”
>
> ― Tim Berners-Lee

Plato suggested that what makes an object belong to a certain category involved it’s relation to a perfect object (often described as a ‘Form’) that exists in some celestial realm. The quote above seems to suggest a more mundane definition of meaning.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/49/%22The_School_of_Athens%22_by_Raffaello_Sanzio_da_Urbino.jpg/800px-%22The_School_of_Athens%22_by_Raffaello_Sanzio_da_Urbino.jpg)

The two men in the center of this painting are Plato (left) and Aristotle (right). Plato is pointing up toward the ‘heaven’ where perfect things exist. Whereas, Aristotle is pointing out toward the real world. These are the extreme positions one can take as to the nature of things and reality. My experience with polar opposite theories is that the truth usually lies somewhere in the middle. Plato's theory was that a pipe is a pipe because it is in some nebulous way related to the perfect pipe that exists in 'heaven'.

It seems to me at this point that Ruby is somewhat Platonic in its approach to objects.

```
class Pipe
    Initialize
    ...
    end
end
```

This is the creation of the blueprint/factory for all the individual pipes in existence. It is the Form in Platonic heaven.

`Pipe.new`

This is the real pipe with attributes and methods that one can stuff with tobacco... or is it?
