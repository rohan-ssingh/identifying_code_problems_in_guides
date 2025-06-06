# identifying_code_problems_in_guides

This project will be exploring a tool that automatically determines if a programming guide contains vulnerabilities, deprecated code, etc. 

Literature Review:

1. https://lup.lub.lu.se/student-papers/search/publication/9178282

A thesis which fine-tuned a HuggingFace model to detect vulnerabilities in several different popular languages including Python, JS, Go, etc. Showed promise in an LLM's ability to be utilized in identifying malicious code. Also referenced additional studies involving arduino and other use cases.

2. Espinha Gasiba, T., Iosif, A.-C., Kessba, I., Amburi, S., Lechner, U., & Pinto-Albuquerque, M. (2024). May the Source Be with You: On ChatGPT, Cybersecurity, and Secure Coding. Information, 15(9), 572. https://doi.org/10.3390/info15090572

A project which explored GPT 3 and 4 against vulnerabilites and bugs such as the overflow buffer bug, along with other errors in code. This paper provides examples of common errors including a discussion of important problems being presented in the OWASP and MITRE AT&CK framework. Conclusions showed that the program using GPT 4 was able to identify most of vulnerability issues surrounding the various test cases but still had some difficulty grasping all of them.
