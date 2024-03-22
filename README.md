# AVS Math Library JS
This is AVS' Math Library for Javascript.

# Algebra.mjs
The Algebra Module is for dealing with polynomials
<hr>
<h2>Term Class</h2>
The Term class is an Object Class given to terms of a polynomial expression.

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Coefficient</td>
    <td>Number</td>
    <td>Term.c</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Degree</td>
    <td>Number</td>
    <td>Term.d</td>
    <td>1</td>
  </tr>
</table>

<h3>Term.evaluate(num)</h3>
The evaluate method will calculate the value of the term when x is a given number.

<h3>Term.toText()</h3>
The toText method will return the term in a string.

<h3>Term.multiply(term2)</h3>
The multiply method will multiply the Term with the inputted term. If the Term is to be multiplied with a number, set term2.d to 0.

<h3>Term.divide(term2)</h3>
The divide method will divide the Term with the inputted term. If the Term is to be divided by a number, set term2.d to 0.
<hr>
<h2>Expression Class</h2>
The Expression class is an Object Class given to a list of Term Class Objects representing a polynomial expression.

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Terms</td>
    <td>List of Term Class Objects</td>
    <td>Expression.terms</td>
    <td></td>
  </tr>
</table>

<h3>Expression.evaluate(num)</h3>
The evaluate method will calculate the value of the expression when x is a given number.

<h3>Expression.toText()</h3>
The toText method will return the term in a string.

<h3>Expression.simplify()</h3>
The simplify method will combine any like terms in the expression.

<h3>Expression.multiply(term)</h3>
The multiply method will multiply the Expression with the inputted term. If the Expression is to be multiplied with a number, set term.d to 0.

<h3>Expression.divide(term)</h3>
The divide method will divide the Expression with the inputted term. If the Expression is to be divided by a number, set term.d to 0.
<hr>
<h2>solveQuadratic(inputs)</h2>
Returns a list of solutions for a quadratic trinomial given an object with a, b, and c, where ax^2+bx+c=0. If there are no real solutions, it will return an empty list.

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>a</th>
    <td>Number</th>
    <td>inputs.a</th>
    <td>1</th>
  </tr>
  <tr>
    <td>b</th>
    <td>Number</th>
    <td>inputs.b</th>
    <td>0</th>
  </tr>
  <tr>
    <td>c</th>
    <td>Number</th>
    <td>inputs.c</th>
    <td>0</th>
  </tr>
</table>
<hr>
<h2>findEquation(inputs)</h2>
Returns an expression where expression=0 has the given the list of solutions. If there are no solutions, it will return an expression with the term equivilant of 1.

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>inputs</td>
    <td>List of Numbers</td>
    <td>inputs</td>
    <td>[]</td>
  </tr>
</table>
<hr>
<h2>findSolutionsOfQuadratic(inputs)</h2>
Returns a list of solutions for a quadratic trinomial (even complex and imaginary ones) given an object with a, b, and c, where ax^2+bx+c=0. If the solutions are imaginary, they will be returned in String form.

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>a</th>
    <td>Number</th>
    <td>inputs.a</th>
    <td>1</th>
  </tr>
  <tr>
    <td>b</th>
    <td>Number</th>
    <td>inputs.b</th>
    <td>0</th>
  </tr>
  <tr>
    <td>c</th>
    <td>Number</th>
    <td>inputs.c</th>
    <td>0</th>
  </tr>
</table>
