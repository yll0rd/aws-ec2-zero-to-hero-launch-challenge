## LEVEL 7: Cost Optimization

**Objective:** Learn to avoid surprise AWS bills.

---

### 💰 Answer These Questions

Create a file named `cost-optimization-answers.txt` and answer:

1. **Why is t2.micro free tier eligible?**  
   Answer: _______________________________________________  
   _______________________________________________

2. **What's the difference between Stop vs Terminate?**  
   Answer: _______________________________________________  
   _______________________________________________

3. **When does EC2 cost money?**  
   Answer: _______________________________________________  
   _______________________________________________

4. **List 3 ways to avoid extra billing:**  
   a) _______________________________________________  
   b) _______________________________________________  
   c) _______________________________________________

---

### 🧾 Check Your AWS Bill

1. Open the **[AWS Console](https://us-east-1.console.aws.amazon.com/console/home) → Billing Dashboard**  
2. Review your **Month-to-Date charges**  
3. Check your **[Free Tier usage](https://us-east-1.console.aws.amazon.com/costmanagement/home#/freetier)**

Create a file named `billing-snapshot.txt` with:

```
Current Month-to-Date Charges: $_______
Free Tier EC2 Hours Used: _______/750
Free Tier EBS Storage Used: _______/30 GB
Any Unexpected Charges?: Yes/No
```

---

### 📸 Required Screenshots

Save these screenshots in your project folder:

- **01-billing-dashboard.png**  
  AWS Billing Dashboard overview

- **02-free-tier-usage.png**  
  Free Tier usage details

---

### 💡 Cost Saving Checklist

Before completing this challenge, make sure you:

- Understand free tier limits (750 hours/month)  
- Know that stopped instances still cost (EBS storage)  
- Know when to **Stop** vs **Terminate** instances  
- Have checked your billing dashboard  
- Are ready to terminate resources to avoid charges

---

### 🧹 Clean Up (FINAL STEP)

Now it’s time to terminate your resources to avoid charges:

1. Go to **EC2 Console → Select ZeroToHero-EC2**  
2. Click **Instance State → Terminate**  
3. Confirm termination  
4. Go to **Volumes → Delete** the 2GB EBS volume  
5. Go to **Security Groups** → decide to keep or delete **zth-security-group**  
6. Take a final screenshot: **03-resources-terminated.png**

---

### 📤 Submission

```bash
git add level-7-cost-optimization/
git commit -m "Complete Level 7: Cost Optimization - Challenge Complete!"
git push origin main
```

---

### ✅ Completion Checklist

- [ ] 4 questions answered  
- [ ] Billing dashboard checked  
- [ ] Understand Stop vs Terminate  
- [ ] 3 screenshots saved  
- [ ] Instance terminated  
- [ ] EBS volume deleted  
- [ ] Files committed  

---

## 🎉 CHALLENGE COMPLETE!

### 🎓 What You've Mastered

- ✅ Launch and configure EC2 instances  
- ✅ Connect via SSH  
- ✅ Install and deploy web servers  
- ✅ Manage EBS storage  
- ✅ Configure security groups  
- ✅ Control instance lifecycle  
- ✅ Optimize costs and avoid surprise bills  

---

### 🚀 Next Steps

- **AWS Certification:** Study for AWS Cloud Practitioner  
- **Expand Skills:** Learn S3, Lambda, RDS  
- **Build Projects:** Deploy your own applications  
- **Join Community:** Share your success on LinkedIn!

---

### 🎉 Share your completion:

> Just completed the Zero-to-Hero EC2 Challenge!  
> Learned: EC2, SSH, Apache, EBS, Security Groups, Cost Optimization  
> #AWS #CloudComputing #EC2 #DevOps
