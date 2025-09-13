# The Long Document

### Navigation

[insert links to points/chapters here]

0. Credits
    - A lot of these points have been made by people smarter than me and I do not intend on taking their credit.
    - By making these notes, I'm learning to focus on common mistakes made in the work/code space so as not to repeat them in the future again.


Establish a Standard Indentation Policy

## 1. Genereal Principles

1. Adhere to the **Style of the Original**
    - [X] Follow the style of the original code. 
    - Never re-write old software to match the style of the new one.
        - making this mistake will make the code harder to read and comprendhend for others and your future self.
    - Rewriting old code to only change it's style might introduce costly and avoidable defects.

--

2. Adhere to the **Principle of Least Astonishment**
    - avoid anything that will surpirse a user (to any) of your software.

    - [X] The behavior of the software must be **predictable and consistent.**
        - [X] If not, Document and Justify any unusual patterns of use or behavior.
        - The following may help; 

---

    - [X] Simplicity
        - Build classes and simple methods.
        - How much you need to do to meet the expectations of your users.

    - [X] Clarity
        - Ensure each class, interface, method, variable, and object has a clear purpose.
            - Explain where, when, why, and how to use each.

    - [X] Completeness
        - Provide the minimum functionality that any reasonable user would expect to find and use.
        - Create complete documentation; document all features and functionality.


    - [X] Consistency
        - Similar Entities should look and behave the same; dissimilar entities should look and behave differently. Create and apply standards whenever possible.

    - [X] Robustness
        - Provide Predictable Documented Behavior for Errors
            - DO NOT HIDE ERRORS (FROM ANYONE)
            - DO NOT FORCE CLIENTS TO DETECT ERRORS

--- 


3. Do it Right the First Time
    - Any and all code of yours will be read by someone (including yourself) and may even be submitted for production.

4. **Document any Deviatations.**
    - No standard is perfect
    - No standard is universally applicable

    - When you deviate from an established standard
        - Explain the rule that you are breaking and the reasonable answer behind that why.

## 2. Formatting Conventions

5. Always Indent Nested Code

```java
button.addActionListerner() {
    new ActionEventListerner () {
        public void actionPerformed() {
        _|_|_|_... // four spaces
        }
    }
}
```

6. Break up Long Lines 
    - (Don't ignore the signs of long-linitus)

```java
double length = Math.sqrt(Math.pow(x, 2.0), Math.pow(y, 2.0)); // too long

double length = Math.sqrt(Math.pow(x, 2.0),
                          Math.pow(y, 2.0)); // this looks better when the screen is bigger
```

7. 