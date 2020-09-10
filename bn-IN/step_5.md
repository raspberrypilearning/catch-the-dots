## আরো বেশি কঠিন করুন

এখন আপনি গেমটিকে আরও বেশি কঠিন করে তুলছেন খেলোয়াড় যত দীর্ঘ সময় এটি খেলবে।. সময়ের সাথে সাথে বিন্দুগুলিকে দ্রুত এবং দ্রুত প্রদর্শিত করে আপনি এটি করবেন।.

--- task ---

Create a new `variable`{:class="block3variables"} called 'delay'.

![Stage sprite](images/stage-sprite.png)

--- /task ---

--- task ---

স্টেজের স্ক্রিপ্টস অঞ্চলে যান এবং একটি নতুন স্ক্রিপ্ট তৈরি করুন যা `delay`{:class="block3variables"} ভেরিয়েবল কে `8` এ সেট করে এবং তারপরে গেমটি চলাকালীন ধীরে ধীরে এর মান হ্রাস করে `delay`{:class="block3variables"}.

![Stage sprite](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

--- /task ---

লক্ষ্য করুন যে এই code টি আপনি একটি কাউন্টডাউন টাইমার তৈরি করতে যে code টি ব্যবহার করেছিলেন তার সাথে খুব মিল!

এরপরে, 'red', 'yellow', এবং 'blue' স্প্রাইটের কোড স্ক্রিপ্টগুলিতে `delay`{:class="block3variables"} ভেরিয়েবলটি ব্যবহার করুন।.

--- task ---

সেই code ব্লকটি সরিয়ে ফেলুন যেটি গেমটিকে ডট স্প্রাইট ক্লোন তৈরির মধ্যে কয়েক অনির্দিষ্ট সেকেন্ড অপেক্ষা করায়।. আপনি যে ব্লকটি মুছেছেন, সেটিকে আপনার নতুন `delay`{:class="block3variables"} ভেরিয়েবল দিয়ে প্রতিস্থাপন করুন:

![screenshot](images/all-dots.png)

```blocks3
-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

এটি সমস্ত তিনটি ডট স্প্রাইটের জন্য করুন।.

--- /task ---

--- task ---

গেমটি পরীক্ষা করুন এবং খেলা চলার সাথে সাথে ডটগুলি আরও দ্রুত প্রদর্শিত হতে শুরু করে কিনা তা পরীক্ষা করুন।.

+ এটি কি সমস্ত তিনটি রঙিন ডট এর জন্য কাজ করে?
+ আপনি কি যে `delay`{:class="block3variables"} ভেরিয়েবলের মান হ্রাস দেখতে পাচ্ছেন?

--- /task ---