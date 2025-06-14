# ☁️ My AWS Learning Journey – Day 1

Hey there! 👋  
Today I officially started learning AWS and cloud computing. I’m documenting my learning here as simply and honestly as possible. I’m just getting started, so expect this to grow as I keep learning. 😊

---

## 🔥 What I Learned Today

### 🚀 1. What is EC2?
- EC2 stands for **Elastic Compute Cloud**.
- It basically helps us create **virtual servers** (not physical machines) in the cloud.
- We can choose how powerful we want the server to be — how much CPU, RAM, storage, etc.
- Think of EC2 as “renting a computer in the cloud” that you can access anytime.

---

### 🖥️ 2. What is a Server?
- A server is a system that **runs code, websites, apps**, etc.
- Normally, you’d need to buy and set one up — but with AWS, we can just create one in minutes.

---

### 🔐 3. AMI, SSH, and Session Manager?
- **AMI** = A pre-built OS + software image (like Windows or Ubuntu). We choose one while launching EC2.
- **SSH** = Way to log into the server using the command line.
- **Session Manager** = AWS tool that lets you connect to your EC2 instance directly from the browser — no need to worry about SSH keys. Also helps log who accessed what.

---

## 🧠 Understanding EC2 Pricing (Simple Cheatsheet)

| 💰 Model | What it Means | When to Use | Discount? |
|---------|----------------|--------------|------------|
| **On-Demand** | Pay per hour | Testing, short projects | ❌ No |
| **Reserved** | Commit to 1-3 years | Long-running apps | ✅ Up to 75% |
| **Spot** | Use spare servers | Temporary/cheap work | ✅ Up to 90% |
| **Dedicated Instance** | Server only for you | Security-sensitive apps | ❌ Expensive |
| **Dedicated Host** | You rent full physical server | Licensing/audits | ❌ Super costly |
| **Savings Plan** | Flexible savings model | Regular usage | ✅ Up to 72% |

I really liked how **Spot Instances** are super cheap, but can be stopped anytime. You get what you pay for. 😂

---

## 💳 Billing & Cost Tracking

- **AWS Free Tier** – Free EC2 hours monthly for new users (yay!).
- **Billing Dashboard** – Where you can see how much you’ve spent.
- **Cost Explorer** – Helps visualize what services cost you the most.
- **Budgets** – You can set spending limits so your bill doesn’t shock you at the end of the month.

---

## 📝 Summary (in my own words):
- EC2 lets us launch cloud servers.
- There are different pricing models — each has pros and cons.
- AWS gives tools to track your bill and avoid surprises.
- Session Manager is super beginner-friendly for connecting to servers.

---

## 📅 Up Next:
- Learn how S3 (cloud storage) works
- Understand networking basics in AWS (VPC, subnets, security groups)
- Try hands-on launching EC2 with a simple app

---

## Day 2 – AWS Billing & Cost Tools

# ☁️ AWS Learning Journey – Day 2

Hey everyone! 👋  
Today I focused on learning how AWS handles **billing, cost tracking, and account management**. These tools are super important if you're managing multiple AWS services or working in a company with many cloud accounts.

---

## 🛡️ AWS Trusted Advisor

This tool is like your **AWS account assistant** — it reviews your setup and gives suggestions to:
- 💰 Save money
- 🔐 Improve security
- 🚀 Boost performance
- 💣 Add fault tolerance
- 📈 Monitor service limits

🔍 Example: It might tell you “Hey, this EC2 instance is not being used — consider stopping it to save cost.”

> 📌 You get 7 basic checks for free. More checks if you're on Business/Enterprise support.

---

## 🧾 Consolidated Billing (via AWS Organizations)

This lets you link **multiple AWS accounts** under one **main payer account**.

### ✅ Why It’s Useful:
- 🧾 One bill for all linked accounts
- 🔍 Easy to track usage per team/project
- 💸 Combine usage across accounts to get **volume discounts**
- 🔒 Each account stays separate and secure

---

## 💸 Volume Discounts with Consolidated Billing

If Account A uses 20 TB of S3, and Account B uses 30 TB,  
➡️ Combined = 50 TB = Qualifies for cheaper storage pricing!

You save **more** because AWS sees your **total usage** across accounts.

> 🧠 Without consolidated billing, each account would miss out on the discount.

---

## 📊 AWS Cost Explorer

This is your **cloud spending dashboard** — super helpful.

### What You Can Do:
- View spending per day/month/service/account
- Filter by tags, regions, services
- Forecast future costs
- Compare usage over time
- Spot unexpected increases (like “Oops! I forgot to stop that instance 😅”)

> 🔍 This tool helps you stay in control of your AWS bill — even as you grow.

---

## ✅ Summary of Today:
| Tool | What it Helps With |
|------|---------------------|
| **Trusted Advisor** | Cost, security, performance tips |
| **Consolidated Billing** | Link multiple accounts, save money |
| **Volume Discounts** | Save more when usage is combined |
| **Cost Explorer** | Visualize, track & control spending |

---


Thanks again for reading!  
Feel free to fork this if you're also learning AWS 😊

— *Thrupthi S.*

