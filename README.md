# 🐾 Wildlife Conservation Monitoring - PostgreSQL Assignment

### ১. PostgreSQL কী?

PostgreSQL হল একটি শক্তিশালী, ওপেন-সোর্স রিলেশনাল ডাটাবেস ম্যানেজমেন্ট সিস্টেম (RDBMS) যা ডাটা সংরক্ষণ, পুনরুদ্ধার এবং পরিচালনার জন্য ব্যবহৃত হয়। এটি SQL স্ট্যান্ডার্ড মেনে চলে এবং উন্নত ফিচার যেমন ট্রানজ্যাকশন, ফরেন কী, কনকারেন্সি কন্ট্রোল, এবং ইনডেক্সিং সমর্থন করে।


---

### ২. PostgreSQL-এ ডাটাবেস স্কিমার উদ্দেশ্য কী?

ডাটাবেস স্কিমা হল ডাটাবেসের গঠন বা ব্লুপ্রিন্ট, যা টেবিল, কলাম, ডাটা টাইপ, কনস্ট্রেইন্ট এবং তাদের মধ্যে সম্পর্ক নির্ধারণ করে। PostgreSQL-এ স্কিমা ডাটাকে সংগঠিতভাবে সংরক্ষণ করতে এবং অ্যাক্সেস নিয়ন্ত্রণ করতে সাহায্য করে।


---

### ৩. PostgreSQL-এ প্রাইমারি কী এবং ফরেন কী কনসেপ্ট ব্যাখ্যা করুন।

**প্রাইমারি কী**: একটি টেবিলের এমন একটি কলাম বা কলামের সমষ্টি যা প্রতিটি রোকে অনন্যভাবে চিহ্নিত করে। এটি `NOT NULL` এবং `UNIQUE` কনস্ট্রেইন্ট মেনে চলে।


**ফরেন কী**: একটি টেবিলের এমন একটি কলাম যা অন্য টেবিলের প্রাইমারি কী-এর সাথে সম্পর্ক স্থাপন করে এবং ডাটার রিলেশনাল অখণ্ডতা নিশ্চিত করে।


---

### ৪. VARCHAR এবং CHAR ডাটা টাইপের মধ্যে পার্থক্য কী?

| বৈশিষ্ট্য | VARCHAR | CHAR |
|-----------|---------|------|
| দৈর্ঘ্য | পরিবর্তনশীল | নির্দিষ্ট |
| স্টোরেজ | শুধুমাত্র প্রকৃত ডাটার জন্য | নির্দিষ্ট স্পেস সংরক্ষিত |
| ব্যবহার | সাধারণত ফ্লেক্সিবল ইনপুট | নির্দিষ্ট দৈর্ঘ্যের ইনপুটের জন্য উপযুক্ত |


---

### ৫. SELECT স্টেটমেন্টে WHERE ক্লজের উদ্দেশ্য কী?

`WHERE` ক্লজ ব্যবহার করা হয় একটি SELECT স্টেটমেন্টে নির্দিষ্ট শর্ত পূরণকারী রো ফিল্টার করার জন্য। এটি ডাটাবেস থেকে প্রাসঙ্গিক ডাটা পুনরুদ্ধার করতে সাহায্য করে।

> উদাহরণ:  
```sql
SELECT * FROM results WHERE location LIKE '%Pass%';
