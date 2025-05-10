# Les champs de pistes: an unbounded distributed collaborative music

## Motivations

How could an unlimited number of people collaborate on one piece of music?

How could this be accessible to as many people as possible? To people with little
money or technical knowledge or bandwidth?

How could this happen with as little technology as possible? With no technology?

## The idea

A **champ de pistes** is a conceptual tape recorder with a potentially unbounded
number of tracks called **pistes**, numbered 1, 2, 3, etc, and sometimes named as
well.

Pistes contain audio **segments**. A segment is a _location_ of an audio
recording, it identifies a recording somewhere on or off the internet.
Note that the recording itself does not have to be stored anywhere with the
piste - the segment points to the audio, it does not contain the audio.

"Recording" is left under-specified. The exact definition of what a recording
can be depends on the specific champ.

Each segment has a **début/start time** within its piste, and a
**durée/duration**. Segments in a piste cannot overlap, but they can touch at the
ends.

Segments are **immutable** which means that once they are placed on a piste they
"cannot"(*) be removed.

A **mix** is a set of instructions on how to mix pistes from one or more champs
into single piece of audio.

A mix can be a program in Python or some other language.

For many people, a mix would be some sort of human-readable score they would
prepare and give to someone else's program to prepare the output for
them.

That score might also be prepared by a program - for example, a program that
reads and records faders a person uses like a classic mixing board, or something
much more radical.

## A concept first, with some technology to make it happen.

I want to re-emphasize that at its base, a champ de pistes is not a
technological thing.

A group of people could agree to a champ de pistes and organize it on paper or
even in their heads, using stopwatches and whatever devices they had at the time
(LPs, cassettes, MiniDisc, wax cylinders), or even sheet music, singing and a
good sense of time (whether sheet music is a "recording" would depend on what
the champ's definition of a recording was.)

That said, there will be simple technology to let you easily do useful things


------

(* - The quotes are because, of course, there will be a way to remove illegal or
offensive segments from your piste, if only for the protection of the nice
people playing our game from the creeps. But it will be possible to just rewrite
history as if the little nastiness never happened, so it will _appear_ as if
immutability were true.

(On the technological side, this is not the big, heavy, hype-magnet named
Blockchain but a proven, lightweight, 70s-vintage technology called the Merkel
tree, in the form of our old, familiar friend, Git.)
