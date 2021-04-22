## Part 1a
1. values added: 20

2. final result: 20

3. values added: 20

4. error; result was defined out-of-scope (within the nested if-statement with the 'let' keyword) so the compiler treats it as undefined.

5. error; result was declared with the 'const' keyword, so the compiler complains when we try to reassign its value in line 7.

6. error; same reasoning as for number 5

## Part 1b
1. "3" gets printed; specifically, i is printed. While i begins with a value of 0, it gets incremented 3 times in the for-loop. There is no error because i is declared with the keyword 'var'.

2. "150" gets printed; specifically, discountedPrice gets printed. The value of discountedPrice changes with each loop iteration, so only its final value, 300 * (1 - 0.5) = 150, gets printed.

3. "150" gets printed; specifically, finalPrice gets printed. While finalPrice begins with a value of 0, this value changes with each loop iteration. Only the final value, Math.round(150 * 100) / 100 = 150, gets printed.

4. The function will return \[50, 100, 150\]; these are the 50% discounted versions of the prices passed into the function on line 19 (\[100, 200, 300\]).

5. error; since i is now declared with the keyword 'let', it goes out of scope once we exit the for-loop.

6. error; since discountedPrice is now declared with the keyword 'let', it goes out of scope once we exit the for-loop.

7. "150" gets printed; changing the keyword 'var' to 'let' in the declaration of finalPrice does not make finalPrice go out of scope, as it was declared outside of the for-loop (but still in discountPrices()). Apart from this, the explanation is the same as for number 3.

8. The function will return \[50, 100, 150\]; changing the keyword 'var' to 'let' in the declaration of discounted does not make finalPrice go out of scope, as it was declared outside of the for-loop (but still in discountPrices()). Apart from this, the explanation is the same as for number 4.

9. error; since i is declared with the keyword 'let', it goes out of scope once we exit the for-loop.

10. "3" gets printed; specifically, length gets printed. length is assigned once and never changed, so there's no error, and \[100, 200, 300\] has 3 elements, hence why length has a value of 3.

11. The function will return \[50, 100, 150\]; though discounted was declared with the keyword 'const', the push value doesn't reassign any value in the array, so there is no error (if we tried to assign a value to a specific index, there would be an issue). Apart from this, the explanation is the same as for number 4.

12.
<ol type="a">
  <li>student.name</li>
  <li>student['Grad Year']</li>
  <li>student.greeting();</li>
  <li>student['Favorite Teacher'].name</li>
  <li>student.courseLoad[0]</li>
</ol>

13.
<ol type="a">
  <li>32; 2 is mapped to the string '2'</li>
  <li>1; '3' is mapped to the integer 3</li>
  <li>3; null is mapped to the integer 0</li>
  <li>3null; null is mapped to the string 'null'</li>
  <li>4; true is mapped to the integer 1</li>
  <li>0; both false and null are mapped to the integer 0</li>
  <li>3undefined; undefined is mapped to the string 'undefined'</li>
  <li>NaN; '3' is mapped to the integer 3 and undefines maps to NaN (Not-a-Number)</li>
</ol>

14.
<ol type="a">
  <li>true; '2' is mapped to the integer 2</li>
  <li>false; '2' is alphabetically after '12'</li>
  <li>true; '2' is mapped to the integer 2</li>
  <li>false; the integer 2 and the string '2' are of different types</li>
  <li>false; true is mapped to the integer 1</li>
  <li>true; anything other than the empty string, 0, undefined, and null is treated as true, so Boolean(2) maps to true</li>
</ol>

15. Whereas the == operator will perform type conversions to resolve type differences, the === operator always considers of operands of different types to be different, and therefore unequal.

16. see part1b-question16.js

17. \[2, 4, 6\] is returned; for each element in \[1, 2, 3\], modifyArray calls doSomething on that element (which multiplies it by 2) and pushes the result onto newArr. After the loop finishes, newArr is returned with the contents of \[1, 2, 3\], but doubled in value.

18. see part1b-question18.js

19. "1 | 4 | 3 | 2", where |'s represent newlines. 1 is printed normally, 2 is delayed by a (relatively) long time, 3 is slightly delayed, and 4 is printed normally.
