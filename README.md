  Task
1. Read carefully all steps described below.

2. Create concept of working by drawing diagram (collaborate with your team)
Diagram can be created as in any specific tool as by drawing on a paper or dashboard (in second case just make a photo)

3. Clone the repo: https://github.com/MNT-Lab/git-tasks.git 
           
4. Create own branch locally by pattern (from master, can be done by one of team member):
(First char of name + surname of first student)-(First char of name + surname of second student)
Example: There are 2 students, Serhei Ivanou and Vasya Pupkin. The branch will be :
sivanou-vpupkin

5. Push the branch from local to remote

6. Change READ.me file with description of your project/team and created  diagram ( useful tip: gitlab  markdown language can be used to beatify formatting of text https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet )
Expected different commits here from each of team member. For example someone was working on description, someone – on pasting diagram.

7. Create Vagrantfile 

Vagrantfile should include:

Configuration of VM
Provisioning script:
1. Jenkins installed to folder /opt/jenkins/
2. Server should be run under ‘jenkins’ user and started from init script as service
3. JENKINS_HOME=/opt/jenkins/master
4. JENKINS_DIR=/opt/jenkins/bin  ( <- .war is here)
5. Closed by Nginx and available by link http://jenkins

Expected different commits here from each of team member. For example someone was working on init script, someone on VM configuration and etc.., every feature should be developed in own feature branch with opened pull request to team branch and merged to it at the end. 
