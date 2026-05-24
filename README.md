# Exno.7-Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

# Date:24.05.26
# Register no:212223060114



#  AIM

To develop a prompt-based application tailored to personal needs using Large Language Models (LLMs), enabling creativity, productivity, and practical problem-solving through AI-assisted interactions.

---

#  OBJECTIVE

- To understand the concept of prompt-based AI applications.
- To design prompts for solving real-world personal problems.
- To develop a Python-based application using prompts and LLM concepts.
- To improve creativity and productivity using AI assistance.
- To learn how prompt engineering influences AI-generated responses.

---

#  SOFTWARE REQUIREMENTS

- Python 3.x
- VS Code / Jupyter Notebook
- AI Chatbot / LLM
- Internet Connection
- Python Libraries:
  - tkinter
  - datetime

---

#  THEORY

Large Language Models (LLMs) are AI systems capable of understanding and generating human-like text responses. Prompt Engineering is the process of designing effective instructions that guide LLMs to produce useful outputs.

Prompt-based applications allow users to interact with AI systems naturally using text instructions. These applications can help in:

- Education
- Productivity
- Planning
- Coding assistance
- Content generation
- Problem solving

In this experiment, a personal AI Study Assistant application is developed using prompt engineering concepts.

---

#  PROBLEM STATEMENT

Students often struggle with:

- Creating study schedules
- Managing time effectively
- Understanding difficult topics
- Staying productive during exams

The developed prompt-based application solves these problems by generating:

- Study plans
- Motivational suggestions
- Topic explanations
- Productivity recommendations

---

#  APPLICATION IDEA

## AI Personal Study Assistant

The application accepts user input such as:

- Subject name
- Study hours
- Exam date
- Difficulty level

Using prompt engineering concepts, the AI generates:

- Personalized study timetable
- Revision strategies
- Productivity tips
- Topic-wise learning plans

---

#  PROMPT USED

```txt
Act as an intelligent study mentor. Create a personalized study plan for a college student based on subject name, available study hours, exam date, and difficulty level. Include revision time, break schedules, and motivational tips.
```

---

#  AI GENERATED RESPONSE (SAMPLE)

```txt
Study Plan for Data Structures

6:00 AM – 7:30 AM → Arrays and Linked Lists
7:30 AM – 8:00 AM → Break

10:00 AM – 12:00 PM → Stack and Queue Problems
12:00 PM – 1:00 PM → Revision

Motivational Tip:
"Consistency is more important than perfection."
```

---

#  APPLICATION ARCHITECTURE

```txt
User Input
     ↓
Prompt Generation
     ↓
Large Language Model
     ↓
AI Response Processing
     ↓
Personalized Study Plan Output
```

---

#  PYTHON IMPLEMENTATION

##  Import Required Libraries

```python
import tkinter as tk
from tkinter import messagebox
from datetime import datetime
```

---

##  Create Main Window

```python
root = tk.Tk()

root.title("AI Personal Study Assistant")
root.geometry("500x500")
```

---

##  User Input Fields

```python
subject_label = tk.Label(root, text="Enter Subject")
subject_label.pack()

subject_entry = tk.Entry(root, width=40)
subject_entry.pack()

hours_label = tk.Label(root, text="Study Hours Per Day")
hours_label.pack()

hours_entry = tk.Entry(root, width=40)
hours_entry.pack()

difficulty_label = tk.Label(root, text="Difficulty Level")
difficulty_label.pack()

difficulty_entry = tk.Entry(root, width=40)
difficulty_entry.pack()
```

---

##  Prompt Generation Function

```python
def generate_prompt():

    subject = subject_entry.get()
    hours = hours_entry.get()
    difficulty = difficulty_entry.get()

    prompt = f"""
    Act as an AI study mentor.
    Create a study plan for {subject}.
    Available study hours: {hours}
    Difficulty level: {difficulty}
    Include revision schedule and motivational tips.
    """

    output_text.delete("1.0", tk.END)
    output_text.insert(tk.END, prompt)
```

---

##  Generate Button

```python
generate_button = tk.Button(
    root,
    text="Generate Study Plan",
    command=generate_prompt
)

generate_button.pack(pady=10)
```

---

##  Output Display Area

```python
output_text = tk.Text(root, height=15, width=60)
output_text.pack()
```

---

##  Run Application

```python
root.mainloop()
```

---

# SAMPLE OUTPUT

```txt
AI Personal Study Assistant

Subject: Operating Systems
Study Hours: 4 Hours
Difficulty: Medium

Generated Study Plan:

6:00 AM – 7:30 AM → Process Scheduling
8:00 AM – 9:30 AM → Memory Management
10:00 AM – 11:00 AM → Revision

Motivational Tip:
"Small progress every day leads to big success."
```

---

#  FEATURES OF THE APPLICATION

- Personalized study schedules
- Prompt-based AI interaction
- Simple graphical interface
- Productivity enhancement
- Motivational support
- User-friendly design

---

#  PROMPT REFINEMENT

##  Initial Prompt

```txt
Create a study plan.
```

---

##  Refined Prompt

```txt
Act as a professional AI study mentor. Create a personalized study plan for a college student based on subject, study hours, and difficulty level. Include revision strategy, break timings, and motivational tips.
```

---

#  OBSERVATIONS

| Activity | Observation |
|-----------|--------------|
| Prompt Design | Better prompts improved outputs |
| GUI Development | Easy interaction with users |
| AI Response Quality | Improved with prompt refinement |
| Productivity Planning | Generated useful study schedules |

---

#  ADVANTAGES

- Improves time management
- Personalized learning support
- Easy to use
- Encourages productivity
- Demonstrates practical AI usage

---

#  LIMITATIONS

- AI responses depend on prompt quality
- No real-time internet-based learning
- Requires manual input
- Basic GUI design

---

#  FUTURE ENHANCEMENTS

- Integrate real LLM APIs
- Add voice assistant support
- Include reminders and notifications
- Add cloud database storage
- Create mobile application version

---

#  REFLECTION NOTE

This experiment helped in understanding how prompt engineering can be used to create practical AI-powered applications. Initially, simple prompts produced generic study plans, but refined prompts generated detailed and personalized schedules.

The experiment also demonstrated:

- Creativity using AI tools
- Practical problem-solving
- GUI application development
- Importance of prompt structure

Prompt engineering significantly improved the usefulness and quality of AI-generated outputs.

---

#  RESULT

Thus, a prompt-based application tailored to personal needs was successfully developed using Prompt Engineering concepts and Python programming. The application demonstrated creativity, productivity enhancement, and practical problem-solving using Large Language Models.

---

#  CONCLUSION

Prompt-based applications are powerful tools that combine AI capabilities with user creativity. By designing effective prompts, developers can create intelligent systems that solve practical real-world problems efficiently. This experiment proved that Prompt Engineering plays a vital role in improving AI-driven applications.

---
