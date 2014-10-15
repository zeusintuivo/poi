poi
===

A set of tools to contribute to Mozilla better. 

Why ?
=======
Because there you are, trying to make a difference to the world. And you turn your eye into "mozilla." The fascinating world of coding for Mozilla. After a week hours in the machine, you realize: "geeez this is harder than I thought, I might as well go back to been selfish and not move a single finger." 

It turns out, learning to contribute is very hard. The instructions are very complex, and usages and commiting and pushing. It only gets you huffing and puffing.

After detailed analysis, I thought to make a significant contribution by creating effitient way to contribute, with less headches. 


Tools 
======

kuma-* A set of scripts for Mozilla Developer Network (Kuma) MDN to facilitate the contributing workflow with ease. Based on the instructions from Kuma's https://github.com/mozilla/kuma/blob/master/CONTRIBUTING.md and Install http://kuma.readthedocs.org/en/latest/installation-vagrant.html.

fireplace-* A set of scripts for Mozilla Marketplace (fireplace) to facilitate the contributing workflow with ease. Based on the instructions from Kuma's https://github.com/mozilla/kuma/blob/master/CONTRIBUTING.md and Install http://kuma.readthedocs.org/en/latest/installation-vagrant.html.

About Naming
=====
I named them "kuma", or "fireplace", because it will make it easier to remember in which folder I am working for example

> kuma is for

~~~
~/Sites/kuma (master) $ _
~~~



Install 
======
I recommend to git clone it or append it to ~/bin like this:

~~~~
git clone https://github.com/zeusintuivo/poi ~/bin
~~~~

If you already have stuff in ~/bin
then you can just add it like this:

~~~~
git clone https://github.com/zeusintuivo/poi ~/bin2
cp -rf ~/bin2/* /bin
~~~~

This will leave ~/bin2 directory folder in your ~/
if you want you want to delete it:

~~~~
rm -rf ~/bin2
~~~~

Usage
=====

### kuma

#### Pre-requisites 
1. First browse Bugzilla for Bugs to fix for MDN (kuma), and pick a bug number. 
2. Set up your working environment 
3. I am guessing you cloned the code
4. Once you have a bug# and you have access to IRC #mdndev from irc.mozilla.org
5. You are ready to contribute.

#### Contributing

> Use kuma-new-issue 888888 to start like this 

~~~
kuma-new-issue 1068486
~~~

make sure you place your own bug#

> Now, work on the bug

> Use kuma-run to start the vargrant server like this: 

~~~
kuma-run
~~~

Once you are logged in the server run the foreman start:

~~~
foreman start
~~~

Once you have fixed, coded, and drank some coffe and ate some candies. 
You are ready to push !

> Use kuma-commit to push changes like this:

~~~
kuma-commit "I fixed some changes message here"
~~~

Remember to place your own message.

Once you want to stop your development, do want to "pause" your vagrant
and maybe you are the kind that forgets that this vargrant is running.
I don't have to explain that you press Ctrl+C to stop foreman start
and that you type exit to exit the vagrant-virtualbox machine. 

But if you forget vagrant suspend, you can always type "k" -> tab
then type "s" -> and press "enter."

~~~
kuma-suspend
~~~

Easy cheese!


### fireplace 

#### Pre-requisites 
1. Fork project online from https://github.com/mozilla/fireplace.git
2. Have your terminal open and be in the place (location, directory, folder), where you want to clone the project. 

> Use fireplace-setup to clone and setup you the whole environment like this:

~~~
fireplace-setup johana-git-guru-user-name-here
~~~

> Use fireplace-compile to run the compilation procedures

~~~
fireplace-compile
~~~

> Use firepace-settings to cat (see, observe, printout) the settings file

~~~
fireplace-settings
~~~

> Use the fireplace-test to run the testing procedures

~~~ 
fireplace-test
~~~




Stage
=====
20141010 - Creation. This is my first try. I guess you can call it *alpha for now



