---

title: Crafting RubyBench &#35;2 - GSoC summary 
date: 2017-08-22 07:54 UTC
tags: 

---

This blog post should serve as a recap of my contributions on RubyBench project during <a href="https://summerofcode.withgoogle.com/projects/#5251786557358080"> Google Summer of Code 2017</a>.

<h4>Project goal</h4>

Main goal was to create comparison chart which would be used to measure framework overhead. We needed something to tell us how much overhead ORM libraries such as ActiveRecord or Sequel brings by comparing them with raw SQL queries directly through ruby database adapter (mysql2, pg). On the other hand, comparing overhead between ActiveRecord and Sequel can help us decide which one to use in our stack.


<h4>Work done</h4>

<h5>Comparison chart</h5>

Main goal has been accomplished - you are now able to compare results on RubyBench. I have used HighStock multiseries feature to get this nice visualization.
<img src="images/comparison-chart.png">

<h6>Code</h6>

https://github.com/ruby-bench/ruby-bench-web/pull/199 <br>
https://github.com/ruby-bench/ruby-bench-web/pull/202 <br>
https://github.com/ruby-bench/ruby-bench-web/pull/203 <br>
https://github.com/ruby-bench/ruby-bench-web/commit/9bb7b392d7bed6c7866293e25d73165b2cb42ace <br>
https://github.com/ruby-bench/ruby-bench-web/pull/216 <br>
https://github.com/ruby-bench/ruby-bench-web/pull/231 <br>

<h5>Suite for pg gem</h5>

<h6>Code</h6>

https://github.com/ruby-bench/ruby-bench-web/pull/243 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/35 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/36 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/37 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/38 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/43 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/44 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/45 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/76 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/92 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/94 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/102 <br>

<h5>Admin UI</h5>
This was needed for some time for convenience. If you want to run suite for number of commits, you can do it through admin UI.

<h6>Code</h6>

https://github.com/ruby-bench/ruby-bench-web/pull/210 <br>
https://github.com/ruby-bench/ruby-bench-web/pull/227 <br>
https://github.com/ruby-bench/ruby-bench-web/pull/234 <br>

<h5>Storing logs on runner server</h5>

<h6>Code</h6>

https://github.com/ruby-bench/ruby-bench-web/commit/9bb7b392d7bed6c7866293e25d73165b2cb42ace <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/25 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/26 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/27 <br>

<h5>Fixed broken Rails suite</h5>

<h6>Code</h6>

https://github.com/ruby-bench/ruby-bench-docker/pull/28 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/29 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/30 <br>
https://github.com/ruby-bench/ruby-bench-docker/pull/31 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/84 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/89 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/90 <br>

<h5>Other</h5>

https://github.com/ruby-bench/ruby-bench-suite/pull/78 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/79 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/81 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/83 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/85 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/86 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/88 <br>
https://github.com/ruby-bench/ruby-bench-suite/pull/100 <br>
