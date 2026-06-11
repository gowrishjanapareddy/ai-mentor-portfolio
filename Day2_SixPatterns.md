# Day 2 — Lab 2A: Six Prompt Patterns

## Pattern 1 — Persona

### Prompt

You are a senior placement coach at Aditya University. You have prepared 200 B.Tech CSE students for TCS, Infosys, and Cognizant placement interviews. A 3rd-year CSE student with 7.5 CGPA asks you about Big-O notation. Explain it the way you would in a 1-on-1 prep session — concrete, conversational, exam-relevant.

### Best Output

Big-O notation describes how an algorithm's running time grows as the input size increases. Think of it as a way to measure efficiency. For example, if you search for a number in a list of n items by checking each element one by one, the time complexity is O(n). If you use nested loops over the same list, the complexity becomes O(n²). Interviewers ask about Big-O because it helps them evaluate whether you can write scalable and efficient code.

### Self Score

4/5

### Peer Score

8/10

---

## Pattern 2 — Few-Shot

### Prompt

Here are example explanations from a placement coach:

Q: What is recursion?
A: A function calling itself with a smaller problem. Like Russian dolls — open one, find a smaller one inside. Stops at a base case. Example: factorial.

Q: What is a stack?
A: LIFO data structure. Push to add, pop to remove. Like a stack of plates — you take from the top.

Q: What is Big-O notation?
A:

### Best Output

Big-O notation tells us how the time or memory used by an algorithm grows as input size increases. Think of it like measuring how much longer a task takes when the amount of work doubles. For example, checking every item in a list is O(n), while comparing every item with every other item is O(n²).

### Self Score

4/5

### Peer Score

8/10

---

## Pattern 3 — Chain of Thought

### Prompt

Explain Big-O notation to a placement interview candidate.

Step 1: Define Big-O in one sentence.

Step 2: Give one concrete example with code.

Step 3: Explain why interviewers ask about it.

Step 4: Summarize in three sentences.

### Best Output

Step 1: Big-O notation describes how an algorithm's performance changes as input size grows.

Step 2:

```python
def find_max(arr):
    max_val = arr[0]
    for num in arr:
        if num > max_val:
            max_val = num
    return max_val
```

This algorithm checks each element once, so its time complexity is O(n).

Step 3: Interviewers ask about Big-O because efficient algorithms are important when handling large amounts of data.

Step 4: Big-O helps compare algorithm efficiency. It predicts performance as input size grows. Understanding it helps developers write scalable programs.

### Self Score

5/5

### Peer Score

9/10

---

## Pattern 4 — Structured Output

### Prompt

Explain Big-O notation for a placement interview.

Return ONLY valid JSON with this exact shape:

{
"definition": "one-sentence definition",
"intuition": "concrete analogy",
"code_example": "Python snippet showing O(n) and O(n²)",
"common_pitfall": "what students get wrong",
"interview_test_question": "a follow-up question an interviewer might ask"
}

### Best Output

{
"definition": "Big-O notation describes how an algorithm's running time or memory usage grows as input size increases.",
"intuition": "Walking through every student in a classroom is O(n), while comparing every student with every other student is O(n²).",
"code_example": "for i in arr: print(i) # O(n)\nfor i in arr:\n for j in arr:\n  print(i,j) # O(n²)",
"common_pitfall": "Students often focus on exact execution time instead of growth rate.",
"interview_test_question": "What is the time complexity of binary search and why?"
}

### Self Score

5/5

### Peer Score

10/10

---

## Pattern 5 — System Prompt

### System Prompt

You are a senior placement coach for B.Tech CSE students at an Indian engineering college. You prepare students for TCS, Infosys, and Cognizant interviews. You explain technical concepts in 50–80 words maximum, conversationally, with one concrete code example.

### User Prompt

Explain Big-O notation.

### Best Output

Big-O notation tells us how an algorithm's performance changes as input size grows. For example, a loop that scans every element in an array has O(n) complexity because it visits each item once. Interviewers ask about Big-O to check whether you can analyze and optimize code. Remember common complexities like O(1), O(log n), O(n), and O(n²).

### Self Score

4/5

### Peer Score

8/10

---

## Pattern 6 — Prompt Chaining

### Conversation 1 Output

1. Definition of Big-O
2. Common time complexities
3. Comparing algorithms
4. Time vs space complexity
5. Importance in interviews

### Conversation 2 Output

Big-O notation measures how algorithm performance changes with input size.

Common complexities include O(1), O(log n), O(n), O(n log n), and O(n²), each representing different growth rates.

Big-O helps compare multiple solutions to the same problem and select the most efficient one.

Time complexity measures execution time growth, while space complexity measures memory growth.

Interviewers use Big-O questions to assess analytical thinking and coding efficiency.

### Conversation 3 Output

Big-O notation explains how an algorithm's performance changes as input size grows. Common complexities include O(1), O(log n), O(n), and O(n²). It helps compare algorithms and choose efficient solutions. Developers must understand both time and space complexity when optimizing programs. Interviewers ask Big-O questions to evaluate problem-solving and scalability awareness.

Practice Question: What is the time complexity of binary search?

### Self Score

5/5

### Peer Score

9/10

---

# Reflection

For my placement-prep students, I will use Persona and Prompt Chaining most often.

Persona helps tailor explanations to the student's academic level, interview goals, and background. Prompt Chaining produces higher-quality responses by breaking complex topics into smaller tasks before combining them into a polished explanation. Together, these patterns make AI-generated learning content more accurate, structured, and useful for placement preparation.
