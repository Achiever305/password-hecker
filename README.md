

🔐 Password Strength & Data Breach Checker

By Iloh Chijioke Victor

📌 Project Overview

This project is a Python-based cybersecurity tool designed to help users evaluate the strength of their passwords and determine whether those passwords have appeared in known data breaches. It integrates secure hashing techniques and privacy-preserving breach detection using the Have I Been Pwned (HIBP) API.

The goal is to improve password awareness while ensuring that sensitive user data is never exposed.

❗ Problem Statement

Weak or reused passwords are one of the leading causes of account compromise. Many users unknowingly use passwords that:
	•	Are easily guessable
	•	Follow predictable patterns
	•	Have already been exposed in previous data breaches

There is a lack of accessible tools that allow users to safely verify password security without revealing their actual passwords.

💡 Solution

I developed a command-line application that:
	•	Evaluates password strength based on complexity
	•	Checks passwords against known data breaches using HIBP
	•	Preserves privacy through SHA-1 hashing and the K-Anonymity model

The tool provides actionable feedback while maintaining secure input handling and isolation through a Python virtual environment.

🔐 Security & Privacy Approach
	•	Passwords are hashed locally using SHA-1
	•	Only the first 5 characters of the hash are sent to the HIBP API
	•	The full password or full hash is never transmitted
	•	Breach detection is done by comparing returned hash suffixes locally

This ensures user privacy while still enabling accurate breach detection.

⚙️ How the System Works
	1.	User enters a password
	2.	Password strength is analyzed
	3.	SHA-1 hash is generated
	4.	Hash prefix is sent to HIBP API
	5.	Matching breach data is returned
	6.	User is notified if the password was found in breaches

🧪 Example Output

Input: P@ssword123
Strength: Medium
Breach Status: Found in 23 data breaches
Recommendation: Use a longer, unique password with higher complexity

🛠 Tools & Technologies
	•	Python 3
	•	Requests library
	•	Kali Linux terminal
	•	Python virtual environment (venv)
	•	Have I Been Pwned (HIBP) API

🖥️ Environment Setup (Kali Linux)
	•	Installed python3-venv
	•	Created and activated a virtual environment
	•	Installed required dependencies
	•	Developed and tested the Python script within the isolated environment

🚀 Key Takeaways
	•	Strong passwords significantly reduce security risks
	•	Users should avoid passwords already exposed in breaches
	•	Privacy-preserving techniques like K-Anonymity are essential in security tools
	•	Secure design can be implemented even in small-scale projects

🔮 Future Improvements
	•	Graphical User Interface (GUI)
	•	Advanced entropy-based strength analysis
	•	Real-time password feedback
	•	Support for additional breach databases

