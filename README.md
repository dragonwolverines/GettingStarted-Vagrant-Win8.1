Few weeks back, someone mailed me asking me to check their company product and asked me to give feedback. <br>
So, i geek-ed into their website and found something called <a href="http://en.wikipedia.org/wiki/Vagrant_%28software%29">"vagrant"</a>.
<br>
While reading about it in curiosity, i found it cool. It's built in Ruby. So, i decided to play with it. <br> <br>
Here are some of the following steps to get started with <code>Windows 8.1</code>:- <br>
Note: None of the steps works in offline. Make sure to turn on the Internet ;) <br>
<b>Step 1:</b> Install <a href="https://www.virtualbox.org/wiki/Downloads">VirtualBox</a>.<br>
<b>Step 2:</b> Install <a href="https://www.vagrantup.com/downloads.html">Vagrant</a>.<br>
Note:- If you are <code>Windows 10 user</code>, then make sure to test it in another system which already has Windows10.<br>
After successfully installing Vagrant in Windows10, then I'd to restart my system for booting. <br>
Then... BAM! Windows10 collapsed and died. So, this is a warning.<br>
<b>Step 3:</b> Install <a href="http://the.earth.li/~sgtatham/putty/latest/x86/putty.exe">PuTTY</a>.<br>
<b>Step 4:</b> Install <a href="http://the.earth.li/~sgtatham/putty/latest/x86/puttygen.exe">PuTTYgen</a>.<br>
Good job! Now, we will require <code>Cloud</code>. <br>
<b>Step 5:</b> Open Command Prompt (run as admin). Dive-in to the directory location.<br>
If your files in another disk, then type cd\ and followed by <code>d:</code> or <code>e:</code> or whatever. <br>
Remember to remove the <code>Vagrant file</code> which will be found in <code>bin</code> folder. <br>

<b>Step 6:</b>
<code>vagrant init ubuntu/trusty64</code> --- this is official box for Ubuntu Server 14.04 LTS. <br>

<b>Step 7:</b><br>
<code>vagrant up</code> --- Now, we need to wait for few hours for the installation to complete. <br>
<b>Step 8: </b> --- Now, installation is completed. <br>
For listing the virtual boxes --> <code>vagrant box list</code> <br>
If we wanna delete a box --> <code>vagrant box remove box/name </code> <br>
During the end of installation in step 6, we would have noticed a problem in <code>SSH</code>. <br>
For that, we require to use <code>PuTTY</code>. <br>
<b>Step 9:</b> <br>
Open PuTTY. <br>
Set host address as <code>127.0.0.1</code> and port as <code>2200</code> <br>
As default, <br>
For config, check --> <code>vagrant ssh-config</code> <br> and also:- <code>vagrant ssh</code> <br>
<b>Step 10:</b><br>
Next is about using public key and private key... <br>
Open PuTTYgen. <br>
If you already have a public/private key, then click <code>load</code> and load the key. <br>
You may already have one stored in <code>.vagrant.d</code> which is insecure. <br>
If not, then click <code>Generate</code>.<br>
After generating it, click <code>Save Private Key</code> and then, <code>Load</code>. <br>
In the meantime, open <code>PuTTY</code>, expand <code>SSH</code> towards your left. <br>
Click <code>Auth</code>. Then, To your right, browse and add the saved private key. 
<br>
<b>Important Basic Hints:- </b><br>
To check vagrant status -> <code>vagrant status</code><br>
To stop or turn off vagrant -> <code>vagrant halt</code><br>
To suspend vagrant -> <code>vagrant suspend</code><br>
To resume vagrant -> <code>vagrant resume</code><br>
To turn back vagrant on -> <code>vagrant up</code><br>
<br>
As developers, next is about setting-up a development environment using Vagrant. <br>
<b>Step 11:</b><br> Go to <b><a href="https://github.com/Varying-Vagrant-Vagrants/VVV#the-first-vagrant-up">VVV</a></b> and follow from step 4 to get started with <code>setup configuration</code>. 
<br>
After successfully accomplishing <code>step 11</code>, Here are bunch of free toys we will get to play:- 
<br>
<code>WordPress Develop, WordPress Stable, WordPress Trunk, WP-CLI, nginx 1.6.x, mysql 5.5.x, php-fpm 5.5.x, 
memcached 1.4.13, 
PHP memcache extension 3.0.8,
PHP xdebug extension 2.2.5, 
PHP imagick extension 3.1.2, 
PHPUnit 4.0.x, 
ack-grep 2.04, 
git 1.9.x, 
subversion 1.8.x,
ngrep,
dos2unix,
Composer,
phpMemcachedAdmin,
phpMyAdmin 4.1.14 (multi-language),
Opcache Status,
Webgrind,
NodeJs Current Stable Version,
grunt-cli Current Stable Version
</code>
