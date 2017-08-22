---

title: Crafting RubyBench &#35;2 - GSoC summary 
date: 2017-08-22 07:54 UTC
tags: 

---

This blog post should serve as a recap of my contributions on RubyBench project during <a href="https://summerofcode.withgoogle.com/projects/#5251786557358080"> Google Summer of Code 2017</a>.

<h4>Project goal</h4>

Main goal was to create comparison chart which would be used to measure framework overhead. We needed something to tell us how much overhead ORM libraries such as ActiveRecord or Sequel brings by comparing them with raw SQL queries directly through ruby database adapter (mysql2, pg). On the other hand, comparing overhead between ActiveRecord and Sequel can help us decide which one to use in our stack.


<h4>Work done</h4>
<img src="images/comparison-chart.png">

#####Comparison chart

