---
layout: post
title:  "Researching and Developing"
date:   2017-07-10
---

_Welcome to my beautiful world of sloppy implementations and tryhard
developing_  

//Alice must be proud

## What I'm up to?

Friday and today my actions were the following: 
* I researched on using Emacs as the [LSP client](https://github.com/emacs-lsp/lsp-mode), but got seriously frustrated on
how sloppy in terms of design the existing lsp-mode is and how hard it was, at
least for me to set it up and use it. I tried setting it up with the [lsp-java](https://github.com/emacs-lsp/lsp-java) language
server. Emacs Lisp and all those buffers are still a little harsh _pour moi_
and in general I was not satisfied by the documentation at all. It was not
friendly.

The list of candidate clients for the LSP implementation are:
* [Eclipse IDE](https://github.com/vladdu/lsp4e)
* [Eclipse
  Che](https://eclipse.org/che/docs/assemblies/sdk-language-server-protocol/index.html)
* ~~[Emacs](https://github.com/emacs-lsp/)~~
* [Neovim](https://github.com/autozimu/LanguageClient-neovim)
* ~~[vscode](https://code.visualstudio.com/docs/extensions/example-language-server)~~


## Why I won't use VS Code

VS Code gets an immediate red flag from me, even tho it's the best functioning
LSP client, with the most _capabilities_, just because I don't like MS products
and when I tried to set it up around 2 years ago it f'd me up.  

## Why Emacs is a dead-end

Emacs gets an F due to my poor EL skillz. And because it's gonna be on alpha
until the end of the decade IMHO in LSP terms.

## Eclipse Che Thoughts

I like the whole spirit of Eclipse Che. It's an ambiguous project that's doing
great so far. But I'm afraid to use it as my editor and I think that I'll have
a real hard time implementing LSP on it. Afraid of a dead end, but not yet
discouraged. Mayve the next couple o' days show me the truth..


**So**, what my conclusion to all this IS to use either Eclipse IDE or neovim as
our client. I didn't put any hands on effort within the weekend, which means
that I started working on these today. Neovim LSP client has some solid
documentation and Eclipse has a lot of people contributing to its LSP stuff
actively, which gives me hope that they'll make their documentation a little
friendlier soon.

## Eclipse Issues

Right now I'm trying to set up the necessary workspace in Eclipse IDE to
connect the client with the [Groovy LS](https://github.com/palantir/language-servers/tree/develop/groovy-language-server), as mr.Per requested me to do so like a
personal challenge. 

There are two issues I'm currently having:
1. I don't know how to package the damn thing with Eclipse IDE 
2. My Eclipse installation has issues installing some necessary dependecies

## What's next?

Tomorrow Thuesday I'll visit the hsgr to continue works. Hopefully I'll have
the Groovy LS working on a client. Gonna devote some time in learning how to use neovim.
We'll see..

Hasta la victoria siempre,  
Harry
