# Project 1 README

Student: Srujana Kuppala (921005375)

## Project Status
This the current status of the project:
Number 1 works, Number 2- I am unsure about, Number 3- not done

## Known Issues
The project fails to function properly in number 2. some of the input do not match up to the Gray code and i've tried redoing the circuit and was still unable to fix it. 

## References
* [Build an XOR gate from AND/NOT](https://electronics.stackexchange.com/questions/487529/build-an-xor-gate-from-and-not)
* [Some other link](https://stackoverflow.com)

## Generative AI Use

I used ChatGPT for setting up my Github, I have not used it in a while. 

Prompt 1: How do i connect my repo to my local

Answer 1: Go into your project folder:

cd path/to/project


Initialize Git (if not already):

git init


Connect to GitHub repo:

git remote add origin https://github.com/<username>/<repo-name>.git


Add + commit files:

git add .
git commit -m "Initial commit"


Push to GitHub:

git push -u origin main


That’s it ✅

Changes made 1: I followed the directions and connected my computer to my github. 

For Question 1:
Prompt 2: When to use XNOR and XOR
Answer 2: 1. XOR (Exclusive OR)

Symbol: ⊕

Truth: 1 if exactly one input is 1, 0 otherwise.

Use when: You want to detect differences between two signals.

Examples:

Equality check: If you want to know if two bits are different, use XOR:

A B | A⊕B
0 0 | 0
0 1 | 1  <-- different
1 0 | 1  <-- different
1 1 | 0


Parity generator/checker: XOR all bits to see if the number of 1s is odd.

Simple addition (half-adder): The sum bit of a half-adder is A⊕B.

Mnemonic: XOR = “different → 1, same → 0”

2. XNOR (Exclusive NOR)

Symbol: ⊙ or sometimes written as ¬(A⊕B)

Truth: 1 if inputs are the same, 0 if different.

Use when: You want to detect equality between two signals.

Examples:

Equality check: XNOR outputs 1 when A and B are equal.

A B | A⊙B
0 0 | 1
0 1 | 0
1 0 | 0
1 1 | 1


Comparator circuits: Check if two binary numbers are equal.

Parity check (even parity): You can use XNORs in certain parity circuits.

Mnemonic: XNOR = “same → 1, different → 0”

Changes Made 2: I used my boolean experessions to simplify them into XOR or XNOR gates

For Problem 2:

Prompt 3: can you branch multiple inputs in logism 

Answer 3: Yes! In Logisim, you can branch multiple inputs, but there are some important details to keep in mind:

1. Using Wires to Branch

Direct branching: You can click on a wire and drag it in multiple directions to connect it to several inputs. Logisim allows a single wire to split into multiple destinations.

Note: The wire itself doesn’t “duplicate” the signal; all connected inputs will see the same signal value.

2. Using Splitters (for buses)

If you have a multi-bit wire (bus), you can’t just branch it like a single wire. You need to use a Splitter component.

A splitter lets you break a bus into individual bits or combine bits into a bus.

You can then connect each bit to different inputs as needed.

3. Avoiding Loops

Make sure you don’t create loops (where a wire goes back into itself). Logisim will throw a warning or behave unexpectedly.

4. Practical Tip

If you need to branch to many inputs, it’s often cleaner to use a wire label.

Label one wire (e.g., A) and connect other inputs by drawing a wire with the same label. Logisim treats all same-labeled wires as connected.

Changes made: I understood that I can connect the input pins to multiple gates to build the right boolean equation. 

