# 📅 Week 1 – Know Yourself

## 🎯 Objective
Understand my hacker mindset, complete initial tasks, and start practical learning.

---

## 🧬 My Hacker Archetype
The Scholar

Why I think this fits me:
- I need to understand before i touch anything.
- Takes time to implement things so that unexpected things may not happen.

---

## 🎮 Game Experience
- My approach to answering questions: It was very fast and I was in a hurry.
- Something that surprised me: That I am the Scholar rather than Breaker (Just 1 point difference).

---

## 💻 TryHackMe / Hack The Box
- Platform: TryHackMe
- Room Name: Hydra

### 🧠 What I Learned
- Hydra is a password brute-forcing tool used to crack login credentials.
- It supports multiple protocols like SSH, FTP, HTTP, etc.

### 📸 Proof
![Hydra Room Completion](./image.png)

---

## 🛠 Tool Deep Dive
Tool Name: ffuf (Fuzz Faster U Fool)

### 🔍 What it does
- ffuf is a web fuzzing tool used to discover hidden endpoints, parameters, and inputs in a web application. It helps identify parts of a system that are not directly visible by systematically testing different inputs.

### ⚙️ How it works
- ffuf works by replacing a placeholder keyword (commonly `FUZZ`) in a request with values from a wordlist. For each value, it sends an HTTP request to the target and analyzes the response.

It evaluates responses based on:
- Status codes (200, 403, 404)
- Response size
- Response content

This allows it to identify valid or interesting results from a large number of requests.

### 💻 Commands Used

#### 1. Basic Directory Fuzzing
```bash
ffuf -u http://target/FUZZ -w /path/to/wordlist.txt
```
#### 2. Parameter Fuzzing
```bash
ffuf -u "http://target/page?param=FUZZ" -w /path/to/wordlist.txt
```

#### 3. Filtering Responses
```bash
ffuf -u http://target/FUZZ -w wordlist.txt -fs 4242
```

### 🧪 My Experiment
I ran:
```bash
ffuf -u http://testphp.vulnweb.com/FUZZ -w common.txt
```
Output:-
![ffuz output](./image2.png)

### 🌍 Real-world usage
- Discover hidden directories and files (e.g., /admin, /backup)
- Identify valid parameters and inputs
- Test how applications handle unexpected or unknown inputs

### 💡 My Insight
I realized that ffuf is not just about brute-forcing directories, but about systematically testing inputs and analyzing differences in server responses to identify hidden functionality.
---

## 🤖 AI Learning
### ❓ Question I asked:
-

### 💡 What I understood:
-

---

## ⚠️ Challenges Faced
-
-

---

## 💡 How I Solved Them
-
-

---

## 🔍 Key Takeaways
-
-
-

---

## 🚀 Next Week Plan
-
-
