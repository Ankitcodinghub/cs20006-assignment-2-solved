# cs20006-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CS20006 Assignment 2 Solved](https://www.ankitcodinghub.com/product/software-engineering-cs20006-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116483&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS20006 Assignment 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
We want to design a User-Defined Datatype (UDT) Fraction for rational numbers. It should behave like the built-in numerical types (for example, int). The concept, interface and implementation of the datatype are discussed below before the engineering requirements and tasks are specified.

1. Concept: Here we outline the basic concept for a Fraction datatype. class Fraction is to be designed as a UDT representing reduced (normalized) proper fractions (rational numbers) of the form where p,q ∈ int, q &gt; 0, and gcd(p,q) = 1. Hence, all will be represented only as .

Most operations available in C++ for int type should be available in their respective syntax and semantics for Fraction. Some operations (like variants of assignments) have been skipped for simplicity and some operations (like logical negation) have been given new semantics.

2. Interface: The expected behavior of the datatype (operations) are discussed in this section.

• Constructors: All constructors must only create normalized fractions. They include

– Constructor with a pair of int values for the numerator and denominator properly defaulted.

∗ Invoked as a default constructor, it would create:

∗ Invoked with one parameter m, it would create:

∗ Invoked with two parameters m and n, it would create: 0, the construction will be done with −m and −n. If m = 0, n is taken to be 1. Naturally, if n = 0, the program would call exit(1) .

– Constructor from a single double value d. The class Fraction should use a preset int precision to convert from d as:

This constructor should not allow implicit conversion.

– Copy Constructor: Should implement the usual semantics

• Destructor: Should implement the usual semantics

• Copy Assignment Operator: Should implement the usual semantics

– Unary minus operator:

– Unary plus operator: +

– Prefix pre-decrement operator for dividendo returns

– Prefix pre-increment operator for componendo returns

– Postfix post-decrement operator for lazy dividendo returns &amp; performs

– Postfix post-increment operator for lazy componendo returns &amp; performs

• Binary Arithmetic Operators (using friend functions): The operator should take a pair of Fraction values and produce a Fraction value after the operation. The operands must not be modified. The operator returns the result of:

– Addition: Adding the First operand to the Second operand

– Subtraction: Subtracting the Second operand from the First operand

– Multiplication: Multiplying the First operand with the Second operand

– Division: Dividing the First operand by the Second operand. Should throw an exception if the divider (Second operand) is zero

– Remainder: Remainder of division of the First operand by the Second operand. Should throw an exception if the divider (Second operand) is zero

• Binary Relational Operators: The operator should take a pair of Fraction values and produce a bool result. The operands must not be modified. The operator returns true when

– Operands are Equal

– Operands are Not Equal

– First operand is Less than Second operand

– First operand is Less than or Equal to Second operand

– First operand is More than Second operand

– First operand is More than or Equal to Second operand

• Special Operators: The negation (!) operator should take a Fraction value and produce an inverted Fraction value as ! . The operand must not be modified and should throw an exception if the fraction is zero.

• I/O Operators (using friend functions): Should implement the usual semantics for streaming.

– Output: Streaming to ostream. to be output as p / q. The divider should be omitted if is a whole number.

– Input: Streaming from istream. Read a pair of int p and q, form and normalize

• Constants of the Datatype: Unity and Zero should be defined as static constants

– sc fUnity = Fraction()

– sc fZero = Fraction(0)

• Utility Functions of the Datatype: The following static functions should be available:

– precision() to return the constant to be used in conversion from double

– int gcd(int, int) finds the greatest common divisor (gcd) for two positive integers

– int lcm(int, int) finds the least common multiple (lcm) for two positive integers

3. Implementation: A suggestive implementation for the datatype is given here. Any other choice of implementation consistent with the interfaces would be acceptable.

• Data Members

– Numerator of type int

– Denominator of type unsigned int

• Utility Function

– A function to normalize a fraction to its proper form. Also, sets q to 1 if p is 0.

4. Engineering: Finally, we engineer the concept based on the expectations of the interface and implementation to create the Fraction datatype. The tasks therein include:

(a) Design the interface for class Fraction containing the exposed member functions (signatures only) as specified in Interface section. Explain the design considerations (like parameters, types, call/return-by-value/reference, const-ness, initialization, exception etc.) in comments before every member function to illustrate your design understanding and depth.

Put the design in “Fraction.hxx”

Destructor [0.5]

Copy Assignment Operator [0.5] Unary Arithmetic Operators [0.5 * 6 = 3]

Binary Arithmetic Operators [1 * 5 = 5] Binary Relational Operators [0.5 * 6 = 3]

Special Operators [0.5] I/O Operators [1 * 2 = 2]

Constants of the Datatype [1 * 2 = 2]

Utility Functions of the Datatype [0.5 * 3 = 1.5]

(b) Add the implementation for class Fraction containing the concealed data members and member functions as specified in Implementation section. Explain the design considerations in comments before every member. [0]

(c) Implement all member functions of class Fraction and inline as appropriate. Add implementation notes as comments for every function.

Put the implementations of the inline member functions in “Fraction.hxx”. Put the non-inline member function implementations and static constants in “Fraction.cxx”

Constructors [2 * 3 = 6]

Destructor [1]

Copy Assignment Operator [2]

Unary Arithmetic Operators [0.5 * 4 + 1 * 2 = 4] Binary Arithmetic Operators [1 * 5 = 5] Binary Relational Operators [0.5 * 6 = 3]

Special Operators [1 + 1 = 2]

I/O Operators [1.5 * 2 = 3]

Constants of the Datatype [0.5 * 2 = 1]

Utility Functions of the Datatype [3]

(d) Test your implementation using the void TestFraction() below from “TestFraction.cxx” file. Finally, int main() (file “Main.cxx”) invokes TestFraction() to perform the test.

Put your test results in “Fraction.out”

Note:

• If you are unable to write the interface (signature) of a member function, skip it in “Fraction.hxx” and comment out its use in “TestFraction.cxx”

• If you are unable to write the implementation of a member function, skip it in “Fraction.hxx” or “Fraction.cxx” and comment out its use in “TestFraction.cxx”

(e) Submit “Fraction.hxx”, “Fraction.cxx”, “TestFraction.cxx”, “Main.cxx”, and “Fraction.out” in a zip file assgn-2-&lt;your roll&gt;.zip.

Note:

• “Fraction.hxx” and “Fraction.cxx” will be evaluated

• “Fraction.out” will be checked for completeness of operators

// File: TestFraction.cxx

// Contains: void TestFraction()

/************ C++ Headers ************************************/

#include &lt;iostream&gt; using namespace std;

/************ PROJECT Headers ********************************/

#include “Fraction.hxx”

void TestFraction() { cout &lt;&lt; ” Test Fraction Data Type” &lt;&lt; endl;

// CONSTRUCTORS

// ———–Fraction f1(5, 3);

Fraction f2(7.2); Fraction f3;

cout &lt;&lt; “Fraction f1(5, 3) = ” &lt;&lt; f1 &lt;&lt; endl; cout &lt;&lt; “Fraction f2(7.2) = ” &lt;&lt; f2 &lt;&lt; endl; cout &lt;&lt; “Fraction f3 = ” &lt;&lt; f3 &lt;&lt; endl;

// BASIC ASSIGNEMENT OPERATOR // ————————–

cout &lt;&lt; “Assignment (Before): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl; f3 = f1; cout &lt;&lt; “Assignment (After): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl;

f3 = Fraction::sc_fUnity;

// UNARY ARITHMETIC OPERATORS // ————————-f3 = -f1; cout &lt;&lt; “Unary Minus: f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl;

// Pre-decrement. Dividendo f3 = Fraction::sc_fUnity;

cout &lt;&lt; “Pre-Decrement (Before): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl; f3 = –f1;

cout &lt;&lt; “Pre-Decrement (After): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl;

// Post-decrement. Lazy Dividendo f3 = Fraction::sc_fUnity;

cout &lt;&lt; “Post-Decrement (Before): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl; f3 = f1–;

cout &lt;&lt; “Post-Decrement (After): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl;

// Pre-increment. Componendo f3 = Fraction::sc_fUnity;

cout &lt;&lt; “Pre-Increment (Before): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl; f3 = ++f1; cout &lt;&lt; “Pre-Increment (After): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl;

// Post-increment. Lazy Componendo f3 = Fraction::sc_fUnity; cout &lt;&lt; “Post-Increment (Before): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl; f3 = f1++; cout &lt;&lt; “Post-Increment (After): f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; endl; // BINARY ARITHMETIC OPERATORS USING FRIEND FUNCTIONS // ————————————————-f1 = Fraction(5, 12); f2 = Fraction(7, 18); f3 = f1 + f2; cout &lt;&lt; “Binary Plus: f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1

&lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

f1 = Fraction(16, 3); f2 = Fraction(22, 13); f3 = f1 – f2; cout &lt;&lt; “Binary Minus: f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1

&lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

f1 = Fraction(5, 12); f2 = Fraction(18, 25); f3 = f1 * f2; cout &lt;&lt; “Multiply: f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1

&lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

f1 = Fraction(5, 12); f2 = Fraction(7, 18); f3 = f1 / f2; cout &lt;&lt; “Divide: f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1

&lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

f1 = Fraction(5, 12); f2 = Fraction(7, 18); f3 = f1 % f2; cout &lt;&lt; “Residue: f3 = ” &lt;&lt; f3 &lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

// BINARY RELATIONAL OPERATORS // ————————–f1 = Fraction(5, 12); f2 = Fraction(7, 18); bool bTest = f1 == f2; cout &lt;&lt; “Equal: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

bTest = f1 != f2; cout &lt;&lt; “Not Equal: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

bTest = f1 &lt; f2; cout &lt;&lt; “Less: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

f1 = Fraction(5, 12); f2 = Fraction(7, 18); f3 = Fraction(5, 12); bTest = f1 &lt;= f2; cout &lt;&lt; “Less Equal: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

bTest = f1 &lt;= f3; cout &lt;&lt; “Less Equal: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f3 = ” &lt;&lt; f3 &lt;&lt; endl;

bTest = f1 &gt; f2; cout &lt;&lt; “Greater: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

bTest = f1 &gt;= f2; cout &lt;&lt; “Greater Equal: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f2 = ” &lt;&lt; f2 &lt;&lt; endl;

bTest = f1 &gt;= f3; cout &lt;&lt; “Greater Equal: Test = ” &lt;&lt; ((bTest)? “true”: “false”)

&lt;&lt; “. f1 = ” &lt;&lt; f1 &lt;&lt; “. f3 = ” &lt;&lt; f3 &lt;&lt; endl;

return;

}

// End-of-File: TestFraction.cxx

// File: Main.cxx

// Contains: int main()

/************ C++ Headers ************************************/

#include &lt;iostream&gt; using namespace std;

/************ PROJECT Headers ********************************/

#include “Fraction.hxx” void TestFraction();

int main() { TestFraction();

return 0;

}

// End-of-File: Main.cxx
