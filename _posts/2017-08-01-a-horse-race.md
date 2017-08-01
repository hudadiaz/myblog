---
layout: post
title: A horse race
---
Recently, I had a technical interview with a startup for a back end developer position. The questions they asked was quite hard for me to answer. I don't know if it was because I haven't done anything for a while or I was nervous or I was just unprepared.

The interview lasted for 2 hours. It was almost disastrous. The first thing they asked was for me to fix my SQL response I sent them beforehand. It was to find duplicates and I assumed there will only be up to 2 duplicates for each record and they wanted it to be able to find more. I tried my best but I just couldn't do it, probably because I was never doing pure SQL. I felt really bad.

Then I had to do bunch of other things. I remembered they asked me find the first `n` digits of _pi_. Then they asked me to print the index of `n` in _pi_. I took the easy path and assume `n` is a digit and now that I think about it, `n` should be a number and my solution wouldn't be able to solve it if it is indeed a number instead of a digit because my solution was to convert _pi_ up to 20 decimal point to string then find the index of `n`.

Finally, I had to write some Ruby classes to solve a simple horse racing problem. I had 2 problems at that moment. First problem, I never wrote a pure Ruby code! Second problem, I don't have enough time to think of the solution... The problem was quite simple. Given `h` number of horses and `t` number of tracks, find the least number of races to find the first and second fastest horses. I couldn't solve that.

This problem stuck in my head for a while. Sure, I had my chance and solving it now wouldn't magically pass me the interview but it should calm me down. So, I think what I could do was to:

1. race the horses in groups of `t`
2. race all the first horses in groups of `t`
3. repeat until there's less than or `t` horses
4. for the first 2 horses of the final group, get the second horse from their initial groups
5. race the four horses to find the first and second fastest horses
6. record all the races to find out how many races actually done

There you have your horses. I feel a bit redeemed.
