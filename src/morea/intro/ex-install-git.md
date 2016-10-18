---
title: "Install Git"
published: true
morea_id: install-git
morea_type: experience
morea_summary: "How to install git on Windows through GitHub Desktop, and check for and install git (if needed) on a Mac."
morea_sort_order: 2
---

# Install Git
The install process for git is different based on the type of computer you are using.  Install information is provided here for Windows & Mac OS.  If you are using Linux, it is likely that you already have git and if not can use the package manager to easily install it.

## Windows Users
If you are a Windows user, typically you will use PowerShell as your command shell.  However, Windows PowerShell does not include git by default.  You will need to download and install git from the web. You can get it from the [Git-SCM Downloads](https://git-scm.com/download/win).

I recommend that you keep the default install settings suggested by the installer, specifically:
<img class="img-responsive" src="{{ "/morea/intro/images/git-install-opt1.png" | prepend:site.baseurl }}" alt="Screenshot of install options">
<img class="img-responsive" src="{{ "/morea/intro/images/git-install-opt2.png" | prepend:site.baseurl }}" alt="Screenshot of install options">


This will install a few different options that allow you to work with Git on a Windows computer.  You may choose any of them you like, but I would recommend GitBash as it will be closest to what you may see from my examples.


## Mac Users
If you are using a Mac, open up a [Terminal](http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line) window and type git.  You may find that it is already installed, or if not that it will prompt you to install the XCode Command Line Developer Tools.  If it does not, you likely have an older version of the Mac OS and should download and install the tools from the [Apple Developer Site](https://developer.apple.com/downloads/index.action).  You can also install the full XCode suite from the Apple App Store, but this will take additional space.  


## Configure Git
Before you dive in, you'll want to configure git with your user information. In the commands below, fill in your name and the email you used with your GitHub account.  This email is what will tie your activity to your account.  **Make sure that you are using the same email and check for typos.**

{% highlight bash %}
$ git config --global user.name "User Name"
$ git config --global user.email "user@email"
{% endhighlight %}

I also recommend saving your git config as a Gist on GitHub so that it is easily available for you to use on any computer.  

You will only need to do this at home once, but you may need to do it each time you use a college lab computer as the configuration may not be saved from use to use.
