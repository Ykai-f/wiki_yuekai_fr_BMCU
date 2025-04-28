---
title: Feedback and suggestions
description: 
published: true
date: 2025-04-28T20:12:01.077Z
tags: 
editor: markdown
dateCreated: 2025-03-31T11:09:20.861Z
---

# Leave any of your comments and thoughts here!
:p

# Experiences from other users

## 1. Slicing Software Issues

Some users have reported abnormal behavior after slicing with **BMCU**, such as:

- All channels being assigned the same color
- Inability to print using **AMS**

After investigation, this issue was identified as a problem with **Bambu Studio** itself.  
It affects both Windows and Mac versions:

- **Mac**: Versions prior to `2.0.0.95` may encounter this issue.
- **Windows**: Versions prior to `2.03.54` may encounter this issue.

**Recommendations:**

- Upgrade **Bambu Studio** to `2.0.0.95` or higher (Mac) and `2.03.54` or higher (Windows).
- Alternatively, using **Oracle Slicer** is another effective solution to avoid these problems.

---

## 2. Single PTFE Tube Being Pulled Out

Some users reported that a **single PTFE tube** was pulled out, instead of the entire **AMS Lite Hub** being ejected.

**Recommendations:**

- Always check for any abnormal resistance when loading/unloading filaments.
- Ensure that the **metal clip** of the **AMS Lite Hub** properly secures the PTFE tube.
- One user, **David**, reported frequent occurrences on a specific filament channel. After disabling the `Long Retraction During Cut` option, he observed significant improvement for that filament channel.

