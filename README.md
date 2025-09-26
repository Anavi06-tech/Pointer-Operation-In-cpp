
🧵 Pointer Operations in C++


---

🎯 Aim

To study and implement pointer operations in C++ and understand the difference between call by value and call by reference parameter-passing methods.


---

📚 Theory

In C++, the way we pass parameters to functions determines whether changes inside the function affect the original variables.

📦 Call by Value

Definition: A copy of the actual parameter is passed to the function.

Effect: Changes are made only on the copy → originals remain unchanged.

Working: Function operates in its own scope and does not affect the caller’s variables.


🔗 Call by Reference

Definition: The address or reference of actual parameters is passed, allowing direct modification of originals.

Effect: Changes done inside the function reflect in the caller variables.

Working: Function works on the actual memory location by using references/pointers.



---

📊 Comparison Table

⚙️ Feature	📦 Call by Value	🔗 Call by Reference

Data Passed	Copy of value	Address / reference
Changes affect original	❌ No	✅ Yes
Memory Use	Extra copy made	No extra copy
Safety	Safer (no side effects)	Can modify caller data
Typical Use Case	Read-only operations	In-place modifications



---

🖼️ Visual Representation

📌 Call by Value vs Call by Reference

Call by Value: Function works on a duplicate copy → original variable remains unchanged.

Call by Reference: Function directly accesses the original memory → changes reflect in the caller.


(Use diagram/flowchart representation in record for better clarity)


---

📋 Algorithms

🔹 Employee Salary Increment Check

1. Start


2. Input details:

Years completed in service

Worked on research projects (Yes/No)

New project pipeline (Yes/No)

Profit generated in rupees

Current salary



3. Pass the above values to function using call by reference.


4. Inside the function:

Initialize conditionsMet = 0

If yearsCompleted ≥ 1 → increment conditionsMet

If worked on research projects → increment conditionsMet

If new project in pipeline → increment conditionsMet

If profit generated > 1,00,000 → increment conditionsMet



5. If conditionsMet ≥ 3:

Increase salary by 20%

Display "Eligible for increment" and updated salary



6. Else:

Display "Not eligible for increment" and unchanged salary



7. End




---

🔹 Reverse a String Using Pointers

1. Start


2. Input a string str1.


3. Find length of the string n.


4. Store base address of the string in a pointer.


5. Display "Reversed String".


6. Loop from last character to first:

Print each character using pointer arithmetic.



7. When loop finishes, reversed string is displayed.


8. End




---

🧠 Conclusion

This experiment highlights how pointers enable different parameter-passing methods:

📦 Call by Value → Works on a copy; original variable remains unaffected.

🔗 Call by Reference → Works directly on real data; changes are reflected in the original variable.


✅ Key Insight:

Use Call by Value when safety and immutability are required.

Use Call by Reference when efficiency and in-place modification are needed.

