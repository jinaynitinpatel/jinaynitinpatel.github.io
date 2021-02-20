---
layout: post
title: Installing OpenMP on mac!
---
If you want to install OpenMP on mac, follow the steps below
1. Install homebrew for mac, if you don't have already. Visit [brew]({https://brew.sh/}) to install homebrew
2. Installing gcc with brew {% highlight ruby %} brew install gcc {% endhighlight %}
3. Find the location where gcc is being installed. Generally, it should be in /usr/local/bin. However, when calling a compiler your bash will look into /usr/bin by default. Hence, you need to add the new directory to your PATH. Export the path using following command. 
{% highlight ruby %} export PATH=/usr/local/bin:$PATH {% endhighlight %}
4. 

