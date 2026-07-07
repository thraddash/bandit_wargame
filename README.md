## 🎯 OverTheWire: Bandit

The **Bandit** wargame is a beginner-focused **Capture The Flag (CTF)** challenge hosted by [OverTheWire](https://overthewire.org).  Designed for absolute beginners, it teaches **Linux fundamentals** and **cybersecurity basics** through 34 progressive levels. 

**Key Features:**
- **Gamified Learning:** Solve puzzles to find passwords ("flags") that unlock subsequent levels via SSH.
- **Skill Building:** Master essential commands (`ls`, `cat`, `grep`, `find`, `ssh`) and concepts like file permissions, hidden files, and data encoding. 
- **Safe Environment:** Provides a risk-free playground to practice command-line navigation and system administration tasks. 

> **Goal:** Connect to `bandit.labs.overthewire.org` and advance from Level 0 to Level 34 by solving each challenge.   
<br>

## https://overthewire.org/wargames/bandit/bandit0.html
```brew install sshpass```<br>
<b>user:password </b>are located inside the file <b>notes.txt , notes.txt includes notes, cmd lines, and solutions for each levels</b>

### Shortcut CMD to ssh into next host server
[replace username to connect to next host server:]<br>
example: bandit0, bandit1, etc..<br>
```
LEVEL=bandit0; sshpass -p "$(grep "^${LEVEL}:" notes.txt | cut -d':' -f2)" ssh -p 2220 ${LEVEL}@bandit.labs.overthewire.org
```
