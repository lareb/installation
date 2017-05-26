INSTALLATION OF RUBY ON RAILS ( From Source )
=============================================

INTRODUCTION
------------

Ruby is a powerful, flexible programming language you can use in web/Internet development, to process text, to create games, and as part of the popular Ruby on Rails web framework. Ruby is a scripting language designed by Yukihiro Matsumoto, also known as Matz. It runs on a variety of platforms, such as Windows, Mac OS, and the various versions of UNIX.

Installation Methods
--------------------

There are several ways to install Ruby:
* When you are on a UNIX-like operating system, using your system’s package manager is the easiest way of getting started. However, the packaged Ruby version usually is not the newest one. 
* Installers can be used to install a specific or multiple Ruby versions. There is also an installer for Windows. 
* Managers help you to switch between multiple Ruby installations on your system. 
* And finally, you can also build Ruby from source. 

Installing Ruby for Ubuntu 14.04
--------------------------------

**Install the dependencies required**
                                                                                                                                                                                  
```
$ sudo apt-get update

$ sudo apt-get install build-essential

$ sudo apt-get install autoconf bison build-essential libssl-dev libyaml-dev libreadline6-dev zlib1g-dev libncurses5-dev libffi-dev  libgdbm3 libgdbm-dev

```

**Downloading ruby**

```
$  wget ftp://ftp.ruby-lang.org/pub/ruby/2.4/ruby-2.4.1.tar.gz
```

**UnZip the Ruby file**
                                                                    
```
$ tar xzvf ruby-2.4.1.tar.gz
```                                                                   

**Enter into the downloaded directory.**
                                                                    
```
$ cd ruby-2.4.1
```                                                                   

**Configure generates the make file and also checks that the server has all of the required dependencies.** 

```
$ ./configure
```                                                                   

**After that, still in the directory, you need to run the "make" command.**
                                                                    
```
$ make
```                                                                  


This may take a bit longer. Once it finishes, use **make install**
                                                                    
```
$ make install  
```                                                                  

**Installation of Bundler**
 
```
$ gem install bundler
```                                                                  


Since ruby package is installed from the source, the gems should already be downloaded. However, they need to be updated.
                                                                 
```
$ gem update --system
```                                                                  

Installation of Rails
---------------------
                                                                 
```
$ gem install rails
```                                                                  

Verify that Rails has been installed properly by printing its version, with this command
```
$ rails -v
```
If it installed properly, you will see the version of Rails that was installed.
