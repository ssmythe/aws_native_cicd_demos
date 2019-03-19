# html_static_ec2
Note: Make sure you're in us-east-1 region

## Set up CodeStar project

1. Choose HTML / Static Website / Amazon EC2
2. Enter "html_static_ec2" in Project name field
3. Choose AWS CodeCommit for repository
4. Enter "html_static_ec2" in Repository name
5. Click "Next"
6. Make sure "AWS CodeStar would like permission to administer AWS resources on your behalf." is checked
7. Click "Create Project"
8. Choose existing key pair for Amazon EC2 Key Pair
9. Check acknowledgement
10. Click "Create Project"
11. Enter your name in "Display Name"
12. Enter your email in "Email"
13. Click "Next"
14. Choose "AWS Cloud9" for editor
15. Click "Next"
16. Choose t2.micro for EC2 instance type
17. Click "Next"

You'll be taken to the CodeStar dashboard for the project

Note: it takes about 10 minutes to set everything up

Once everthing is up and running...

## View sample website

1. Click URL listed in Application endpoints
2. See "Congratulations!" text

## Make a change

1. Navigate back to CodeStar dashboard
2. Click "Start Coding" to launch Cloud9 editor
3. Down in terminal section setup your git user.name and user.email configs
4. Open html_static_ec2 > webpage > index.html
5. Change line 61 text "Congratulations!" to "Hey, you just made a change!"

## Commit the change
In the terminal window...

1. git diff
2. git add .
3. git commit -m "Change h1 to made a change message"
4. git push

## Watch change deploy out

1. Navigate to CodeStar dashboard
2. See pipeline activate and start Source > Build > Deploy
3. Open Application endpoints URL
4. Periodically refresh endpoint page, and then switch back to dashboard, and back to page

## View pipeline history

1. Navigate to CodeStar dashboard
2. Click "Pipeline history" link
