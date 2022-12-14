---
keywords: fastai
description: Page to show basic python skills learned in Week 1.
title: Python Basics(Week 1)
toc: true 
badges: true
comments: true
categories: [jupyter, csp, week1, python]
image: images/python.png
nb_path: _notebooks/2022-08-23-python-week1.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-23-python-week1.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Basic-Function">Basic Function<a class="anchor-link" href="#Basic-Function"> </a></h1><p>Printing the famous "Hello world" statement.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span> <span class="p">(</span><span class="s2">&quot;Hello world&quot;</span><span class="p">)</span> <span class="c1"># This is a comment. Allows one to explain their work.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello world
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Running-quiz.py">Running quiz.py<a class="anchor-link" href="#Running-quiz.py"> </a></h1><p>Using the given code from the APCSP website and running the code.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">getpass</span><span class="o">,</span> <span class="nn">sys</span>

<span class="k">def</span> <span class="nf">question_and_answer</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer: &quot;</span> <span class="o">+</span> <span class="n">msg</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">question_with_response</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span>
    <span class="k">return</span> <span class="n">msg</span>

<span class="n">questions</span> <span class="o">=</span> <span class="mi">3</span>
<span class="n">correct</span> <span class="o">=</span> <span class="mi">0</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Hello, &#39;</span> <span class="o">+</span> <span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; running &quot;</span> <span class="o">+</span> <span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You will be asked &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; questions.&quot;</span><span class="p">)</span>
<span class="n">question_and_answer</span><span class="p">(</span><span class="s2">&quot;Are you ready to take a test?&quot;</span><span class="p">)</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What command is used to include other functions that were previously developed?&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="s2">&quot;import&quot;</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What command is used to evaluate correct or incorrect response in this example?&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="s2">&quot;if&quot;</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;Each &#39;if&#39; command contains an &#39;_________&#39; to determine a true or false condition?&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="s2">&quot;expression&quot;</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; you scored &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">correct</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello, poonam running /opt/anaconda3/bin/python
You will be asked 3 questions.
Question: Are you ready to take a test?
Answer: Yes!
Question: What command is used to include other functions that were previously developed?
import is correct!
Question: What command is used to evaluate correct or incorrect response in this example?
if is correct!
Question: Each &#39;if&#39; command contains an &#39;_________&#39; to determine a true or false condition?
expression is correct!
poonam you scored 3/3
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="My-Quiz">My Quiz<a class="anchor-link" href="#My-Quiz"> </a></h1><p>The quiz which I have created, based on the functions learned in the lesson. Takes advantage of str() to convert floats(numbers) to strings. The use of .lower() also helps to make sure any capitalization configuration of the answer will be marked as correct.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">getpass</span><span class="o">,</span> <span class="nn">sys</span><span class="o">,</span> <span class="nn">math</span> <span class="c1"># Getting necessary libraries to run the code.</span>

<span class="c1"># Function with question and response structure.</span>
<span class="k">def</span> <span class="nf">question</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span> 
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span> <span class="c1"># Prints question in clear way.</span>
    <span class="n">respond</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span> <span class="c1"># Gets an answer for the question from the user.</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer: &quot;</span> <span class="o">+</span> <span class="n">respond</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">respond</span> <span class="c1"># Important to return.</span>

<span class="c1"># Creating a list for the questions</span>
<span class="n">list_question</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;What do you call multiple lines of code?&quot;</span><span class="p">,</span> 
<span class="s2">&quot;How do you get a message from the user?&quot;</span><span class="p">,</span> 
<span class="s2">&quot;Are numbers a string? Yes or No&quot;</span><span class="p">,</span> 
<span class="s2">&quot;What does a function take in?&quot;</span><span class="p">,</span> 
<span class="s2">&quot;If the if portion of a code is not met, what runs?&quot;</span><span class="p">]</span>

<span class="c1"># Creating a list for the answers</span>
<span class="n">answer_key</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;sequence&quot;</span><span class="p">,</span> <span class="s2">&quot;input&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;parameter&quot;</span><span class="p">,</span> <span class="s2">&quot;else&quot;</span><span class="p">]</span>

<span class="c1"># Variables</span>
<span class="n">question_count</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">list_question</span><span class="p">)</span> <span class="c1"># In this case, question_count = 5, which is the number of indexes in the list</span>
<span class="n">score</span> <span class="o">=</span> <span class="mi">0</span> <span class="c1"># Running score on quiz.</span>

<span class="c1"># Greeting</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Hello, &#39;</span> <span class="o">+</span> <span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;.&quot;</span><span class="p">)</span> 
<span class="n">question</span><span class="p">(</span><span class="s2">&quot;How has your day been?&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;I hope this quiz brightens your day.&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You will answer &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">question_count</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; quiz questions.&quot;</span><span class="p">)</span>

<span class="c1"># For loop to repeat</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">list_question</span><span class="p">)):</span> <span class="c1"># for each i in the range of the question list</span>
    <span class="n">response</span> <span class="o">=</span> <span class="n">question</span><span class="p">(</span><span class="n">list_question</span><span class="p">[</span><span class="n">i</span><span class="p">])</span> <span class="c1"># using the defined function</span>
    <span class="n">check</span> <span class="o">=</span> <span class="n">answer_key</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="c1"># variable for the answer</span>
    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="n">check</span><span class="p">:</span> <span class="c1"># .lower() helps account for capitalization</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Correct!&quot;</span><span class="p">)</span>
        <span class="n">score</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># Add one to score</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Incorrect.&quot;</span><span class="p">)</span>



<span class="c1"># Function for finding percent.</span>
<span class="k">def</span> <span class="nf">grade</span><span class="p">(</span><span class="n">sco</span><span class="p">,</span> <span class="n">quests</span><span class="p">):</span> 
    <span class="n">percent</span> <span class="o">=</span> <span class="mi">100</span> <span class="o">*</span> <span class="nb">float</span><span class="p">(</span><span class="n">sco</span><span class="p">)</span><span class="o">/</span><span class="nb">float</span><span class="p">(</span><span class="n">quests</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">percent</span>

<span class="n">quiz_percentage</span> <span class="o">=</span> <span class="n">grade</span><span class="p">(</span><span class="n">score</span><span class="p">,</span> <span class="n">question_count</span><span class="p">)</span> <span class="c1"># Defining variable</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You got &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">score</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; of &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">question_count</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; questions correct.&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Your score is &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">quiz_percentage</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;%.&quot;</span><span class="p">)</span> <span class="c1"># Final print statement with score, as a percentage.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello, poonam.
Question: How has your day been?
Answer: Great!
I hope this quiz brightens your day.
You will answer 5 quiz questions.
Question: What do you call multiple lines of code?
Answer: SEQUEnce
Correct!
Question: How do you get a message from the user?
Answer: ask
Incorrect.
Question: Are numbers a string? Yes or No
Answer: NO
Correct!
Question: What does a function take in?
Answer: parameter
Correct!
Question: If the if portion of a code is not met, what runs?
Answer: else
Correct!
You got 4 of 5 questions correct.
Your score is 80.0%.
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Running the quiz, we can see it can correctly see if the user types in the right answer or not. Additionally, the code correctly grades the quiz, giving both the number of questions correct and the percentage. Using the for command helps to reduce the amount of code in the program, and the use of lists helps to make this code more adaptable to changes in the question and answer list.</p>

</div>
</div>
</div>
</div>
 

