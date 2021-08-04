# **Git**

### What is git 

* Basically git is an open source distributed version control system.
* It is designed to handle minor to major projects with high speed and efficiency.
* It is developed to coordinate the work among the developers


### To create a file in git Repository
> 
> ##### step 1 (Create a file )
> 
> * create folder (abc_git)
> 
> * cd folder (cd abc_git)
> 
> * git init .
> 
> * touch file (create new file ex. touch readme )
> 
> * cat > file_name (cat > readme )
> 
> * git status
> 
> #### step 2 (Add file to git)
> 
> * git add file_name
> 
> * git status
> 
> #### step 3 (commit file )
> 
> * git commit -m"added file"
> 
> * git show
> * git log
> 
> #### step 4 (To push the file to remote )
> 
> * git push origin master


#### some Highlighting points of Git 
> * In git Untracked files are shown in Red colour and
> Commited files are shown in green colour.
> * In git there are always 2 stages i.e Registeration or commit.
> * first we add the file and the commit the file.
> * Add converts unstaged files to staged files.
> * commit converts staged files to commited .
> * latest commit will always comes at the Top.
> * when we add something it is in green colour.
> * when we remove something it is in Red colour.
> * Commit history shows us at what point of time who made the changes.

 *In my words git has different branches just like a tree.git starts with a trunk and then all branches. That trunk is usually called as a 'Master' and tip of the Trunk is called as 'Head'
Trunk remains same and Tips changes.* 



## Git Commands



<table>
<thead>
	<tr>
		<th>command</th>
		<th>Used For</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>git init .</td>
		<td>turn current directory into empty repository.</td>
	</tr>
	<tr>
		<td>git add &lt;file_name/Dir_name&gt;</td>
		<td>add a file/dir to staging area/be tracked.</td>
	</tr>
	<tr>
		<td>git add .</td>
		<td>add all files that are not staged.</td>
	</tr>
	<tr>
		<td>git commit -m &lt;message_for_commit&gt;</td>
		<td>record changes of file to local repository</td>
	</tr>
	<tr>
		<td>git commit -a -m &lt;message_for_commit&gt;</td>
		<td>commit all the staged changes.</td>
	</tr>
	<tr>
		<td>git status</td>
		<td>return current state of working tree.</td>
	</tr>
	<tr>
		<td>git push &lt;remote_name&gt; &lt;branch_name&gt;</td>
		<td>send local commits to remote repository.</td>
	</tr>
	<tr>
		<td>git log</td>
		<td>commit history of repository.</td>
	</tr>
	<tr>
		<td>git remote add &lt;remote_name&gt; &lt;remote_repo_URL&gt;</td>
		<td>add remote repository.</td>
	</tr>
	<tr>
		<td>git clone &lt;remote_repo_URL&gt;</td>
		<td>to create local working copy of existing remote repository.</td>
	</tr>
	<tr>
		<td>git pull &lt;remote_name&gt; &lt;branch_name&gt;</td>
		<td>to get latest version of remote repository of specified branch. If many people make changes the our push may get rejected the use this command</td>
	</tr>
	<tr>
		<td>git branch &lt;branch_name&gt;</td>
		<td>create new branch</td>
	</tr>
	<tr>
		<td>git branch -D &lt;branch_name&gt;</td>
		<td>delete a branch</td>
	</tr>
	<tr>
		<td>git checkout &lt;branch_name&gt;</td>
		<td>switch to specified branch.</td>
	</tr>
	<tr>
		<td>git checkout -b &lt;new_branch_name&gt;</td>
		<td>checkout to and create specified branch.</td>
	</tr>
	<tr>
		<td>git switch &lt;branch_name&gt;</td>
		<td>switch to specified branch.</td>
	</tr>
	<tr>
		<td>git merge &lt;branch_name&gt;</td>
		<td>merge changes from specified branch into current branch.</td>
	</tr>
	<tr>
		<td>git show [commit_SHA]</td>
		<td>data and content changes of specified commit.</td>
	</tr>
</tbody>
</table>
