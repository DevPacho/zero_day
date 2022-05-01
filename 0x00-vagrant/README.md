<h1>[Optional project] Vagrant</h1>

<img src="https://ostechnix.com/wp-content/uploads/2020/12/Check-username-and-hostname-in-vagrant-machine.png">

<p>©. <a href="https://ostechnix.com/how-to-reset-vagrant-virtual-machine-to-original-state/" target="_blank"><i><b>Image source</a></i></b></p>
<br>
<h2>Resources</h2>
<p><strong>Read or watch</strong>:</p>
<ul>
    <li><a href="https://intranet.hbtn.io/rltoken/NcuS4-7zF9-edjbo157uQQ" target="_blank" title="Zero day">Zero day</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/v2RbeSrU14w3KTwbGYH3Fw" target="_blank" title="Virtual machine">Virtual machine</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/3AHxDiZwhZwPM_GiHox0gQ" target="_blank" title="man uname">man uname</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/i2CtlPhs4zaAbtEUdY2l3A" target="_blank" title="Resources to learn Git">Resources to learn Git</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/86HNyB59eoxAhtIahOXKGQ" target="_blank" title="About READMEs">About READMEs</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/4szBlqEXwOgr1YON9bxhPQ" target="_blank" title="How to write a Git commit message">How to write a Git commit message</a></li>
</ul>
<h2>Learning Objectives</h2>
<p>At the end of this project, you are expected to be able to&nbsp;<a href="https://intranet.hbtn.io/rltoken/9E9csOc85_TcgG0jeF8Oxw" target="_blank" title="explain to anyone">explain to anyone</a>,&nbsp;<strong>without the help of Google</strong>:</p>
<h3>General</h3>
<ul>
    <li>What is a zero-day</li>
    <li>What is a virtual machine</li>
    <li>What is Vagrant</li>
    <li>Who wrote Vagrant</li>
    <li>What is Ubuntu</li>
    <li>What does &ldquo;Ubuntu&rdquo; mean</li>
    <li>How to use VMs with Vagrant</li>
    <li>What does the command&nbsp;<code>uname</code> do</li>
    <li>What is source code management</li>
    <li>What is Git</li>
    <li>What is GitHub</li>
    <li>What is the difference between Git and GitHub</li>
    <li>How to create a repository</li>
    <li>What is a README</li>
    <li>How to write good READMEs</li>
    <li>How to commit</li>
    <li>How to write helpful commit messages</li>
    <li>How to push code</li>
</ul>
<h2>Requirements</h2>
<h3>General</h3>
<ul>
    <li>A&nbsp;<code>README.md</code> file at the root of the repo, containing a description of the repository</li>
    <li>A&nbsp;<code>README.md</code> file, at the root of the folder of&nbsp;<em>this</em> project (i.e.&nbsp;<code>0x00-vagrant</code>), describing what this project is about</li>
</ul>
<h2>More Info</h2>
<h3>Install&nbsp;<code>git</code></h3>
<p>If&nbsp;<code>git</code> is not already installed on your terminal:</p>
<pre><code>$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git</code></pre>
<h3>Basic usage</h3>
<p>At the end of this project you should be able to reproduce and understand these command lines:</p>
<pre><code>$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main</code></pre>
<h3>Warning</h3>
<p>This project <b>can’t be done in Sandboxes</b> - it can be done only in your local computer. Please refer to our concept pages for your operating system.</p>
<br>
<h1>Tasks</h1>
<h2>0. Create and setup your Git and GitHub account</h2>
<p><b><i>Advanced task</i></b><p>
<p>You will need Git for this project, you might have to&nbsp;<a href="https://intranet.hbtn.io/rltoken/TJrA7MIEl9LxnkGNH_ddmw" target="_blank" title="install it">install it</a> on your computer if it&rsquo;s not done yet.</p>
<ul>
    <li>Configure your basic info (name, email) on your local machine &ndash; they will be part of your commits.&nbsp;<a href="https://intranet.hbtn.io/rltoken/72jmwYpf2OeuoOn9XM3vQg" target="_blank" title="Tips">Tips</a></li>
</ul>
<p>On&nbsp;<a href="https://intranet.hbtn.io/rltoken/m27bKy8K40cIkyHWQ36i2w" target="_blank" title="GitHub.com">GitHub.com</a>:</p>
<ul>
    <li>Using the graphic interface on the website, create the repository (if it&rsquo;s not done yet)<ul>
            <li>Description:&nbsp;<code>This is my first repository as a full-stack engineer</code></li>
            <li>Public repo:&nbsp;<code>zero_day</code></li>
            <li>No&nbsp;<code>README</code>,&nbsp;<code>.gitignore</code>, or license</li>
        </ul>
    </li>
</ul>
<p>On your computer, open a terminal and do the following:</p>
<ul>
    <li>Navigate to your home directory.&nbsp;<a href="https://intranet.hbtn.io/rltoken/-odz94uVNOsPV1ovYZLuyw" target="_blank" title="Tips">Tips</a></li>
    <li>Create a directory&nbsp;<code>zero_day</code>.&nbsp;<a href="https://intranet.hbtn.io/rltoken/AHYBfU0itf9qEiwLdiaVJw" target="_blank" title="Tips">Tips</a></li>
    <li>Navigate to this new directory.&nbsp;<a href="https://intranet.hbtn.io/rltoken/9g9c-qBPHWSGcpxbs69ASw" target="_blank" title="Tips">Tips</a></li>
    <li>Initialize git and add the remote origin</li>
    <li>Create a file&nbsp;<code>README.md</code> with Emacs (or other command line editors) and write a small&nbsp;<a href="https://intranet.hbtn.io/rltoken/Ru3ANLuzGs4g0v2qsN3efA" target="_blank" title="Markdown">Markdown</a> text to present this project.&nbsp;<strong>This file is mandatory in projects</strong></li>
    <li>Add this new file to git, commit the change with this message &ldquo;My first commit&rdquo; and push to the remote server / origin (Note: You will probably need to set your login/password to push to the remote server)</li>
</ul>
<p>Good job!</p>
<p>You pushed your first file in your&nbsp;<strong>first repository</strong> of the&nbsp;<strong>first task</strong> of your&nbsp;<strong>first School project</strong>.</p>
<ul>
    <li><b>GitHub repository:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day" target="_blank">zero_day</b></i></a></code></li>
    <li><b>File:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x00-vagrant/README.md" target="_blank">README.md</b></i></a></code></li>
</ul>
<br>
<h2>1. Hello Ubuntu</h2>
<p><b><i>Advanced task</i></b><p>
<p>Inside the&nbsp;<code>zero_day</code> repo, create a new directory called&nbsp;<code>0x00-vagrant</code>. Add a&nbsp;<code>README.md</code> file to this directory.</p>
<p><code>ssh</code> into your Ubuntu VM. What does the command&nbsp;<code>uname</code> print when you run it without any option?</p>
<p>Type your answer into a file in the&nbsp;<code>0x00-vagrant</code> directory and push it to GitHub. Name your file accordingly as shown below.</p>
<ul>
    <li><b>File:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x00-vagrant/0-hello_ubuntu" target="_blank">0-hello_ubuntu</b></i></a></code></li>
</ul>
<br>
<h2>License & Copyright</h2>
<i>©. Project provided by: <a href="https://www.holbertonschool.com/" target="_blank"><b>Holberton School</a></i></b>
<br>
<i>©. Project developed by:<b> Francisco Ramírez </b><b>|&nbsp;<a href="https://github.com/FranRM15" target="_blank"> GitHub</a> <b>|</b>&nbsp;<a href="https://twitter.com/FranciscoR_15" target = "_blank" rel="nofollow"> Twitter</b></a></p>
