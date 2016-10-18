---
title: "Install Ruby"
published: true
morea_id: install-ruby
morea_type: experience
morea_summary: "How to install and use Ruby on Windows and on a Mac."
morea_sort_order: 3
---

# Install Ruby
The install process for ruby is different based on the type of computer you are using.  Install information is provided here for Windows & Mac OS.  If you are using Linux, it is likely that you already have git and if not can use the package manager to easily install it.

## Windows Users
If you are a Windows user you will not have ruby available by default.  You will need to download and install ruby from the web. You can get it from [Ruby Installer](http://rubyinstaller.org/downloads/), but will need to carefully choose your version.  It is recommended to use the latest 32 bit Ruby 2.2.X installer.  

Make sure that you check the options to add ruby to your path.
<img class="img-responsive" src="{{ "/morea/intro/images/ruby-install-options.png" | prepend:site.baseurl }}" alt="Screenshot of install options">


## Mac Users
If you are using a Mac, open up a [Terminal](http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line) window and type `ruby --version`.  You may find that ruby is already installed, or if not that it will prompt you to install the XCode Command Line Developer Tools.  If it does not, you can install ruby using [RVM](https://rvm.io/) which will also allow you to have different versions installed.  This is handy even if it is installed by default as you may want a newer version.  

Open terminal and use the following `curl` commands to install rvm with the latest stable ruby version.

{% highlight bash %}
$ \curl -sSL https://get.rvm.io | bash -s stable --ruby
{% endhighlight %}



## Verify Install
Once you have Ruby installed, make sure to verify that you have access to it from the shell:

{% highlight bash %}
$ ruby --version
{% endhighlight %}

My examples will use Ruby 2.2.x, but any version of Ruby 2 should be fine for this course.  

If you are not seeing a line that shows your version of Ruby, you will need to do some troubleshooting or try uninstalling and then reinstalling ruby.  First, close all your shell windows and reopen them to try again.  If you are using the Windows installer, make sure to check the box to add ruby to your path.  
