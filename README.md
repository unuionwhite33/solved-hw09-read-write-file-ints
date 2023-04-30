Download Link: https://assignmentchef.com/product/solved-hw09-read-write-file-ints
<br>
Now that we’ve had a taste of what file I/O is all about, here’s your chance to try it out on your own!

You’re to write a program that will prompt the user if he/she would like to read ints from a file (and have them displayed to stdout) or write ints to a file for safekeeping. If the user wishes to save a set of numbers, then the file <strong>nums.txt</strong> is opened for writing and the user is prompted for integer values which are written to the output file. If the user decides to read the ints from <strong>nums.txt</strong>, then the file is opened and the integers it contains are extracted and displayed to stdout. If you’d like to see some sample runs, take a look at <strong>ReadWriteIntsSampleRuns.txt</strong>. For this implementation, you’ll have to write a couple of other functions in addition to the <strong>main</strong> function:

<strong>WriteInts</strong> — this function is called from <strong>main</strong> if the user wants to save a set of integers to the <strong>nums.txt</strong> file; it accepts as an input argument an opened output file stream object that’s ready for writing. It then prompts the user for five integer values, each of which are written to the output file before returning back to the caller.

<strong>DisplayInts</strong> — this function is called from <strong>main</strong> if the user wants to display the contents of <strong>nums.txt</strong> to stdout; it accepts as an input argument an opened input file stream object that’s ready for reading. It proceeds to extract the five integer values and display them to stdout.

The <strong>main</strong> function will drive the whole program, it’ll be responsible for determining which function to call as well as the opening and closing of files. For more information, you may want to look in your book on <strong>p.308</strong> for an introduction to file I/O, and a simple example on <strong>p.313</strong> where the author demonstrates the<strong>.open</strong> and <strong>.close</strong> member functions you can call once you’ve declared an <strong>ifstream</strong> or <strong>ofstream</strong> variable. (However, don’t forget to call the <strong>.fail</strong> function after you open the file so you can check if you were successful in opening the file; see <strong>p.316</strong> for a brief discussion of that as well as a code sample!) Finally, on <strong>p.334</strong> where the author points out that when you pass file stream variables as arguments to functions, they <strong>must be passed by reference</strong>.

<strong>Sample of Output:</strong>

<strong>Run #1</strong>: user attempts to read from a file that doesn’t yet exist

Do you wish to R)ead or W)rite ints? r

Unable to open the input file…

<strong>Run #2</strong>: user decides to save a set of ints to file “nums.txt”

Do you wish to R)ead or W)rite ints? w

Enter an int: 11

Enter an int: 22

Enter an int: 33

Enter an int: 44

Enter an int: 55

<strong>Run #3:</strong> user displays the contents of “nums.txt” to stdout.

Do you wish to R)ead or W)rite ints? r

11

22

33

44

55