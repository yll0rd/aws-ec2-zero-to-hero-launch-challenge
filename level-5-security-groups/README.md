## LEVEL 5: Security Group Deep Dive

**Objective:** Master cloud firewalls through experimentation.

---

### 🔬 Experiment

### Test 1: Remove HTTP Access

1. **Open the [AWS EC2 Console](https://us-east-1.console.aws.amazon.com/ec2/home?#Home:)** and go to **Security Groups**.  
2. Find and click on the security group named **zth-security-group**.  
3. Click on the **Inbound Rules** tab, then click **Edit**.  
4. Find the rule that allows **HTTP (port 80)** traffic and delete it.  
5. Save your changes.  
6. Now, try to open your website by entering `http://<Your-IP>` in your browser.  
7. Notice what happens — does the page load or not?.


### Test 2: Restore HTTP Access

1. Go back to the **Inbound Rules** of the **zth-security-group** and click **Edit** again.  
2. Add a new rule:  
   - **Type:** HTTP  
   - **Port:** 80 (this will be set automatically)  
   - **Source:** Anywhere (0.0.0.0/0)  
3. Save the rule.  
4. Refresh your browser and visit `http://<Your-IP>` again.  
5. Observe what happens now.

---

### ✍️ Write Your Explanation

Create a file named `security-group-explanation.txt` and answer:

**What are Security Groups?**  
Line 1: _______________________________________________  
Line 2: _______________________________________________  

**What I learned from the experiment:**  
_______________________________________________  
_______________________________________________  

---

### 📸 Required Screenshots

Save these screenshots in your project folder:

- **01-rules-with-http.png**  
  Security group showing HTTP rule enabled

- **02-rules-without-http.png**  
  Security group with HTTP rule removed

- **03-browser-blocked.png**  
  Browser unable to connect (HTTP rule removed)

- **04-browser-working.png**  
  Browser working again (HTTP rule restored)

---

### 📋 Final Security Group Rules

Make sure your **zth-security-group** has these inbound rules:

- **SSH (port 22)** from your IP address only  
- **HTTP (port 80)** from anywhere (`0.0.0.0/0`)

---

### 📤 Submission

```bash
git add level-5-security-groups/
git commit -m "Complete Level 5: Security Groups"
git push origin main
```

---

### ✅ Completion Checklist

- [ ] HTTP rule tested (removed and restored)  
- [ ] Explanation written in `security-group-explanation.txt`  
- [ ] 4 screenshots saved  
- [ ] Files committed  

---

Fill out this form to get your badge: https://forms.gle/Bx3xD4rck9qfxNLr7

**Next:** → [Level 6](../level-6-lifecycle/README.md)
