# AVS Math Library JS
This is AVS' Math Library for Javascript.

# Algebra.mjs
The Algebra Module is for dealing with polynomials

<h1>Term Class</h1>
The Term class is an Object Class given to terms of a polynomial expression.
<h2>Attributes:</h2>
<table>
  <tr>
    <th>Attribute Name</th>
    <th>Type</th>
    <th></th>
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
<h2>Methods:</h2>
<h3>Term.evaluate(num)</h3>
The evaluate method will calculate the value of the polynomial when x is a given number.

<h3>Term.toText()</h3>
The toText method will return the term in a string.

<h3>Term.multiply(term2)</h3>
The multiply method will multiply the Term with the inputted term. If the Term is to be multiplied with a number, set term2.d to 0.

<h3>Term.divide(term2)</h3>
The divide method will divide the Term with the inputted term. If the Term is to be divided with a number, set term2.d to 0.

<h1>Expression Class</h1>
The Expression class is an Object Class given to a list of Term Class Objects representing a polynomial expression.

<h2>Attributes:</h2>
<table>
  <tr>
    <th>Attribute Name</th>
    <th>Type</th>
    <th></th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Terms</td>
    <td>List of Term Class Objects</td>
    <td>Expression.terms</td>
    <td></td>
  </tr>
</table>
