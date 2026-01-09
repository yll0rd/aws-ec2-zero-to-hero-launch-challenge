 LEVEL 3: Install Software on Your EC2
Objective: Deploy a web server to the internet.

🌐 Install Apache
While connected via SSH:
bashsudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd

📄 Create Webpage
bashecho "Welcome to my Zero-to-Hero EC2 Challenge!" | sudo tee /var/www/html/index.html

🧪 Test in Browser
Visit: http://<Your-Public-IP>

⚠️ Page Not Loading? CRITICAL LESSON!
This is THE most important EC2 lesson:
Your server is running, but AWS is protecting it by default.
Fix: Add HTTP Rule

EC2 Console → Security Groups → zth-security-group
Inbound Rules → Edit
Add rule:

   Type: HTTP
   Port: 80
   Source: 0.0.0.0/0 (Anywhere-IPv4)

Save → Refresh browser

💡 Key Lesson: "Cloud isn't insecure. It's secure by default."

📸 Required Screenshots
Save in this folder:

01-apache-install.png

Terminal showing Apache installation


02-security-group-before.png

Security group rules BEFORE adding HTTP


03-security-group-after.png

Security group rules AFTER adding HTTP


04-webpage-working.png

Browser showing your custom message



Also create web-server-notes.txt:
Apache Install Status: Success/Failed
Security Group Rule Added: Yes/No
Webpage URL: http://_______________
Key Lesson Learned: _______________

📤 Submission
bashgit add level-3-install-software/
git commit -m "Complete Level 3: Deploy Web Server"
git push origin main

✅ Completion

 Apache installed
 Custom message displays
 HTTP rule added
 4 screenshots saved
 Notes file created
 Files committed

🏆 Badge Earned: 🟪 Cloud Developer
Next: Level 4 →
