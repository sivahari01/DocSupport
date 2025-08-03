💡 Little’s Law – Pacing Formula



👥 Number of Users = 🔁 Iterations per Second × (⏱️ E2E Response Time + 🧠 Total Think Time + ⏳ Pacing Delay)


🔄 TPM (Transactions per Minute) = 🔁 Iterations per Second × 60

⏱️ E2E (End-to-End) Response Time is the total time taken to complete one full iteration of your performance test script — from the start of the first transaction to the end of the last one — excluding think time and pacing.

👥 Number of Users – Total concurrent virtual users

🔁 Iterations per Second – Load (TPS or IPS)

⏱️ E2E Response Time – How long one iteration takes

🧠 Think Time – Pause time between transactions

⏳ Pacing Delay – Delay between iterations


💡 What is E2E Response Time?
⏱️ E2E (End-to-End) Response Time is the total time taken to complete one full iteration of your performance test script — from the start of the first transaction to the end of the last one — excluding think time and pacing.

✅ E2E Response Time = Sum of all Transaction Response Times (excluding Think Time)
🧮 How to Calculate It (Step-by-Step):
Identify all business transactions in one iteration
(e.g., Login → Search → Add to Cart → Logout)

Measure individual response times for each transaction from your test results or APM tool

Add all transaction response times together

📌 Example:
Transaction	Response Time (sec)
Login	1.5
Search Product	2.2
Add to Cart	1.3
Checkout	2.5
Logout	1.0

Total E2E Response Time = 1.5 + 2.2 + 1.3 + 2.5 + 1.0 = 8.5 seconds

🧠 Do not include:

Think Time

Pacing Delay



Let’s say:

🎯 Target TPM = 600

⏱️ Response Time = 3s

🧠 Think Time = 2s

⏳ Pacing Delay = 5s

👉 TPS = 600 ÷ 60 = 10 TPS

👥 Users = 10 × (3 + 2 + 5) = 10 × 10 = 100 Users
