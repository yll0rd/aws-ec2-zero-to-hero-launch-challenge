
LEVEL 6: Instance Lifecycle Management
Objective: Control your EC2 instance states.

🔄 Perform These Actions
From the EC2 Console:
1. Stop Instance

Select instance → Instance State → Stop
Wait until state = Stopped
Note the Public IP

2. Start Instance

Instance State → Start
Wait until state = Running
Compare the new Public IP

3. Reboot Instance

Instance State → Reboot
Check if Public IP changed

4. Check EBS Data

SSH back into instance
Run: ls /mydata
Verify your test file still exists


📝 Answer These Questions
Create lifecycle-observations.txt:
1. What happened to the Public IP when you stopped/started?
Answer: _______________________________________________

2. What happened to the Public IP when you rebooted?
Answer: _______________________________________________

3. Did your EBS volume data remain after stop/start?
Answer: _______________________________________________

4. What's the difference between Stop and Terminate?
Answer: _______________________________________________
_______________________________________________

📸 Required Screenshots
Save in this folder:

01-instance-running.png

Instance running with original Public IP


02-instance-stopped.png

Instance in stopped state


03-instance-started-new-ip.png

Instance running again with new Public IP highlighted


04-ebs-data-persisted.png

Terminal showing /mydata contents still exist




🔑 Quick Reference
Action    Instance     Data     IP        Cost
Stop      Paused✅    Kept❌  Changes    EBS only
Reboot    Restarts✅  Kept✅  Same       Full
Terminate ❌Deleted❌ Lost*❌ Gone       $0
*Unless EBS "Delete on Termination" is disabled

⚠️ Important
DO NOT terminate your instance yet! You still need it for Level 7.

📤 Submission
bashgit add level-6-lifecycle/
git commit -m "Complete Level 6: Lifecycle Management"
git push origin main

✅ Completion

 Stopped and started instance
 Rebooted instance
 IP behavior documented
 EBS persistence verified
 4 questions answered
 4 screenshots saved
 Files committed

🏆 Badge Earned: 🟩 Lifecycle Commander
Next: Level 7 →
