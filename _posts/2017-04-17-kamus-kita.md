---
layout: post
title: KamusKita
---

TLDR: I made an Urban Dictionary copy

<img src="/images/kamus_kita_screenshot.png" alt="KamusKita screenshot" style="max-width: 400px;"/>

I really like Urban Dictionary (UD). I like its simplicity and straightforward-ness. I also like how they allow anyone to submit word definitions. So, I thought, why not make something like it for Malaysians? We have a lot of unique undocumented words. While UD have language selection when you submit a definition, it's still kinda too broad. I wanted to make something localized to Malaysians. Something that all of us can relate to.

I developed the app using Ruby on Rails as back-end and Foundation for the front-end. I chose Rails because I've been using Rails for so long that I'm confident I can build the app within days. Which I did. It took me 2 days. I chose Foundation instead of Bootstrap because it looks cleaner and more *professional* to me.

At first, it was hard imagining things as how the model should look like. Given that there are many words, and each words have many definitions, I had to stop to think for a while. Most probably because I have the tendency to complicate stuffs. After some time, I decided to make it definition based dictionary. So, users can submit a defintion at will; all they have to provide is a word(doesn't matter how it's spelt), the definition and an example. Then the system decides what to do on it's own.

What I did was to find (or create if not found) the new word before a definition is saved. Then, the definition is saved to the word. It's clearer when it's in my mind. So, users can submit multiple definitions for a word, without actually having to know the word (that the app knows) or having to submit the word first.

Furthermore, users can like and dislike definitions. The most liked definitions will be the default definition for their respective words.

Lastly, I deployed the app to Heroku on free dyno so it's kinda slow but it's serving it's purpose for now. So all is well.

The app is at [https://kamuskita.zaidhuda.com/](https://kamuskita.zaidhuda.com/)
