---
title: 'Challenging myself to use vim'
description: 'Trying to figure out how to fit vim in my programming setup.'
pubDate: 'Aug 16 2024'
tags: ['vim', 'programming', 'learning']
# heroImage: '/blog-placeholder-3.jpg'
---

I have been trying to get on the vim hypetrain for a very long time now,
I understand the value, love the flow state of vim movement and getting things done all within the terminal.
But every time I tried to get into it I would get overwhelmed with a sharp angle of the vim learning curve.
I would come in expecting an experience akin to the other text editors I used before, VScode, Sublime or Pycharm. 
Most of your problems have a solution just a plugin install away, everything is already included and configured for your convenience. 
As most people who tried vim already know this is very much not the case here,
in order to get the modern IDE experience you need to make vim your own,
 and that takes focus and effort.

## My experience so far

Around 2020 I got familiar with basic vim movement and started using [Vimium](https://vimium.github.io/) for chrome. 
I didnt really want to build the editor myself, especially since I didn t exactly know what I was doing back then, 
so I played around for a while with [SpaceVim](https://spacevim.org/),
since it has a lot of the features you would normally expect in a IDE already pre-built and configured. 
Plugins are interconnected via leader keys and theres a really cool feature that shows you what menus you can open after pressing a key.
Potentially you would learn how to use spacevim while working with it just by following the tooltips.
That really didnt stick with me, I found the pre-built editor experience even more of a mental strain then trying to piece one together on my own. 
I would spend more time trying to change things, install more plugins instead of just using what has already been given to me by the pre-build.
So I stuck with my usual PyCharm setup and didnt really use vim at all for a while,
just popping in there from time to time to learn about splits and try to use it on remote machines.

2 years later I made the switch from Windows to a M1 Mac and with that came a fresh install of vim, 
I didnt want to copy my config specifically because I finally decided that it clearly hasnt been working for me.
This time I tried to build my own vim experience, I installed a bunch of plugins that would try to replicate the average IDE experience.
Session manager, debugger, file explorer and a bunch of other things of varying usability.
I fell down the rabbit hole of productivity and spent way too much time trying to make vim function like an IDE,
while not actually doing anything productive because, well it wasnt comfy enough.
I would install plugins for my plugins to make even the tiniest of changes work, like an image viewer or something.

Around 2023 I watched a video of The Primeagean talking about the [telescope plugin](https://github.com/nvim-telescope/telescope.nvim).
The main takeaway for me was this idea that the way IDEs have a file explorer open by default and always on is actually a waste of visual space,
you dont actually need to see all of your files open 99% of the time,
and its much better to just open it only when you specifically need to.
And with telescope you just jump exactly where you want by looking up for the specific search term. 
That way you can always focus on things that matter,
jumping between windows and brining up file tree only when you need to.

That made me trash my init.vim one last time and start from the beginning once again.
Now I went very limited, installing only the most basic plugins and only when I actually knew what I wanted to do with them.
I got telescope, [coc](https://github.com/neoclide/coc.nvim), [startify](https://github.com/mhinz/vim-startify) and [nerd-commenter](https://github.com/preservim/nerdcommenter).
With that I felt confident enough to be able to do light text editing,
without being distracted by too many things. At this point im pretty happy with what I have,
but I still couldnt really find the confidence to just switch to use vim full-time,
I was still extremely slow, ending up opening my projects in pycharm.

## Finally feeling comfortable

Well, now its August 2024 and I decided to make this blog,
just a simple project that I can use to tinker and showcase some projects,
 write about things etc. Usually I would just spin up the usual VScode project,
 but this time, finally, I decided to try and work exclusively in vim.
I already had a more-or-less working setup that I was comfortable in.
For a typescript project I really was only missing a way to interact with a terminal in a convenient way.
Previously I would either just use a separate iTerm window or launch vim in tmux.
Both are not the best approaches, tmux has its own learning curve and a bunch of shortcuts that are configured and handled separately,
pretty much the same applies to using a separate iTerm window.
So I found something called [toggleterm](https://github.com/akinsho/toggleterm.nvim).
It uses nvim's internal terminal and is exactly what I was looking for, as a bonus I configured lazygit to handle git within vim just a keystroke away. 

While my setup is still not perfect, I think for the first time ever I actually dont reach for other tools and can be productive in vim.
I have my dotfiles saved in a [github repo](https://github.com/Wattabak/dotfiles) and I'm going to try and use vim exclusively at least while working on this blog. 

