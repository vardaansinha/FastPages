---
keywords: fastai
description: "A quiz on some of the most common Python commands and terminology."
title: "Python Quiz"
toc: true 
badges: true
comments: true
categories: [jupyter,python]
author: Vardaan Sinha
nb_path: _notebooks/2022-08-28-pythonquiz.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-28-pythonquiz.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">getpass</span><span class="o">,</span><span class="nn">sys</span>
<span class="c1"># The import command is used to import particular Python modules that involve certain sets of functions and variables that may be useful in a specific script.</span>
<span class="k">def</span> <span class="nf">question_answer</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span><span class="p">)</span>
    <span class="n">message</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer:&quot;</span> <span class="o">+</span><span class="n">message</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">response</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">message</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span> 
    <span class="k">return</span> <span class="n">message</span>   

<span class="n">integer</span> <span class="o">=</span> <span class="mi">3</span>
<span class="c1"># Here, what I did was that I defined the value of the integer. This needed to be done for the Bonus question.</span>
<span class="n">question_data</span> <span class="o">=</span> <span class="p">[</span>
    <span class="s2">&quot;What type of statement is used to evaluate an expression list?&quot;</span><span class="p">,</span>
    <span class="s2">&quot;What type of statement is used to return an expression list?&quot;</span><span class="p">,</span>
    <span class="s2">&quot;What type of statement is used to call other Python modules to utilize their functions?&quot;</span><span class="p">,</span>
    <span class="s2">&quot;BONUS: What is the name of the Python module used to utilize StackOverflow without leaving the terminal?&quot;</span>
<span class="p">]</span> 

<span class="n">answer_data</span> <span class="o">=</span> <span class="p">[</span>
    <span class="s2">&quot;expression&quot;</span><span class="p">,</span>
    <span class="s2">&quot;return&quot;</span><span class="p">,</span>
    <span class="s2">&quot;import&quot;</span><span class="p">,</span>
    <span class="s2">&quot;howdoi&quot;</span><span class="p">,</span>
<span class="p">]</span>

<span class="n">questions</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">question_data</span><span class="p">)</span>
<span class="n">correct</span> <span class="o">=</span> <span class="mi">0</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Hey skippy, &#39;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; questions.&quot;</span><span class="p">)</span>
<span class="n">resp</span> <span class="o">=</span> <span class="n">response</span><span class="p">(</span><span class="s2">&quot;Prepared? Say &#39;yes&#39; or &#39;no&#39;.&quot;</span><span class="p">)</span>

<span class="k">if</span> <span class="n">resp</span> <span class="o">==</span> <span class="s2">&quot;yes&quot;</span><span class="p">:</span>
    
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Let&#39;s start.&quot;</span><span class="p">)</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">question_data</span><span class="p">)):</span>
        <span class="n">resp</span> <span class="o">=</span> <span class="n">response</span><span class="p">(</span><span class="n">question_data</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>
        <span class="k">if</span> <span class="n">resp</span> <span class="o">==</span> <span class="n">answer_data</span><span class="p">[</span><span class="n">i</span><span class="p">]:</span>
            <span class="nb">print</span><span class="p">(</span><span class="n">resp</span> <span class="o">+</span> <span class="s2">&quot; is correct.&quot;</span><span class="p">)</span>
            <span class="n">correct</span> <span class="o">+=</span><span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="n">resp</span> <span class="o">+</span> <span class="s2">&quot; is wrong.&quot;</span><span class="p">)</span>
    
    
    <span class="nb">print</span> <span class="p">(</span><span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; you got a &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">correct</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">integer</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; or a &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">((</span><span class="n">correct</span> <span class="o">/</span> <span class="n">integer</span><span class="p">)</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;%&quot;</span><span class="p">)</span>

<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Leave.&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hey skippy, 4 questions.
Question: Prepared? Say &#39;yes&#39; or &#39;no&#39;.
Let&#39;s start.
Question: What type of statement is used to evaluate an expression list?
expression is correct.
Question: What type of statement is used to return an expression list?
return is correct.
Question: What type of statement is used to call other Python modules to utilize their functions?
import is correct.
Question: BONUS: What is the name of the Python module used to utilize StackOverflow without leaving the terminal?
howdoi is correct.
vardaan you got a 4/3 or a 133.33333333333331%
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Now, I'd like to talk about a caveat that I used in the code. As you can all see, I defined 'integer' as 3 at the start, even though there were 4 questions. This is because the 4th question was defined as a bonus question, and if someone got the bonus question right, they should get more than a 100%.</p>
<p>First, I tried without defining the integer value in the code and just adding the number 3 in the last print statement, but that did not work, as Python cannot concatenate an integer into a string value. Therefore, I had to define the integer as a string, and that made the print statement work without crashing at the end.</p>
<p>Thanks!</p>

</div>
</div>
</div>
</div>
 
