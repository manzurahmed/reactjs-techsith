# React Routing

## 1. Introduction to section

এই পর্ব ReactJS এ Routing কিভাবে কাজ করে সে সম্পর্কে বিস্তারিত আলোচনা করা হয়েছে। আমাদের কন্টাক্ট এ্যাপটি লক্ষ্য করলে দেখবেন যে, এখানে সব কিছু এক পেজে নিয়ে এ্যাপ বানানো হয়েছে।

About পেজে কোন কিছু দেয়া হয়নি। About লিংকে ক্লিক করলে About পেজের কন্টেন্ট দেখাবে। এই যে, request এর ভিত্তি করে কোন কন্টেন্ট লোড করতে হবে, সেই ডিশিসন মেকিং টাস্কটার দায়িত্ব নিয়েছে ReactJS এর Routing বাবাজি।



## 2. Client vs Server side Routing

**Server-side routing**

![Server-side Routing](https://github.com/manzurahmed/reactjs/blob/master/server-side-routing.jpg)

এই ক্ষেত্রে ইউজার ওয়েবসাইট/এ্যাপ ব্রাউজ করার জন্য example.com ওয়েবসাইটে রিকুয়েস্ট পাঠালে, রিকুয়েস্টটা সার্ভারে পৌঁছাবে এবং URL এর উপরে ভিত্তি করে প্রয়োজনীয় প্রসেসিং শেষে request টা পুনরায় ব্রাউজারে পাঠাবে।

আবার, example.com/about URL এ রিকুয়েস্ট পাঠাবে তখন আবারও সার্ভার থেকে প্রয়োজনীয় ডাটা ব্রাউজারের কাছে ফেরত পাঠাবে যেটা ইউজার দেখতে পারবেন।

উভয় ক্ষেত্রেই ব্রাউজারের পেজটা Reload হয়ে নতুন কন্টেন্ট দেখা যাবে।

**Client-side routing**

![Client-side Routing](https://github.com/manzurahmed/reactjs/blob/master/client-side-routing.jpg)

একটা উদাহরণ দিয়ে Client-side routing টা বুঝানো হয়েছে। যদি আমরা https://reactjs.org ওয়েবসাইট ব্রাউজ করি, তাহলে খেয়াল করে দেখা যাবে যে, এর হোম পেজ ব্রাউজ করার সময় রিকুয়েস্টটা সার্ভারে যাচ্ছে এবং পুরো সাইটের কন্টেন্টসহ ব্রাউজারে অর্থাৎ ক্লায়েন্টের কাছে পাঠিয়ে দেয়া হচ্ছে। অর্থাৎ ক্লায়েন্ট সাইডে রিয়াক্টজেএস সাইটের কন্টেন্টকে cache করে রাখা হচ্ছে।

পরবর্তীতে যখন অন্যান্য লিংকে ক্লিক করলে, ঐ লিংকের কন্টেন্টের জন্য আর সার্ভার পর্যন্ত যেতে হচ্ছে না, বরং, ক্লায়েন্ট সাইডে ক্যাশে হয়ে থাকা কন্টেন্ট থেকে দেখানো হচ্ছে। এইটাই হল, Client-side routing এর সুবিধা।

## 3. Introduction to React-router-dom use

কোর ReactJS Library এর মধ্যে Routing যুক্ত করা নাই। একে npm এর মাধ্যমে প্রজেক্টের সাথে যুক্ত করে নিতে হয়।

জনপ্রিয় দু'টি রাউটিং প্যাকেজের নাম react-router-dom এবং reach-router.

https://www.npmjs.com/package/react-router-dom 

https://www.npmjs.com/package/@reach/router

https://reacttraining.com/react-router/web/guides/quick-start
https://reach.tech/router

শুরুতেই react-router-dom ইন্সটল করে নিব। রাউটিং সম্পর্কে বিস্তারিত জানতে reacttraining.com এর ডকুমেন্টেশন পড়তে হবে।

```
yarn add react-router-dom
```

Routing এর ৩টি মেইন কম্পোনেন্ট হল, BrowserRouter,Router, এবং, Link

## 4. Where to use render in Routing

## 5. Continue to working with Routing

## 6. Loading NotFound Page

## 7. Working with Link and NavLink component

## 8. Working with Link continued

## 9. Little Organization