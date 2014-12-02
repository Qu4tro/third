


Why?
The main reason is that ifttt is not opensource. 
Anyone can add agents and anyone can add new features. You also don't need to trust someone with your data.
Huginn is a good alternative, but I have two problems with it:
Agents must be written in ruby. It's not that ruby is a bad language, but why not gather more programmers, by making possible that ANYONE with programming knowledge can contribute.
It gives you a web interface and nothing else. 



Project Guidelines:

Daemon/Client arquitecture

Agent Guidelines:

Each agent **must** be completed sandboxed in a Docked env.

Each agent must present its actions and reactions according to some guidelines(I'm thinking a small config file is enough)

Testing, Documentation and Logging is of paramount importance!

Logging using syslog-ng

Documentation using [lit](https://github.com/cdosborn/lit)

Testing using [assert.sh](https://github.com/lehmannro/assert.sh)

OAuth whenever possible


Initial goals:

Simple cli client

Agents:

    Email
    Date and time
    RSS
    Pushbullet
    Dropbox
    Weather
    XMPP


Later goals:

Web, Desktop, Curses clients

Replicate most ifttt channels

Each condition can have more than one action and more than one reaction

Condition-Sharing website

Pipe? (Pipe agent)
