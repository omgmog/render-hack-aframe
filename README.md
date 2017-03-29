# Multi-user VR experiences with A-Frame
> At the Render Conference 2017 Hackathon

This repository contains a bunch of useful things to take part in my guided project at the Render Conference evening hackathon.

If you're reading this either you're in the wrong place, or I suggested you come here to get started.


## An introduction to A-Frame

A-Frame is like the jQuery of Three.js and WebVR. _That's not as insulting as it sounds._ A-Frame is a really great tool to make creating WebVR projects simple.

From the A-Frame docs:

> A-Frame is a web framework for building virtual reality experiences. It was started by Mozilla VR to make WebVR content creation easier, faster, and more accessible.
>
> A-Frame lets you build scenes with just HTML while having unlimited access to JavaScript, three.js, and all existing Web APIs. A-Frame uses an entity-component-system pattern that promotes composition and extensibility. It is free and open source with a welcoming community and a thriving ecosystem of tools and components.


## Some resources I've put together previously

I held a hackday last Summer ([Game Dev Day](http://gamedevday.club/)) and so created some resources to get attendees up to speed. You can find them here:

- [An introduction to A-Frame (PDF)](https://github.com/omgmog/gdd-2016/blob/master/Intro%20to%20A-Frame.pdf)
- [A-Frame guide](http://blog.omgmog.net/gdd-aframe-guide/)

Also, though not using A-Frame, for some examples of what can be done with JavaScript and Google Cardboard check out the things that I made each day in October last year for [Cardboctober](https://cardboctober.xyz/).

Some highlights from Cardboctober:

- Gaze-based look interaction ([Write-up](https://blog.omgmog.net/post/cardboctober-03/), [Demo](https://cardboctober.xyz/max/03/))
- A "pairs" game ([Write-up](https://blog.omgmog.net/post/cardboctober-06/), [Demo](https://cardboctober.xyz/max/06/))
- Speech recognition ([Write-up](https://blog.omgmog.net/post/cardboctober-09/), [Demo](https://cardboctober.xyz/max/09/))
- Beat sequencer ([Write-up](https://blog.omgmog.net/post/cardboctober-11/), [Demo](https://cardboctober.xyz/max/11/))


## Other resources

- [Official A-Frame docs](https://aframe.io/docs/)
- [Official A-Frame School (tutorial)](https://aframe.io/aframe-school/)
- [Official A-Frame examples](https://aframe.io/aframe/examples/)
- [A-Frame boilerplate](https://github.com/aframevr/aframe-boilerplate/)
- [Bringing Virtual Reality to the web with A-Frame](http://tengio.com/blog/bringing-vr-to-the-web-a-frame/)

## A starting point for our project today

So today we're going to create an A-Frame project that connects users to one another. We'll be using the following technologies:

- A-Frame
- Socket.io / WebRTC
- Network A-Frame
  - [Project on Github](https://github.com/haydenjameslee/networked-aframe)
  - [Tutorial](https://github.com/haydenjameslee/networked-aframe/blob/master/docs/Tutorial:%20Create%20your%20first%20Networked-Aframe%20experience.md)


The exact theme of our project is undecided (or may be decided when you're reading this). Some ideas I've had in the past that would work nicely with this, and might lend themselves to being completed in 3-4 hours:

- Werewolf in VR ([Game rules](http://www.brenbarn.net/werewolf/rules.html))
- 3D Pong (2 players (or more!))
- Guess who / Find the target / Sniper

## Limitations

There are obviously going to be some limitations to using Google Cardboard as our platform of choice. These are mainly in performance/quality and input methods. We can do headtracking well enough, but our input is limited to gaze-based gestures, and (depending on the headset) screen touch events.

We're also limited in terms of _locomotion_ -- so in most experiences the user will be stuck in one position, but will be able to look around.
