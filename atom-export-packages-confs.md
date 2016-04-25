#### :rocket: Export and import my Atoms packages & configurations

I'm a big fan of [Atom](http://atom.io), who doesn't no :tea: ?  
But sometimes could be a little hard to have differents environments (home, work, friends, and so on...) so i want a simple way to **export** my configurations and **import** them in one easy step so a make this [shell script](https://raw.githubusercontent.com/juliomatcom/atom-configuration-pkgs/master/install.sh) that works out of the box *(tested with Ubuntu)*.  
The script will merge the packages already installed in your system with the packages list in [packages.txt](https://raw.githubusercontent.com/juliomatcom/atom-configuration-pkgs/master/packages.txt) file and copy the config files to your *~/.atom* folder and you will have a new Atom configured and ready to be productive as always. Yes thats it.

#### Using this with your owns packages and configurations files
Should not be too hard to change the **packages.txt** list for any others of your choices, just change line 12 for
`filename=my-custom/atom-configuration-pkgs/packages.txt`

Another way is **fork** the [repo](https://github.com/juliomatcom/atom-configuration-pkgs) 
and replaces the config files in *confs/* folder and packages.txt for your owns.

Check the original repo at [https://github.com/juliomatcom/atom-configuration-pkgs](https://github.com/juliomatcom/atom-configuration-pkgs)

Hope this could help you too.  
Until the next, 

[@juliomatcom](https://twitter.com/juliomatcom)
