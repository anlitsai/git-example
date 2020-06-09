# git-example
this is a git example

## SSH connection
git@github.com:anlitsai/gasp.git  

### or create a new repository on the command line  

echo "# gasp" >> README.md  
git init  
git add README.md  
git commit -m "first commit"  
git remote add origin git@github.com:anlitsai/gasp.git  
git push -u origin master  

### or push an existing repository from the command line  

#gitpush.sh $name $comment
#$name is the name of the repository, $comment is commit message
name='gasp'
datetime=`date +%Y%m%d-%H%M`
comment='update_'$datetime

git status  
git add .  
echo "git commit -m $comment"
git commit -m $comment
git status  
git remote add origin git@github.com:anlitsai/gasp.git  
git push -u origin master  


### or import code from another repository  

You can initialize this repository with code from a Subversion, Mercurial, or TFS project.  


## https connection:
https://github.com/anlitsai/gasp.git  

### or create a new repository on the command line  

name='gasp'
#gitinit $name
#$name is the name of the repository

rm -rf .git/
git init  
git remote add origin git@github.com:anlitsai/$name.git
git status
git add .
git commit -m "first commit"  
git status
git push -u origin master  

### or push an existing repository from the command line  

git remote add origin https://github.com/anlitsai/gasp.git  
git push -u origin master  

### or import code from another repository  

You can initialize this repository with code from a Subversion, Mercurial, or TFS project.  
