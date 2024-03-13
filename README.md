# Before Profiling and Performance Optimization

## JMeter GUI
![before_jmeter_gui_1.jpg](readme_img%2Fbefore_jmeter_gui_1.jpg)
![before_jmeter_gui_2.jpg](readme_img%2Fbefore_jmeter_gui_2.jpg)
![before_jmeter_gui_3.jpg](readme_img%2Fbefore_jmeter_gui_3.jpg)

## JMeter CLI
![before_jmeter_cli_1.jpg](readme_img%2Fbefore_jmeter_cli_1.jpg)
![before_jmeter_cli_2.jpg](readme_img%2Fbefore_jmeter_cli_2.jpg)
![before_jmeter_cli_3.jpg](readme_img%2Fbefore_jmeter_cli_3.jpg)

<hr>

# After Profiling and Performance Optimization

## JMeter GUI
![after_jmeter_gui_1.jpg](readme_img%2Fafter_jmeter_gui_1.jpg)
![after_jmeter_gui_2.jpg](readme_img%2Fafter_jmeter_gui_2.jpg)
![after_jmeter_gui_3.jpg](readme_img%2Fafter_jmeter_gui_3.jpg)

## JMeter CLI
![after_jmeter_cli_1.jpg](readme_img%2Fafter_jmeter_cli_1.jpg)
![after_jmeter_cli_2.jpg](readme_img%2Fafter_jmeter_cli_2.jpg)
![after_jmeter_cli_3.jpg](readme_img%2Fafter_jmeter_cli_3.jpg)

<hr>

# Reflection

#### 1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?

**Answer:**
Testing with JMeter is useful to evaluate the performance of web applications, databases, and servers under varying conditions and loads, but
it won't show what *causes* the application to perform as it does.

In contrast, profiling with IntelliJ Profiler can show an application's runtime behavior, memory usage, execution speed, and thread activity. Being able to see the runtime of individual methods helps to shed light on which part of the application
is slowing down the rest, which JMeter's performance testing on its own is unable to do.

<br>


#### 2. How does the profiling process help you in identifying and understanding the weak points in your application?

**Answer:**
The profiling process, specifically using IntelliJ Profiler, helps me identify the weak points in my application by showing which of my methods and processes are consuming excessive resources.
This helps me understand which parts of my code I should refactor and optimize.

<br>


#### 3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?

**Answer:**
Yes! Like previously stated, IntelliJ Profiler helps me see which parts of my code are dragging down the rest and which are using
more resources than necessary. Usually, these bottlenecks are methods (besides the main method) that rank high when seeing the CPU Time order in the Method List view of IntelliJ Profiler.

<br>


#### 4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?

**Answer:**
Personally, I'm still not very familiar with JMeter and when to use each Sampler and Listener. Throughout this module, I only really relied on the View Results in Table listener and nothing else.
I'm also quite unfamiliar with the many views in IntelliJ Profiler other than the method list. Even in the method list itself, I often find it hard to see what's causing performance problems since I have to scroll
down a *lot* of methods— most of which are imported methods/built-in methods that I never even wrote.

To overcome these challenges, I need to familiarize myself more with JMeter and IntelliJ Profiler and learn about shortcuts I could use to make using both these tools easier.

<br>


#### 5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?

**Answer:**
Using the IntelliJ Profiler helps me pinpoint problems in my code much quicker. Most importantly, it tells me what I should prioritize in refactoring, since some code smells need to be fixed asap due to causing performance issues while some others can be
fixed at a less urgent pace. It also helps me see if my refactoring actually worked by showing me the new running time after the changes are made.

<br>


#### 6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?

**Answer:**
Though I haven't encountered such a case, I would re-check whether or not it was caused by different testing conditions (hardware, network, etc) or if it was caused by a problem in how I set up my
JMeter and IntelliJ Profiler. There's the possibility that it's caused by extremely unstable code running time, but I would ask friends to do tests on their hardwares too to see if their findings were more consistent or if it really *was* caused by instability.

<br>


#### 7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?

**Answer:**
My main strategy of optimizing application code is by refactoring methods and code sections that cause bottlenecks in my application. In future projects, I would ensure it doesn't change the application's functionality by checking my tests, and also by limiting myself so I don't change too much of my code at a time.
Per refactoring, instead of remaking the parts of my application's structure, I try to just change how one particular method functions at a time.

