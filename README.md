# identifying_code_problems_in_guides

This project will be exploring a tool that automatically determines if a programming guide contains vulnerabilities, deprecated code, etc. 

Literature Review:

1. https://lup.lub.lu.se/student-papers/search/publication/9178282

A thesis which fine-tuned a HuggingFace model to detect vulnerabilities in several different popular languages including Python, JS, Go, etc. Showed promise in an LLM's ability to be utilized in identifying malicious code. Also referenced additional studies involving arduino and other use cases.

2. Espinha Gasiba, T., Iosif, A.-C., Kessba, I., Amburi, S., Lechner, U., & Pinto-Albuquerque, M. (2024). May the Source Be with You: On ChatGPT, Cybersecurity, and Secure Coding. Information, 15(9), 572. https://doi.org/10.3390/info15090572

A project which explored GPT 3 and 4 against vulnerabilites and bugs such as the overflow buffer bug, along with other errors in code. This paper provides examples of common errors including a discussion of important problems being presented in the OWASP and MITRE AT&CK framework. Conclusions showed that the program using GPT 4 was able to identify most of vulnerability issues surrounding the various test cases but still had some difficulty grasping all of them.

3. Omer Said Ozturk, Emre Ekmekcioglu, Orcun Cetin, Budi Arief, and Julio Hernandez-Castro. 2023. New Tricks to Old Codes: Can AI Chatbots Replace Static Code Analysis Tools? In Proceedings of the 2023 European Interdisciplinary Cybersecurity Conference (EICC '23). Association for Computing Machinery, New York, NY, USA, 13–18. https://doi.org/10.1145/3590777.3590780

This paper compared ChatGPT API against static code analysis programs to see its accuracy. While the OpenAI API did outperform the static code analysis programs, the API had a high false positive rate, indicating that any future project must work to minimize the possible false positives produced by the algorithm.

4. Zhang, J., Bu, H., Wen, H. et al. When LLMs meet cybersecurity: a systematic literature review. Cybersecurity 8, 55 (2025). https://doi.org/10.1186/s42400-025-00361-w

A review detailling various methods: traditional machine learning and more recently developed Large Language Models (such as OpenAI's GPT) to be used for malicious code detection. The reivew, as a whole, found that LLM's are better than traditional machine learning methods in identifying and fixing malicious code, however, LLM's struggle with a high false positive rate. This means that a project would need to ensure that any discovered potential malicious code examples would need to be verified (*possibly through calls from other models to validate the findings?*) to ensure that the problem is truly a problem and not simply a false positive.

5. https://research.tees.ac.uk/ws/portalfiles/portal/77055020/1-s2.0-S0957417423016858-main.pdf

This tool analyzes a website's source code to check its embedded URLs and code to see if it is possibly a website used for phishing. It takes in a site's URL along with its HTML code, and then converts it into an embedding, and then uses a convolutional neural network, trained on data from Alexa, to see if it could possibly be related to phishing usage. It achieved a pretty high accuracy compared to other methods.
