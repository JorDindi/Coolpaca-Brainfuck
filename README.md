# Challenge: Reflection of a Circular Path via Vectors

This challenge combines vector reflections with dynamic loci in a geometric construction. You can set this up in **GeoGebra** (or Desmos if you’re comfortable with its vector tools) to see real-time effects as you drag points.

---

## The Setup

1. **Fixed Circle and Points:**  
   - Construct a fixed circle with center \(O\) (choose any convenient position for \(O\)).  
   - Pick two distinct fixed points \(A\) and \(B\) on the circumference of the circle. The line \(AB\) will act as your reflection axis.

2. **Variable Point on the Circle:**  
   - Define a variable point \(P\) that moves along the circumference of the circle.

3. **Reflection Construction:**  
   - Construct the reflection \(P'\) of \(P\) with respect to the line \(AB\).  
   - Use the vector reflection formula to express \(P'\) in terms of \(P\), \(A\), and \(B\).

---

## Your Tasks

### Task 1. Derive the Reflection Formula in Vector Terms

Show that the reflection of a point \(P\) across the line passing through \(A\) with direction 
\[
\mathbf{u} = B - A
\]
is given by
\[
P' = A + 2 \cdot \frac{(P - A) \cdot \mathbf{u}}{\mathbf{u} \cdot \mathbf{u}} \, \mathbf{u} - (P - A).
\]

**Hints:**
- Recall that the projection of \(P - A\) onto \(\mathbf{u}\) is:
  \[
  \text{proj}_{\mathbf{u}}(P-A) = \frac{(P-A) \cdot \mathbf{u}}{\mathbf{u} \cdot \mathbf{u}} \, \mathbf{u}.
  \]
- The reflection is obtained by “flipping” the component perpendicular to the line while leaving the projection unchanged.

---

### Task 2. Prove that the Reflection’s Locus is a Circle

Using your derived formula, demonstrate that as \(P\) moves over the circle with center \(O\), the reflection \(P'\) always lies on another circle. In other words, prove that there exists a fixed point \(K\) (the center of the locus) and a positive real number \(R\) (the radius) such that:
\[
\| P' - K \| = R.
\]

**Hints:**
- Try to “complete the square” in vector terms by rewriting \(P'\) as:
  \[
  P' = K + \lambda (P - L)
  \]
  where \(K\) and \(L\) are expressions involving \(A\), \(B\), and possibly \(O\), and \(\lambda\) is a scaling factor.
- Use the constant nature of \(\|P - O\|\) for all \(P\) on the circle.

---

### Task 3. Express the New Circle’s Center and Radius

Determine explicit expressions for:
- **The Center \(K\) of the Locus:** Express \(K\) in terms of the fixed points \(A\), \(B\), and possibly \(O\).
- **The Radius \(R\):** Derive \(R\) in a manner that shows it is independent of the position of \(P\).

**Hints:**
- Since reflections are isometries, start by finding how the center \(O\) transforms under the reflection in line \(AB\).
- Explore the relationships between the midpoint of \(AB\) and the reflected image of \(O\) relative to line \(AB\).

---

### Task 4. Implement and Explore in GeoGebra

1. **Construction:**
   - Construct the circle centered at \(O\) with a given radius.
   - Place \(A\) and \(B\) on the circle.
   - Define \(P\) as a draggable point on the circle.
   - Construct \(P'\) using the reflection formula. (While many geometry tools allow you to reflect a point over a line directly, try to expose the underlying vector arithmetic by showing an algebraic construction.)

2. **Verification:**
   - Identify or compute the candidate center \(K\) of the locus of \(P'\).
   - Use GeoGebra’s locus tools to confirm that the distance \(\|P' - K\|\) remains constant as you drag \(P\).

3. **Analysis:**
   - Experiment with different positions of \(A\) and \(B\) on the original circle.
   - Observe how the circle traced by \(P'\) changes and analyze the relationship between the positioning of \(A\) and \(B\) and the new circle’s center and radius.

---

## Final Thoughts

This challenge not only tests your understanding of vector operations and reflections but also deepens your insight into geometric transformations. A complete solution involves:
- A rigorous vector derivation of the reflection formula.
- Algebraic manipulation to reframe \(P'\) in a way that reveals a constant distance from a fixed point.
- A dynamic verification in GeoGebra that reinforces the algebraic findings.

Feel free to experiment further by exploring variations such as rotating the reflection line or investigating other isometries.

**Happy constructing and proving!**
