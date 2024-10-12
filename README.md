# comp2022 Assignment 3

## 1. General Information
- This assignment is due in Week 10 and should be submitted to Gradescope.
- All work must be done individually without consulting anyone else’s solutions in accordance with the University’s “Academic Dishonesty and Plagiarism” policies.
- Go to the last page of this document and read the Submission Instructions. For clarifications and updates, monitor “Assignment FAQ”.

## 2. Problem 1 (10 marks)
### 2.1. Deterministic Turing Machine M over $\sum = \{a, b\}$
- **Transition Rules**:
```
0 _ _ L 1
0 * * R 0
1 b _ L 2
2 a _ L 3
1 _ _ * halt_accept
3 _ _ R 0
3 * * L 3
```
### 2.2. Tasks
- **(a) (5 marks)** State five strings that are in $L(M)$, and five that are not. The strings should be over Σ.
- **(b) (5 marks)** Provide a low level description in Morphett notation of a (1 - tape deterministic) Turing Machine for the language that has time complexity at most $5n + 5$.

## 3. Problem 2 (10 marks)
### 3.1. Nondeterministic Turing Machine N over $\sum = \{a, b\}$
- **Transition Rules**:
```
0 _ _ * halt-reject
0 a a r 0
0 b b r 0
0 b x l 1
1 x x l 1
1 a x r 2
1 b x r 2
1 _ _ r 4
2 x x r 2
2 a x r 3
2 b x r 3
2 _ _ * halt-reject
3 x x r 3
3 a x l 1
3 b x l 1
3 _ _ * halt-reject
4 x x r 4
4 a a * halt-reject
4 b b * halt-reject
4 _ _ * halt-accept
```
### 3.2. Tasks
- **(a) (5 marks)** State five strings that are in $L(N)$, and five that are not. The strings should be over Σ.
- **(b) (5 marks)** Provide a low level description in Morphett notation of a (1 - tape deterministic) Turing Machine for the language.

## 4. Problem 3 (30 marks)
For each of the following languages over the input alphabet $\sum = \{a, b, c\}$, provide a low level description in Morphett notation of a (1 - tape deterministic) TM for the language.
### 4.1. The language of non - empty strings where the final character appears at most 3 times in the string (including the final character).
### 4.2. The language of strings of the form $a^{n}b^{n}c^{n}a^{n}$ for $n ≥ 1$.
### 4.3. The language of strings that can be turned into a palindrome by replacing at most two characters by other characters.
### 4.4. The language of strings for which the longest substring that matches $a^{*}$ is longer than the longest substring that matches $b^{*}$.
### 4.5. The language of strings of the form $uvcvu$ where $u, v\in \{a, b\}^{*}$.
### 4.6. The language of strings of the form $uvw$ where $v$ is a non - empty string with the same number of $a$s, $b$s, and $c$s.

## 5. Problem 4 (5 marks + 5 bonus marks)
### 5.1. (5 marks) Provide a low level description in Morphett notation of a (1 - tape deterministic) TM over input alphabet $\sum = \{a\}$ that accepts every string, has at most 20 states, and has time complexity $f(n)$ such that $2^{n}≤f(n)≤2^{2n + 1}$ for all $n$.
### 5.2. (5 bonus marks) Provide a low level description in Morphett notation of a (1 - tape deterministic) TM over input alphabet $\sum = \{a\}$ that accepts every string, has at most 40 states, and has time complexity exactly $2^{n}$.

## 6. Problem 5 (15 marks)
### 6.1. (5 marks) Prove that the language $\{M, x: M$ halts on $x$ in exactly $77n$ steps for some integer $n > 0\}$ is undecidable.
### 6.2. (10 marks) Consider the following specification. The inputs are Turing machines over input alphabet $\sum = \{\bar{a}, \bar{b}\}$
- **(a)** If the input is a Turing machine $M$ that accepts some input, the output should be any string $x$ that $M$ accepts.
- **(b)** If the input is a Turing machine $M$ that does not accept any input, the output should be any string $x$. (There still must be an output, i.e., the machine satisfying this specification must halt.)
Prove or disprove whether there exists a Turing Machine that halts on every input and satisfies this specification.

## 7. Submission Instructions
- Problems 1, 2, 3 and 4 are autograded. Ensure submission is formatted correctly for the autograder. An incorrectly formatted submission for a question will receive zero marks for that question. A scaffold will be provided on Ed with the file names the autograder expects.
- Problem 1.1, 2.1 format: The first line of each answer should contain a comma separated sequence of five strings that are in the language, and the second line should contain a comma separated sequence of five strings that are not in the language.
- Problem 1.2, 2.2, 3, 4 format (TMs): All TMs should be deterministic, single - tape, and doubly - infinite. Use Morphett’s format for low - level descriptions. The initial state must be 0. Include an explicit transition to halt - reject when rejecting a string.
- Problem 5 format: Problem 5 is handgraded. Submit a single typed pdf (no pdf containing text as images, no handwriting). Type your student ID at the top of the first page of each pdf. Do not type your name. Do not include a cover page. Submit only your answers to the questions. Do not copy the questions. Your pdf must be readable by Turnitin.
# comp2022 A3

# CS Tutor | 计算机编程辅导 | Code Help | Programming Help

# WeChat: cstutorcs

# Email: tutorcs@163.com

# QQ: 749389476

# 非中介, 直接联系程序员本人
