<h1>0x03. Git</h1>
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
