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






🎯 Goal: Achieve 1000 TPM
So,

✅ TPM = 1000

✅ TPS = TPM ÷ 60 = 1000 ÷ 60 = 16.67 TPS

🛍️ Scenario: E-Commerce "Place Order" Transaction
Steps in One Iteration:
Login

Search Product

View Product Details

Add to Cart

Checkout

Payment

Logout

🕒 Step 1: Assume E2E Response Time
Step	Response Time (sec)
Login	1.5
Search Product	2.0
View Product Details	1.0
Add to Cart	1.2
Checkout	2.0
Payment	2.3
Logout	1.0
Total	11.0 sec

✅ ⏱️ E2E Response Time = 11 seconds

🤔 Step 2: Assume Think Time
Let’s say the user pauses 2 seconds between each action.

Total think pauses between 7 steps = 6 pauses

🧠 Think Time = 6 × 2 = 12 seconds

🎯 Step 3: Calculate Pacing Delay
Let’s try a pacing delay of 7 seconds as a starting point.
So:

⏳ Pacing Delay = 7 seconds

📐 Step 4: Apply Little’s Law Formula
Number of Users 👥
=
TPS 🔁
×
(
E2E Time ⏱®
+
Think Time 🧠
+
Pacing Delay ⏳
)
Number of Users 👥=TPS 🔁×(E2E Time ⏱ 
R
◯
 +Think Time 🧠+Pacing Delay ⏳)
Users
=
16.67
×
(
11
+
12
+
7
)
=
16.67
×
30
=
500.1
≈
500
𝑈
𝑠
𝑒
𝑟
𝑠
Users=16.67×(11+12+7)=16.67×30=500.1≈500Users
✅ Final Answer:
Metric	Value
Target TPM	1000
TPS	16.67
E2E Response Time	11 sec
Total Think Time	12 sec
Pacing Delay	7 sec
Required Users	500
