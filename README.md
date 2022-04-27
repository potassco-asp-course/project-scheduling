# Scheduling Project

You can find the instructions of the project in the file [scheduling.ipynb](scheduling.ipynb).

To submit your solution, please modify the files
[flowshop.lp](asp/flowshop.lp)
and
[jobshop.lp](asp/jobshop.lp)
of the directory [asp](asp) with your encoding.

Every time you push a new commit, your solution will be tested automatically.
The timeout per instance is `180` seconds, and the actual command calls for the tests are:
* ``python3.6 asp/test.py -e asp/flowshop.lp -s asp/solutions-flowshop -t 180 -opt``
* ``python3.6 asp/test.py -e asp/jobshop.lp -s asp/solutions-jobshop -t 180 -opt``

For help, type `python3.6 asp/test.py --help`.
Note that the script `test.py` only computes and checks one optimal answer set.

After a few minutes you will be able to see the result of the test in the **Actions** tab.
You can get more information about the result of the test by clicking successively on:
1. The specific test.
2. "Autograding".
3. "Run education/autograding@v1".

Then scroll down until around line 150.
For each instance, you will see if the test is a:
* "success" (correct answer),
* "failure" (wrong answer),
* "timeout" (no solution found before the time runs out), or
* "error" (clingo error).
