# mit-6-0001-problem-set-4-solved
**TO GET THIS SOLUTION VISIT:** [MIT-6.0001 Problem Set 4 Solved](https://www.ankitcodinghub.com/product/mit-6-00-mit-opencourseware-http-ocw-mit-edu-solved-4/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;121268&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MIT-6.0001 Problem Set 4 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (4 votes)    </div>
    </div>
6.00 Introduction to Computer Science and Programming

Fall 2008

For information about citing these materials or our Terms of Use, visit: http://ocw.mit.edu/terms.

6.00: Introduction to Computer Science and Programming

Problem Set 4

Introduction

This problem set will introduce you to using successive approximation, as well as data structures such as tuples and lists.

Collaboration

Submission

This problem set, and future ones, will be auto-graded by a test harness. The test harness will expect your files to include just function definitions, with no executable code outside the function definitions. All your testing code should be in the appropriate test function, which is provided in the template; for example, the testing code for the futureRetire() problem should be in testFutureRetire(). Be sure to add test cases to these test functions beyond what is provided in the template!

Planning for the future

We can model a retirement fund with some simple equations. Assume your starting salary is represented by salary; that the percentage of your salary you put into a retirement fund is save; and that the annual growth percentage of the retirement fund is growthRate. Then your retirement fund, represented by the list F, should increase as follows:

Retirement fund

End of year 1 F[0] = salary * save * 0.01

End of year 2 F[1] = F[0] * (1 + 0.01 * growthRate) + salary * save * 0.01

End of year 3 F[2] = F[1] * (1 + 0.01 * growthRate) + salary * save * 0.01

This process continues each year, with your retirement fund growing both by new contributions and by growth of the principal. Throughout this problem set, growth rates will always be positive (this is not true in the real world, alas!).

Problem 1.

Write a function, called nestEggFixed, which takes four arguments: a salary, a

percentage of your salary to save in an investment account, an annual growth percentage for the investment account, and a number of years to work. This function should return a list, whose values are the size of your retirement account at the end of each year, with the most recent year’s value at the end of the list.

Complete the implementation of:

def nestEggFixed (salary, save, growthRate, years):

Write your code in the appropriate place in the ps4.py template. To test your function, run the test cases in the test function testNestEggFixed(). You should add additional test cases to this function to further test your code.

This first model is pretty simple. Clearly, the market does not grow at a constant rate. So a better model would be to account for variations in growth percentage each year.

Problem 2.

Write a function, called nestEggVariable, which takes three arguments: a salary (salary), a percentage of your salary to save (save), and a list of annual growth percentages on investments (growthRates). The length of the last argument defines the number of years you plan to work; growthRates[0] is the growth rate of the first year,

growthRates[1] is the growth rate of the second year, etc. (Note that because the

retirement fund’s initial value is 0, growthRates[0] is, in fact, irrelevant.) This function should return a list, whose values are the size of your retirement account at the end of each year.

Complete the implementation of:

def nestEggVariable(salary, save, growthRates):

Write your code in the appropriate place in the ps4.py template. To test your function, run the test cases in the test function testNestEggVariable(). You should add additional test cases to this function to further test your code.

Of course, once you retire you will want to be able to withdraw some amount of money each year for living expenses. You can use your previous code to get the size of your retirement fund when you stop working. Now we want to model how much you can withdraw to spend each year after retirement.

Suppose that, after retirement, your retirement fund continues to grow according to a list of annual growth percentages on investments (growthRates), while your annual expenses are constant (wouldn’t zero percent inflation be nice?), called expenses. To see how your retirement fund will change after retirement, we can use the following chart, where we let F represent the size of the retirement fund at the time of retirement, and we let expenses represent the amount of money we withdraw in the first year to cover our living costs:

Retirement fund

End of year 1 F[0] = savings * (1 + 0.01 * growthRates[0]) – expenses

End of year 2 F[1] = F[0] * (1 + 0.01 * growthRates[1]) – expenses

End of year 3 F[2] = F[1] * (1 + 0.01 * growthRates[2]) – expenses

Problem 3.

Write a function, called postRetirement, which takes three arguments: an initial amount of money in your retirement fund (savings), a list of annual growth percentages on investments while you are retired (growthRates), and your annual expenses (expenses). Assume that the increase in the investment account savings is calculated before subtracting the annual expenditures (as shown in the above table). Your function should return a list of fund sizes after each year of retirement, accounting for annual expenses and the growth of the retirement fund. Like problem 2, the length of the growthRates argument defines the number of years you plan to be retired.

Note that if the retirement fund balance becomes negative, expenditures should continue to be subtracted, and the growth rate comes to represent the interest rate on the debt (i.e. the formulas in the above table still apply).

Complete the definition for: def postRetirement(savings, growthRates, expenses):

Write your code in the appropriate place in the ps4.py template. T o test your function, run the test cases in the test function testPostRetirement(). You should add additional test cases to this function to further test your code.

Problem 4.

Write a function, called findMaxExpenses, which takes five arguments: a salary

(salary), a percentage of your salary to save (save), a list of annual growth percentages on investments while you are still working (preRetireGrowthRates), a list of annual growth percentages on investments while you are retired (postRetireGrowthRates), and a value for epsilon (epsilon). As with problems 2 and 3, the lengths of preRetireGrowthRates and postRetireGrowthRates determine the number of years you

plan to be working and retired, respectively.

Use the idea of binary search to find a value for the amount of expenses you can withdraw each year from your retirement fund, such that at the end of your retirement, the absolute value of the amount remaining in your retirement fund is less than epsilon (note that you can overdraw by a small amount). Start with a range of possible values for your annual expenses between 0 and your savings at the start of your retirement (HINT #1: this can be determined by utilizing your solution to problem 2). Your function should print out the current estimate for the amount of expenses on each iteration through the binary search (HINT #2: your binary search should make use of your solution to problem 3), and should return the estimate for the amount of expenses to withdraw. (HINT #3: the answer should lie between zero and the initial value of the savings + epsilon.) Complete the implementation of:

def findMaxExpenses(salary, save, preRetireGrowthRates, postRetireGrowthRates, epsilon):

Write your code in the appropriate place in the ps4.py template. To test your function, run the test cases in the test function testFindMaxExpenses(). You should add additional test cases to this function to further test your code.

Hand-In Function

1. Save

Save your code in the specific file name indicated for each problem. Do not ignore this step or save your file(s) with different names.

2. Time and Collaboration Info

At the start of each file, in a comment, write down the number of hours (roughly) you spent on the problems in that part, and the names of the people you collaborated with. For example:

# Problem Set 4

# Name: Jane Lee

# Time: 1:30

#

… your code goes here …
