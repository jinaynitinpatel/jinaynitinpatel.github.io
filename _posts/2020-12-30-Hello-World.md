---
layout: post
title: Installing OpenMP on mac!
permalink: /OpenMP-on-Mac
---
If you want to install OpenMP on mac, follow the steps below
-  Install homebrew for mac, if you don't have already. Visit [brew]({https://brew.sh/}) to install homebrew
-  Installing gcc with brew {% highlight python %} brew install gcc {% endhighlight %} 
-  Find the location where gcc is being installed. Generally, it should be in /usr/local/bin. However, when calling a compiler your bash will look into /usr/bin by default. Hence, you need to add the new directory to your PATH. Export the path using following command. 
{% highlight ruby %} export PATH=/usr/local/bin:$PATH {% endhighlight %}
-  Now compile with OpenMP with following command
{% highlight ruby %} gcc-10 -fopenmp -o prog_name prog_name.c {% endhighlight %}
Note:- gcc-10 is the current version that I installed. You may have installed gcc-8 or gcc-7 or maybe someother version in future release. 
