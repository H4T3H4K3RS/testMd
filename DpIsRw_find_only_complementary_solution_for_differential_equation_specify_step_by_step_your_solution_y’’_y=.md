

# **Solution of Differential Equation**

Given differential equation is:

$$ y'' + y = 6 \sin2x $$

## **Step 1:**

Rewrite the given differential equation in standard form using the following identities:

$$ \sin2x = 2 \sin x \cos x $$

$$ y'' + y = 6 \sin x \cos x $$

## **Step 2:**

Let $$ y = A \sin x + B \cos x $$

be the solution of the given differential equation.

## **Step 3:**

Substitute $$ y, \; y' \; \text{and} \; y'' $$ in the differential equation and solve for $$ A \; \text{and} \; B $$

$$ \begin{aligned} y &= A \sin x + B \cos x \\ y' &= A \cos x - B \sin x \\ y'' &= -A \sin x - B \cos x \end{aligned} $$

Substituting these in the differential equation, we get:

$$ A \sin x + B \cos x + (-A \sin x - B \cos x) = 6 \sin x \cos x $$

Simplifying, we get:

$$ \begin{aligned} A \sin x + B \cos x &= 6 \sin x \cos x \\ A \sin x &= 6 \sin x \cos x - B \cos x \end{aligned} $$

From above equations, we get:

$$ A = 6 \cos x \quad \text{and} \quad B = -6 \sin x $$

## **Step 4:**

The solution of the given differential equation is:

$$ y = 6 \cos x \sin x -6 \sin x \cos x $$

Simplifying, we get:

$$ y = 6 \sin 2x $$