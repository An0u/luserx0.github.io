---
layout: post
title:  "Wind of Change"
date:   2017-07-05
---
  
### Greetings to all the lamers of this world,  

## The project has changed its scope  

SchemeScript as a valid Kawa IDE integration has sunk. I have lost my passion
to it due to not being able to figure out the huge codebase I'm dealing with
and mr.Per got a little frustrated by my results. That's ok since we are no
losers and have the ability to adjust in difficult situations.   Haven't
wirtten in a while in this blog exactly because I didn't have a certain plan on
my mind to portray.

## Language da Server w/ Protokewl

So what are we up to?  

We are going to implement the youngster of protokewls [Language Server
Protocol](https://github.com/Microsoft/language-server-protocol)
(abbr. LSP). Ok it's an initiative of Microsoft and for that judgement comes
above all, so as to not get criticised for this decision in the not so distant
future. As it seems it's a great initiative and potentially the future of IDEs
as well as editors (Vim, Emacs, Sublime, etc).  

## "How will ye do it Harry?"  

I'll try to use as basis for a client the existing [Emacs LSP client
implementation](https://github.com/emacs-lsp/lsp-mode) and if that fails I will
lightning quick switch to the [Eclipse LSP client
implementation](https://github.com/eclipse/lsp4j). Pretty kewl so far.  

The challenge lies on the server. How will the client-server communicate? How
will the server be structured? What is a legal milestone for GSoC? Also: Will
Google approve of this transition?  

Well the answer to those questions is mr.[Duncan
Mak](https://github.com/duncanmak). He will help me along with Per Bothner to
write the server in Kawa Scheme.  


Still researching and trying to come up with a plan.  
More info soon.  
Harry


