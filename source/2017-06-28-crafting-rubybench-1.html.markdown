---

title: Crafting RubyBench &#35;1
date: 2017-06-28 18:22 UTC
tags:

---

Recently I have started contributing to Ruby Bench project.
I wrote a few words about it in my <a target="_blank" href="/2017/05/28/getting-into-open-source/">previous post</a>.

In this post I want to summarize contributions I've made during last month.

<h4>Sequel benchmarks</h4>
Finally we have Sequel benchmarks set up and running. Some results are already <a target="_blank" href="https://rubybench.org/jeremyevans/sequel/commits?result_type=sequel/mysql2_scope_all&display_count=2000">onsite</a>. Last year GSoC student got most of work done here, I was happy to finish it up and make it onsite.

<h4>Comparing results between libraries</h4>
So far you could have tracked performance of various libraries and platforms present on Ruby Bench.
Though you couldn't tell which one performs better or even how changing library dependencies affect its performance.
Being able to compare performance between ORM libraries can be useful when deciding which one to use in your stack.
How much performance is left on table when using one? You may want to take that insight into account.

Following are some comparison highlights :
<ul>
  <li>
    <a target="_blank" href="https://rubybench.org/rails/rails/commits?result_type=activerecord/mysql2_scope_all&display_count=200&compare_with=activerecord/postgres_scope_all">ActiveRecord and Sequel performs better with postgres.</a>
  </li>
  <li>
    <a target="_blank" href="https://rubybench.org/rails/rails/commits?result_type=activerecord/mysql2_scope_all&display_count=20&compare_with=sequel/mysql2_scope_all">Sequel performs generally faster than ActiveRecord.</a>
  </li>
</ul>

Further we need some comparison insight how much performance is being left on table. Therefore we need to have these benchmarks running against raw <a target="_blank" href="https://github.com/brianmario/mysql2">mysql</a> and <a target="_blank" href="https://github.com/ged/ruby-pg">pg</a> gems. Maybe ruby implementation comparisons would be interesting to see?

<h4>Other contributions</h4>
During last month I've made number of other smaller contributions.
<ul>
  <li><a href="https://github.com/ruby-bench/ruby-bench-web/issues/193" target="_blank">Fixed</a> Rails benchmarks which were broken for some time.</li>
  <li>We can now run benchmark suite <a href="https://github.com/ruby-bench/ruby-bench-web/pull/210" target="_blank">manually</a> for number of last commits.</li>
</ul>
<h4>Next steps</h4>
As Sam Saffron <a href="https://community.rubybench.org/t/how-can-active-record-be-faster/142/11" target="_blank">suggested</a>, we need to make our benchmarks more honest and put them in order. Next step is to add <i>real world</i> bench. Here's <a href="https://github.com/ruby-bench/ruby-bench-suite/pull/88" target="_blank">WIP</a> regarding this.
