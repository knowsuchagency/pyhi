.. title: Luke Davis Interview
.. slug: luke-davis-interview
.. date: 2015-09-07 16:13:36 UTC-10:00
.. tags: interviews, Luke Davis, python, vagrant, webassembly
.. category: interviews
.. link:
.. description: A short interview of Luke Davis from Planet Labs.
.. type: text

Summary
=======
Today we had a chance to sit down and talk to `Luke Davis`_ from `Planet Labs`_. Planet Labs launched with the idea of imaging every spot on the planet every day. They have now launched more satellites in to orbit than any other organization in the world and are devoted to using their platform to improve our Earth. Luke's recent projects involve a large Django web application that allows satellite operators to have a web-based gui to control the entire network of spacecraft! His typical development environment involves Vagrant_ virtual enviroments, private git repos, and lots of Python.

.. TEASER_END

How did you become a programmer?
--------------------------------
  In Spring, 2008, I realized that programming was a way to think outside your head, and thinking was something extremely valuable. Therefore, with that idea I knew I had to learn to program. I also knew that I had to be excellent at it, and move up that gradient to master it. At some point, I was given the opportunity to move from a hobby to a vocation and I jumped on the opening. I didn't set out to have a job as a programmer, I set out to become excellent at programming because of the relationship to thought.

Why did you choose Python?
--------------------------
  Universality. Python is the lingua franca of scientific computing and many other things. Python spans so many communities and you can take part in a huge conversation about programming, machine intelligence, and many other things. That opportunity doesn't exist in other languages like Ruby, C++, or javascript. The low barrier to entry and preeminence with the scientific computing community creates a perfect mix of easy for novices, yet full featured enough for profession research. There is a smooth onboarding from novice to professional. When you compare Python to Java/C++ , both have a great scientific community but those other languages are much harder for people to get involved in. In a similar situation with R, there is a great community but it is much smaller and not a good fit for what I like doing: thinking. All that is why I think Python is an attractive language.

Do you use other programming languages?
---------------------------------------
  Yes, JavaScript. JS is the native language of the winning platform, web browsers. JS is also good for teaching because of the immediate feedback and universal web browser. There is no need to setup a development environment, dependences, or anything else. It is really invaluable to do things on the web and I am doing a lot on the web. I wouldn't use JS if it wasn’t part of the winning platform. For instance, Lua is a great language that I would use but it didn't win, so there isn't a large community and there are not a variety of modules. When you go to look for something in Lua, you may end up having to go build it from scratch.
  I think we are living in the zenith of JavaScript. You have already seen things come and pull the market from JS, like coffescript, but soon if the WebAssembly_ train doesn't get derailed, we'll see the decline of JS. Apple, Google, Microsoft, Mozilla, and others have all agreed to push forward on WebAssembly to create a low level bytecode for web browsers. JS tries to be a good language and a good compiled target, but it isn't really good at either one. WebAssembly will be an extremely fast target for compiled languages for any browser that is part of the consortium. If WebAssembly doesn't get derailed, JS will decline.

What has been your favorite Python project?
-------------------------------------------
  Well at work we use Python to control satellites! We've built a suite of tools to control the birds, the ground stations, and every thing else. The satellite has a linux based controller and runs Python so literally everything we do can be Python based. An example, you can manipulate how the satellite is pointing. We have two systems for that, all controlled with Python. The first is a reaction wheel using gyroscopes, which moves very fast. The second, for slower movements, is a magnetorquer which applies torque to the satellite by interacting with the Earth's magnetic field! We also use Python to establish a radio connection with the ground stations and control the ground site antennas. The ground site antennas must point within 1-2 degrees of arc of the satellite in order to communicate.

What is your favorite Python module?
------------------------------------
 Good old **datetime**! I hate calculating timestamps, and this save me so much time. I literally use it every day, multiple times a day. We have 15 ground sites across the Earth so we are constantly calculating local time zones and time differences.

.. _Planet Labs: https://www.planet.com/
.. _Luke Davis: http://www.lucaswadedavis.com/
.. _Vagrant: https://www.vagrantup.com/
.. _WebAssembly: https://medium.com/javascript-scene/what-is-webassembly-the-dawn-of-a-new-era-61256ec5a8f6
