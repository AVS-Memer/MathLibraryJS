# AVS Math Library JS
<p>This is AVS' Math Library for Javascript.</p>

<hr>
<h1>Algebra.mjs</h1>
<p>The Algebra Module is for dealing with polynomials</p>
<hr>
<h2>Term Class</h2>
<p>The Term class is an Object Class given to terms of a polynomial expression.</p>

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
<p>The evaluate method will calculate the value of the term when x is a given number.</p>

<h3>Term.toText()</h3>
<p>The toText method will return the term in a string.</p>

<h3>Term.multiply(term2)</h3>
<p>The multiply method will multiply the Term with the inputted term. If the Term is to be multiplied with a number, set term2.d to 0.</p>

<h3>Term.divide(term2)</h3>
<p>The divide method will divide the Term with the inputted term. If the Term is to be divided by a number, set term2.d to 0.</p>
<hr>
<h2>Expression Class</h2>
<p>The Expression class is an Object Class given to a list of Term Class Objects representing a polynomial expression.</p>

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
<p>The evaluate method will calculate the value of the expression when x is a given number.</p>

<h3>Expression.toText()</h3>
<p>The toText method will return the term in a string.</p>

<h3>Expression.simplify()</h3>
<p>The simplify method will combine any like terms in the expression.</p>

<h3>Expression.multiply(term)</h3>
<p>The multiply method will multiply the Expression with the inputted term. If the Expression is to be multiplied with a number, set term.d to 0.</p>

<h3>Expression.divide(term)</h3>
<p>The divide method will divide the Expression with the inputted term. If the Expression is to be divided by a number, set term.d to 0.</p>
<hr>
<h2>solveQuadratic(inputs)</h2>
<p>Returns a list of solutions for a quadratic trinomial given an object with a, b, and c, where ax^2+bx+c=0. If there are no real solutions, it will return an empty list.</p>

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>a</td>
    <td>Number</td>
    <td>inputs.a</td>
    <td>1</td>
  </tr>
  <tr>
    <td>b</td>
    <td>Number</td>
    <td>inputs.b</td>
    <td>0</td>
  </tr>
  <tr>
    <td>c</td>
    <td>Number</td>
    <td>inputs.c</td>
    <td>0</td>
  </tr>
</table>
<hr>
<h2>findEquation(inputs)</h2>
<p>Returns an expression where expression=0 has the given the list of solutions. If there are no solutions, it will return an expression with the term equivilant of 1.</p>

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
<p>Returns a list of solutions for a quadratic trinomial (even complex and imaginary ones) given an object with a, b, and c, where ax^2+bx+c=0. If the solutions are imaginary, they will be returned in String form.</p>

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>a</td>
    <td>Number</td>
    <td>inputs.a</td>
    <td>1</td>
  </tr>
  <tr>
    <td>b</td>
    <td>Number</td>
    <td>inputs.b</td>
    <td>0</td>
  </tr>
  <tr>
    <td>c</td>
    <td>Number</td>
    <td>inputs.c</td>
    <td>0</td>
  </tr>
</table>

<hr>
<h1>Calculus.mjs</h1>
<p>The Calculus Module is for derivating and integrating polynominals.</p>
<hr>
<h2>derivativeOf(inputs)</h2>
<p>Derives Expression, and evaluates it at Number if given.</p>

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Expression</td>
    <td>Expression Class Object (from Algebra.mjs)</td>
    <td>inputs.expression</td>
    <td></td>
  </tr>
  <tr>
    <td>Number</td>
    <td>Number</td>
    <td>inputs.number</td>
    <td></td>
  </tr>
</table>

<hr>
<h2>integralOf(inputs)</h2>
<p>Integrates Expression, and evaluates it at Number if given.</p>

<h3>Inputs</h3>
<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Expression</td>
    <td>Expression Class Object (from Algebra.mjs)</td>
    <td>inputs.expression</td>
    <td></td>
  </tr>
  <tr>
    <td>Number</td>
    <td>Number</td>
    <td>inputs.number</td>
    <td></td>
  </tr>
</table>

<hr>
<h1>Geometry.mjs</h1>
<p>The Geometry Module is for Point, Line, and Polygon Objects, and can be utilized for graphing.</p>
<hr>
<h2>Point Class</h2>
<p>The Point class is an Object Class given to points that could be plotted on a graph.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>x</td>
    <td>Number</td>
    <td>Point.x</td>
    <td>0</td>
  </tr>
  <tr>
    <td>y</td>
    <td>Number</td>
    <td>Point.y</td>
    <td>0</td>
  </tr>
</table>

<h3>Point.translate(inputs)</h3>
<p>Translates the point according to the inputs.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>x</td>
    <td>Number</td>
    <td>inputs.x</td>
    <td>The horizontal distance to translate the point by.</td>
    <td>0</td>
  </tr>
  <tr>
    <td>y</td>
    <td>Number</td>
    <td>inputs.y</td>
    <td>The vertical distance to translate the point by.</td>
    <td>0</td>
  </tr>
</table>
<hr>
<h2>Line Class</h2>
<p>The Line class is an Object Class given to lines that could be plotted on a graph.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Endpoint 1</td>
    <td>Point Class Object</td>
    <td>Line.pt1</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Endpoint 2</td>
    <td>Point Class Object</td>
    <td>Line.pt2</td>
    <td>1</td>
  </tr>
</table>

<h3>Line.update()</h3>
<p>Updates the line's other properties.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Slope</td>
    <td>Number</td>
    <td>Line.lSlope</td>
    <td>Slope of the line</td>
  </tr>
  <tr>
    <td>Length</td>
    <td>Number</td>
    <td>Line.lLength</td>
    <td>Length of the line</td>
  </tr>
  <tr>
    <td>Angle</td>
    <td>Number</td>
    <td>Line.lAngle</td>
    <td>Angle of Elevation of the line</td>
  </tr>
</table>

<h3>Line.translate(inputs)</h3>
<p>Translates both endpoints according to the inputs.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>x</td>
    <td>Number</td>
    <td>inputs.x</td>
    <td>The horizontal distance to translate the line by.</td>
    <td>0</td>
  </tr>
  <tr>
    <td>y</td>
    <td>Number</td>
    <td>inputs.y</td>
    <td>The vertical distance to translate the line by.</td>
    <td>0</td>
  </tr>
</table>
<hr>
<h2>Side Class (Inherits from Line)</h2>
<p>The Side class is an Object Class given to lines that form the sides of a polygon.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Endpoint 1</td>
    <td>Point Class Object</td>
    <td>Side.pt1</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Endpoint 2</td>
    <td>Point Class Object</td>
    <td>Side.pt2</td>
    <td>1</td>
  </tr>
</table>

<h3>Side.update()</h3>
<p>Updates the side's other properties.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Slope</td>
    <td>Number</td>
    <td>Side.lSlope</td>
    <td>Slope of the side</td>
  </tr>
  <tr>
    <td>Length</td>
    <td>Number</td>
    <td>Side.lLength</td>
    <td>Length of the side</td>
  </tr>
  <tr>
    <td>Angle</td>
    <td>Number</td>
    <td>Side.lAngle</td>
    <td>Angle of Elevation of the side</td>
  </tr>
</table>
<hr>
<h2>Polygon Class</h2>
<p>The Polygon class is an Object Class given to polygons that could be plotted on a graph.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Points</td>
    <td>List of Point Class Objects</td>
    <td>Polygon.pts</td>
    <td></td>
  </tr>
</table>

<h3>Polygon.update()</h3>
<p>Updates the polygon's other properties.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Sides</td>
    <td>List of Side Class Objects</td>
    <td>Polygon.sides</td>
    <td>The sides of the polygon</td>
  </tr>
  <tr>
    <td>Angles</td>
    <td>Number</td>
    <td>Polygon.pts[i].angle</td>
    <td>The angle at each point of the polygon</td>
  </tr>
  <tr>
    <td>Perimeter</td>
    <td>Number</td>
    <td>Polygon.perimeter</td>
    <td>The perimeter of the polygon</td>
  </tr>
</table>

<h3>Polygon.dialate(inputs)</h3>
<p>Scales the polygon the given amount from the Dialation Point.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Dialation Point</td>
    <td>Point Class Object</td>
    <td>inputs.dialationPt</td>
    <td>The point of dialation for the polygon.</td>
    <td>{x: 0, y: 0}</td>
  </tr>
  <tr>
    <td>Scale</td>
    <td>Number</td>
    <td>inputs.scale</td>
    <td>The size to dialate the polygon by.</td>
    <td>1</td>
  </tr>
</table>

<h3>Polygon.rotate(inputs)</h3>
<p>Rotates the polygon amount from the Rotation Point.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Rotation Point</td>
    <td>Point Class Object</td>
    <td>inputs.rotationPt</td>
    <td>The point of dialation for the polygon.</td>
    <td>{x: 0, y: 0}</td>
  </tr>
  <tr>
    <td>Angle</td>
    <td>Number</td>
    <td>inputs.angle</td>
    <td>The angle to rotate the polygon by.</td>
    <td>1</td>
  </tr>
</table>

<h3>Polygon.translate(inputs)</h3>
<p>Translates the polygon according to the inputs.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>x</td>
    <td>Number</td>
    <td>inputs.x</td>
    <td>The horizontal distance to translate the polygon by.</td>
    <td>0</td>
  </tr>
  <tr>
    <td>y</td>
    <td>Number</td>
    <td>inputs.y</td>
    <td>The vertical distance to translate the polygon by.</td>
    <td>0</td>
  </tr>
</table>
<hr>
<h2>Triangle Class (Inherits from Polygon)</h2>
<p>The Triangle class is an Object Class given to triangles that could be plotted on a graph.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Points</td>
    <td>List of Point Class Objects of Length 3</td>
    <td>Triangle.pts</td>
    <td></td>
  </tr>
</table>

<h3>Triangle.update()</h3>
<p>Updates the triangle's other properties.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Sides</td>
    <td>List of Side Class Objects</td>
    <td>Triangle.sides</td>
    <td>The sides of the triangle</td>
  </tr>
  <tr>
    <td>Angles</td>
    <td>Number</td>
    <td>Triangle.pts[i].angle</td>
    <td>The angle at each point of the triangle</td>
  </tr>
  <tr>
    <td>Perimeter</td>
    <td>Number</td>
    <td>Triangle.perimeter</td>
    <td>The perimeter of the triangle</td>
  </tr>
  <tr>
    <td>Side Type</td>
    <td>String</td>
    <td>Triangle.sideType</td>
    <td>The type of triangle based off of the sides</td>
  </tr>
  <tr>
    <td>Angle Type</td>
    <td>String</td>
    <td>Triangle.angleType</td>
    <td>The type of triangle based off of the angles</td>
  </tr>
  <tr>
    <td>Area</td>
    <td>Number</td>
    <td>Triangle.area</td>
    <td>The area of the triangle</td>
  </tr>
  <tr>
    <td>Altitudes</td>
    <td>List of Numbers</td>
    <td>Triangle.alts</td>
    <td>The altitudes from each point of the triangle</td>
  </tr>
  <tr>
    <td>Inradius</td>
    <td>Number</td>
    <td>Triangle.inradius</td>
    <td>The radius of the incircle of the triangle</td>
  </tr>
  <tr>
    <td>Circumradius</td>
    <td>Number</td>
    <td>Triangle.circumradius</td>
    <td>The radius of the circumcircle of the triangle</td>
  </tr>
</table>

<h3>Triangle.dialate(inputs)</h3>
<p>Scales the triangle the given amount from the Dialation Point.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Dialation Point</td>
    <td>Point Class Object</td>
    <td>inputs.dialationPt</td>
    <td>The point of dialation for the triangle.</td>
    <td>{x: 0, y: 0}</td>
  </tr>
  <tr>
    <td>Scale</td>
    <td>Number</td>
    <td>inputs.scale</td>
    <td>The size to dialate the triangle by.</td>
    <td>1</td>
  </tr>
</table>

<h3>Triangle.rotate(inputs)</h3>
<p>Rotates the triangle amount from the Rotation Point.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Rotation Point</td>
    <td>Point Class Object</td>
    <td>inputs.rotationPt</td>
    <td>The point of dialation for the triangle.</td>
    <td>{x: 0, y: 0}</td>
  </tr>
  <tr>
    <td>Angle</td>
    <td>Number</td>
    <td>inputs.angle</td>
    <td>The angle to rotate the triangle by.</td>
    <td>1</td>
  </tr>
</table>

<h3>Triangle.translate(inputs)</h3>
<p>Translates the triangle according to the inputs.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>x</td>
    <td>Number</td>
    <td>inputs.x</td>
    <td>The horizontal distance to translate the triangle by.</td>
    <td>0</td>
  </tr>
  <tr>
    <td>y</td>
    <td>Number</td>
    <td>inputs.y</td>
    <td>The vertical distance to translate the triangle by.</td>
    <td>0</td>
  </tr>
</table>
<hr>
<h2>Quadrilateral Class (Inherits from Polygon)</h2>
<p>The Quadrilateral class is an Object Class given to quadrilaterals that could be plotted on a graph.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Points</td>
    <td>List of Point Class Objects of Length 4</td>
    <td>Quadrilateral.pts</td>
    <td></td>
  </tr>
</table>

<h3>Quadrilateral.update()</h3>
<p>Updates the quadrilateral's other properties.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Sides</td>
    <td>List of Side Class Objects</td>
    <td>Quadrilateral.sides</td>
    <td>The sides of the quadrilateral</td>
  </tr>
  <tr>
    <td>Angles</td>
    <td>Number</td>
    <td>Quadrilateral.pts[i].angle</td>
    <td>The angle at each point of the quadrilateral</td>
  </tr>
  <tr>
    <td>Perimeter</td>
    <td>Number</td>
    <td>Quadrilateral.perimeter</td>
    <td>The perimeter of the quadrilateral</td>
  </tr>
  <tr>
    <td>Type</td>
    <td>String</td>
    <td>Quadrilateral.type</td>
    <td>The type of quadrilateral</td>
  </tr>
  <tr>
    <td>Area</td>
    <td>Number</td>
    <td>Quadrilateral.area</td>
    <td>The area of the quadrilateral</td>
  </tr>
</table>

<h3>Quadrilateral.dialate(inputs)</h3>
<p>Scales the quadrilateral the given amount from the Dialation Point.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Dialation Point</td>
    <td>Point Class Object</td>
    <td>inputs.dialationPt</td>
    <td>The point of dialation for the quadrilateral.</td>
    <td>{x: 0, y: 0}</td>
  </tr>
  <tr>
    <td>Scale</td>
    <td>Number</td>
    <td>inputs.scale</td>
    <td>The size to dialate the quadrilateral by.</td>
    <td>1</td>
  </tr>
</table>

<h3>Quadrilateral.rotate(inputs)</h3>
<p>Rotates the quadrilateral amount from the Rotation Point.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>Rotation Point</td>
    <td>Point Class Object</td>
    <td>inputs.rotationPt</td>
    <td>The point of dialation for the quadrilateral.</td>
    <td>{x: 0, y: 0}</td>
  </tr>
  <tr>
    <td>Angle</td>
    <td>Number</td>
    <td>inputs.angle</td>
    <td>The angle to rotate the quadrilateral by.</td>
    <td>1</td>
  </tr>
</table>

<h3>Quadrilateral.translate(inputs)</h3>
<p>Translates the quadrilateral according to the inputs.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>x</td>
    <td>Number</td>
    <td>inputs.x</td>
    <td>The horizontal distance to translate the quadrilateral by.</td>
    <td>0</td>
  </tr>
  <tr>
    <td>y</td>
    <td>Number</td>
    <td>inputs.y</td>
    <td>The vertical distance to translate the quadrilateral by.</td>
    <td>0</td>
  </tr>
</table>
<hr>
<h2>Vector Class</h2>
<p>The Vector class is an Object Class given to vector arrows that could be plotted on a graph.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>i</td>
    <td>Number</td>
    <td>Vector.i</td>
    <td>0</td>
  </tr>
  <tr>
    <td>j</td>
    <td>Number</td>
    <td>Vector.j</td>
    <td>0</td>
  </tr>
</table>

<h3>Vector.update()</h3>
<p>Updates the vector's other properties.</p>

<table>
  <tr>
    <th>Attributes</th>
    <th>Type</th>
    <th>Variable Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Slope</td>
    <td>Number</td>
    <td>Line.vSlope</td>
    <td>Slope of the vector</td>
  </tr>
  <tr>
    <td>Magnitude</td>
    <td>Number</td>
    <td>Line.vMagnitude</td>
    <td>Length of the vector</td>
  </tr>
  <tr>
    <td>Angle</td>
    <td>Number</td>
    <td>Line.vAngle</td>
    <td>Angle of the vector</td>
  </tr>
</table>

<h3>Vector.add(vector2)</h3>
<p>Adds Vector to vector2.</p>

<h3>Vector.subtract(vector2)</h3>
<p>Subtracts Vector from vector2.</p>

<h3>Vector.multiply(number)</h3>
<p>Multiplies Vector by number.</p>

<h3>Vector.divide(number)</h3>
<p>Divides Vector by number.</p>

<h3>Vector.dotProduct(vector2)</h3>
<p>Returns the dot product of Vector and vector2.</p>

<h3>Vector.crossProduct(vector2)</h3>
<p>Returns the cross product of Vector and vector2.</p>
