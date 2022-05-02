<h1>0x03. Git</h1>
<img src="https://www.edureka.co/blog/wp-content/uploads/2016/11/Git-Architechture-Git-Tutorial-Edureka-2.png">
<p>©. <a href="https://www.edureka.co/blog/git-tutorial/" target="_blank"><i><b>Image source</a></i></b></p>
<br>
<h2>Resources</h2>
<p><strong>Read or watch:</strong></p>
<ul>
    <li><a href="https://intranet.hbtn.io/rltoken/rOOPwBFp4ezRunQ0G0YHYQ" target="_blank" title="Resources to learn Git">Resources to learn Git</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/4CwCa3MmQvJfXu5poTRVQw" target="_blank" title="About READMEs">About READMEs</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/zkdCE4WEr9H91WlOpfNlGA" target="_blank" title="How to write a Git commit message">How to write a Git commit message</a></li>
</ul>
<p><strong>Resources for advanced tasks</strong> (Read only after finishing the mandatory tasks):</p>
<ul>
    <li><a href="https://intranet.hbtn.io/rltoken/514Jj2WL9uL6wOyOYWejdA" target="_blank" title="Learning branching">Learning branching</a></li>
    <li><a href="https://intranet.hbtn.io/rltoken/ZUE0eoAWDKadJd4QCQkzQg" target="_blank" title="Effective pull requests and other good practices for teams using GitHub">Effective pull requests and other good practices for teams using GitHub</a></li>
</ul>
<h2>Learning Objectives</h2>
<p>At the end of this project, you are expected to be able to&nbsp;<a href="https://intranet.hbtn.io/rltoken/9nDe1J66MhvFwTm9pj88WQ" target="_blank" title="explain to anyone">explain to anyone</a>,&nbsp;<strong>without the help of Google</strong>:</p>
<h3>General</h3>
<ul>
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
    <li>How to pull updates</li>
    <li>How to create a branch</li>
    <li>How to merge branches</li>
    <li>How to work as collaborators on a project</li>
    <li>Which files should and which files should not appear in your repo</li>
</ul>
<h2>Requirements</h2>
<h3>General</h3>
<ul>
    <li>A&nbsp;<code>README.md</code> file at the root of the repo, containing a description of the repository</li>
    <li>A&nbsp;<code>README.md</code> file, at the root of the folder of&nbsp;<em>this</em> project (i.e.&nbsp;<code>0x03-git</code>), describing what this project is about</li>
    <li><strong>Do not use GitHub&rsquo;s web UI</strong>, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won&rsquo;t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.</li>
    <li>Your answer files should only contain the command, and nothing else</li>
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
<br>
<h1>Tasks</h1>
<h2>0. Create and setup your Git and GitHub account</h2>
<p>You will need Git for this project, you might have to&nbsp;<a href="https://intranet.hbtn.io/rltoken/n2SJyaVuu1tuhVgHSKw5Sg" target="_blank" title="install it">install it</a> on your computer if it&rsquo;s not done yet.</p>
<ul>
    <li>Configure your basic info (name, email) on your local machine &ndash; they will be part of your commits.&nbsp;<a href="https://intranet.hbtn.io/rltoken/WCZwvMlDTWNwo7D2h5RXiw" target="_blank" title="Tips">Tips</a></li>
</ul>
<p>On&nbsp;<a href="https://intranet.hbtn.io/rltoken/YNvmlBzyEYR4EcwFclIbwQ" target="_blank" title="GitHub.com">GitHub.com</a>:</p>
<ul>
    <li>Using the graphic interface on the website, create the repository (if it&rsquo;s not done yet)<ul>
            <li>Name:&nbsp;<code>zero_day</code></li>
            <li>Description:&nbsp;<code>This is my first repository as a full-stack engineer</code></li>
            <li>Public repo</li>
            <li>No&nbsp;<code>README</code>,&nbsp;<code>.gitignore</code>, or license</li>
        </ul>
    </li>
</ul>
<p>Update your Intranet profile by adding your Github username&nbsp;<a href="https://intranet.hbtn.io/rltoken/18IAhpoWtIm4rxdhYLU3kg" target="_blank" title="here">here</a> - if it&rsquo;s not done,&nbsp;<strong>the Checker won&rsquo;t be able to correct your work</strong></p>
<p>On your computer, open a terminal and do the following:</p>
<ul>
    <li>Navigate to your home directory.&nbsp;<a href="https://intranet.hbtn.io/rltoken/nSl91LBC_er1QmayRs60Rg" target="_blank" title="Tips">Tips</a></li>
    <li>Create a directory&nbsp;<code>zero_day</code>.&nbsp;<a href="https://intranet.hbtn.io/rltoken/qE0DHC3e86f7eZF6mlqFyQ" target="_blank" title="Tips">Tips</a></li>
    <li>Navigate to this new directory.&nbsp;<a href="https://intranet.hbtn.io/rltoken/hgr3egDWXiBW_PIDqBAWDA" target="_blank" title="Tips">Tips</a></li>
    <li>Initialize git and add the remote origin</li>
    <li>Create a file&nbsp;<code>README.md</code> with Emacs or Vi (or other command line editors) and write a small&nbsp;<a href="https://intranet.hbtn.io/rltoken/Na_yqM9Y5nNNXtvjVAxZKA" target="_blank" title="Markdown">Markdown</a> text to present this project.&nbsp;<strong>This file is mandatory in all School projects</strong></li>
    <li>Add this new file to git, commit the change with this message &ldquo;My first commit&rdquo; and push to the remote server / origin (Note: You will probably need to set your login/password to push to the remote server)</li>
</ul>
<p>Good job!</p>
<p>You pushed your first file in your&nbsp;<strong>first repository</strong> of the&nbsp;<strong>first task</strong> of your&nbsp;<strong>first School project</strong>.</p>
<ul>
    <li><b>GitHub repository:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day" target="_blank">zero_day</b></i></a></code></li>
    <li><b>File:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/README.md" target="_blank">README.md</b></i></a></code></li>
</ul>
<br>
<h2>1. Repo-session</h2>
<p>Create a new directory called&nbsp;<code>0x03-git</code> in your&nbsp;<code>zero_day</code> repo.</p>
<p>Make sure you include a not empty&nbsp;<code>README.md</code> in your directory:</p>
<ul>
    <li>at the root of your repository&nbsp;<code>zero_day</code></li>
    <li>AND in the directory&nbsp;<code>0x03-git</code></li>
</ul>
<p>And important part:&nbsp;<strong>Make sure your commit and push your code to Github - otherwise the Checker will always fail.</strong></p>
<ul>
    <li><b>GitHub repository:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day" target="_blank">zero_day</b></i></a></code></li>
</ul>
<br>
<h2>2. Coding fury road</h2>
<p>For the moment we have an empty project directory containing only a&nbsp;<code>README.md</code>. It&rsquo;s time to code!</p>
<ul>
    <li>Create these directories at the root of your project:&nbsp;<code>bash</code>,&nbsp;<code>c</code>,&nbsp;<code>js</code></li>
    <li>Create these empty files:<ul>
            <li><code>c/c_is_fun.c</code></li>
            <li><code>js/main.js</code></li>
            <li><code>js/index.js</code></li>
        </ul>
    </li>
    <li>Create a file&nbsp;<code>bash/best</code> with these two lines inside:&nbsp;<code>#!/bin/bash</code> and&nbsp;<code>echo &quot;Best&quot;</code></li>
    <li>Create a file&nbsp;<code>bash/school</code> with these two lines inside:&nbsp;<code>#!/bin/bash</code> and&nbsp;<code>echo &quot;School&quot;</code></li>
    <li>Add all these new files to git</li>
    <li>Commit your changes (message: &ldquo;Starting to code today, so cool&rdquo;) and push to the remote server</li>
</ul>
<ul>
    <li><b>Files:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/bash/best" target="_blank">bash/best</b></i></a></code>, <b></b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/bash/school" target="_blank">bash/school</b></i></a></code>, <b></b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/c/c_is_fun.c" target="_blank">c/c_is_fun.c</b></i></a></code>
</ul>
<br>
<h2>3. Collaboration is the base of a company</h2>
<p>A branch is like a copy of your project. It&rsquo;s used mainly for:</p>
<ul>
    <li>adding a feature in development</li>
    <li>collaborating on the same project with other developers</li>
    <li>not breaking your entire repository</li>
    <li>not upsetting your co-workers</li>
</ul>
<p>The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers&rsquo; work.</p>
<p>For this project, create a branch&nbsp;<code>update_script</code> and in this branch:</p>
<ul>
    <li>Create an empty file named&nbsp;<code>bash/98</code></li>
    <li>Update&nbsp;<code>bash/best</code> by replacing&nbsp;<code>echo &quot;Best&quot;</code> with&nbsp;<code>echo &quot;Best School&quot;</code></li>
    <li>Update&nbsp;<code>bash/school</code> by replacing&nbsp;<code>echo &quot;School&quot;</code> with&nbsp;<code>echo &quot;The school is open!&quot;</code></li>
    <li>Add and commit these changes (message: &ldquo;My personal work&rdquo;)</li>
    <li>Push this new branch&nbsp;<a href="https://intranet.hbtn.io/rltoken/w-vaOsoyqzITnQQ2NoSf6g" target="_blank" title="Tips">Tips</a></li>
</ul>
<p>Perfect! You did an amazing update in your project and it&rsquo;s isolated correctly from the&nbsp;<strong>main</strong> branch.</p>
<p>Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:</p>
<ul>
    <li>Change branch to&nbsp;<code>main</code></li>
    <li>Update the file&nbsp;<code>bash/best</code> by replacing&nbsp;<code>echo &quot;Best&quot;</code> with&nbsp;<code>echo &quot;This School is so cool!&quot;</code></li>
    <li>Delete the directory&nbsp;<code>js</code></li>
    <li>Commit your changes (message: &ldquo;Hot fix&rdquo;) and push to the origin</li>
</ul>
<p>Ouf, hot fix is done!</p>
<ul>
    <li><b>Files:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/bash/best" target="_blank">bash/best</b></i></a></code>, <b></b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/bash/school" target="_blank">bash/school</b></i></a></code>, <b></b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/bash/98" target="_blank">bash/98</b></i></a></code>
</ul>
<br>
<h2>4. Collaboration: be up to date</h2>
<p>Of course, you can also work on the same branch as your co-workers and it&rsquo;s best if you keep up to date with their changes.</p>
<p>For this task &ndash;&nbsp;<strong>and only for this task</strong> &ndash; please update your file&nbsp;<code>README.md</code> in the main branch from GitHub.com. It&rsquo;s the&nbsp;<strong>only time</strong> you are allowed to update and commit from GitHub interface.</p>
<p>After you have done that, in your terminal:</p>
<ul>
    <li>Get all changes of the main branch locally (i.e. your&nbsp;<code>README.md</code> file will be updated)</li>
    <li>Create a new file&nbsp;<code>up_to_date</code> at the root of your directory and in it, write the git command line used</li>
    <li>Add&nbsp;<code>up_to_date</code> to git, commit (message: &ldquo;How to be up to date in git&rdquo;), and push to the origin</li>
</ul>
<ul>
    <li><b>Files:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/README.md" target="_blank">README.md</b></i></a></code>, <b></b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/up_to_date" target="_blank">up_to_date</b></i></a></code>
</ul>
<br>
<h2>5. HAAA what did you do???</h2>
<p><b><i>Advanced task</i></b><p>
<p>Collaboration is cool, but not really when you update the same file at the same time&hellip;</p>
<p>To illustrate that, please merge the branch&nbsp;<code>update_script</code> to&nbsp;<code>main</code>: &ldquo;Cool, all my changes will be now part of the main branch, ready to be deployed!&rdquo;</p>
<p><strong>HHHHHHHAAAAAAAA</strong></p>
<pre><code>CONFLICT (content): Merge conflict in bash/best
</code></pre>
<p>As you can see, you have conflicts between two branches on the same file.</p>
<p>Your goal now is to resolve conflicts by using the version of the branch&nbsp;<code>update_script</code>, and push the result to the origin.</p>
<p>At the end, you should have all your work from the branch&nbsp;<code>update_script</code> (new file and two updated files) and all latest&nbsp;<code>main</code> commits (new files, delete folder, etc.),&nbsp;<em>without</em> conflicts.</p>
<br>
<h2>6. Never push too much</h2>
<p>Create a&nbsp;<code>.gitignore</code> file and define a rule to never push&nbsp;<code>~</code> files (generated by Emacs).&nbsp;<a href="https://intranet.hbtn.io/rltoken/0ANsyvhObT_TYAToY8-lbA" target="_blank" title="Tips">Tips</a> </p>
<ul>
    <li><b>File:</b>&nbsp;<code><i><b><a href="https://github.com/FranRM15/zero_day/blob/main/0x03-git/.gitignore" target="_blank">.gitignore</b></i></a></code></li>
</ul>
<br>
<h2>License & Copyright</h2>
<i>©. Project provided by: <a href="https://www.holbertonschool.com/" target="_blank"><b>Holberton School</a></i></b>
<br>
<i>©. Project developed by:<b> Francisco Ramírez </b><b>|&nbsp;<a href="https://github.com/FranRM15" target="_blank"> GitHub</a> <b>|</b>&nbsp;<a href="https://twitter.com/FranciscoR_15" target = "_blank" rel="nofollow"> Twitter</b></a></p>
