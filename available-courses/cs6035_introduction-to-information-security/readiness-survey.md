# CS 6035 Prerequisites

Two prerequisite documents are linked from the OMSCS course page's "Before Taking This Class" section:

- Source 1: [Basic Information Security Prerequisites (Google Doc)](https://docs.google.com/document/d/1YxQGox5FMVeO2J01ZKbkq9cSGjNMk7SW43eF4zL78LQ/edit)
- Source 2: [Project and Technical Prerequisites (Google Doc)](https://docs.google.com/document/d/1x0waLzR4-GfYWiEeGBZruJLIAY8xIczyGMF4JT7al2s/edit)

## Basic Information Security Prerequisites

CS 6035 assumes classical computer science (CS) background, preferably from an accredited undergraduate CS program. A wide variety of CS and programming knowledge is required to be successful in project coursework. These are the prerequisites:

### Computer Organization and Architecture
- Be able to describe what a stack, heap (high-level memory organization, not the data structure), registers, virtual memory, and processes are.
- Understanding of the stack's role in program execution.
- How memory is allocated both statically and dynamically.
- Be able to follow basic assembly language as it applies to compiled code (C).

### Programming
- Experience programming in a high-level language. CS 6035 projects specifically use C, Python 3.x, Java, HTML/JS/PHP, and SQL in various contexts. The ability to pick up programming languages on the fly will benefit learning outcomes.
- Experience with algorithms, data structures, and basic time complexity.
- The majority of advanced debugging involves execution analysis of C programs, with GNU Debugger (`gdb`) used as the debugging platform. Knowing how to use `gdb` to dump registers/stack memory, set breakpoints to follow the execution path, and analyze compiled assembly will be very helpful.
- The ability to translate pseudocode into applied, functioning code — even in a programming language you might not be familiar with and are actively learning.

### Mathematics
- Understanding of public-key cryptography, basic hashing mechanisms, discrete mathematics, number-system foundations, and modular arithmetic can be very helpful to learning outcomes.

### Misc Computer Skills
- Working knowledge of VirtualBox VMs and their intermediate management.
- Basic understanding of how to navigate a Linux shell and execute basic command-line tools.
- How to compile C programs, write and compile Java classes, interpret Python code, use built-in browser tools to analyze web-development interactions between integrated technologies (e.g., HTML and JS), and understand basic SQL queries.
- Basic understanding of Linux network protocols and command-line tools (`nslookup`, `dig`, DNS); knowledge of `wireshark` is helpful.
- Familiarity with the Microsoft Windows registry — its function, how to change it, and the consequences of such changes.

### Knowledge Gaps
Gaps in one's overall skill set and predicate knowledge may require significant time and effort to overcome, on top of the time required to study course-specific materials. Due to the scale of the class and program, students are expected to fill in gaps in their own knowledge; instructors will not have resources to provide remedial assistance. These hardships are not insurmountable, even without a CS background, if sufficient effort is applied.

### Useful Resources
- `gdb-example-ncurses.html` (GDB)
- [phrack.org/issues/49/14.html](http://phrack.org/issues/49/14.html) (buffer overflow concepts)
- [cprogramming.com/gdb.html](https://www.cprogramming.com/gdb.html) (GDB)
- [docs.python.org/3/tutorial/](https://docs.python.org/3/tutorial/)
- [hacksplaining.com](https://www.hacksplaining.com) (SQL injection / JavaScript / XSS / CSRF vulnerabilities)

## Suggested Background (course page)

An undergraduate degree in computer science or a related field is assumed, per Georgia Tech admission criteria. The OMSCS course page's "Before Taking This Class" section summarizes the concrete working knowledge expected: C (memory management, stack/heap), Python (scripting, exploit tools such as pwntools), JavaScript, SQL/T-SQL; computer architecture and assembly, operating systems, network protocols (HTTP/HTTPS, TCP/IP), and cryptographic concepts; plus security-specific skills in web security (XSS/CSRF), binary analysis/exploitation (GDB, pwndbg), database security (SQL injection), and malware analysis. Full detail is in the two prerequisite documents above.

## Project and Technical Prerequisites

Per-project technical prerequisites for CS 6035 coursework.

### Binary Exploitation
- Working knowledge of C and familiarity with x86_64/aarch64 architecture.
- Understanding of registers, memory allocation, and hexadecimal/binary representation.
- Ability to read assembly language at a basic level.
- Debugging proficiency, particularly with `gdb`.
- Linux command-line competency and VirtualBox VM configuration skills.

### Log4Shell
- Basic knowledge of Java and remote-code-execution concepts.
- JNDI/LDAP familiarity within Java contexts.
- Networking fundamentals: IP addresses, ports, and client-server models.
- Application logging analysis.
- Basic understanding of REST APIs and how they are called.
- `curl` proficiency for GET requests and header manipulation.
- Linux command execution for Docker, JAR files, and Python; VirtualBox management.

### Malware Analysis
- Linux command-line skills and Python scripting.
- Understanding of isolated environments and honeypot systems.
- Knowledge of operating-system components and malware interaction.
- Conceptual understanding of process lineage, including parent/child relationships.

### Machine Learning on CLAMP
- Python programming familiarity with functions and basic operators.
- Basic understanding of NumPy and pandas.
- Data-science concepts including preprocessing and train/test splits.
- Knowledge of supervised/unsupervised learning models and model-comparison metrics.

### RSA Cryptography
- Linux command execution and Python scripting.
- Familiarity with modular arithmetic and discrete math.
- Cryptography primitives and hashing functions.
- Unit-testing script knowledge.

### Man in the Middle
- TCP/IP network stack and protocol understanding.
- Basic understanding of Wireshark for PCAP analysis.
- Python programming with the `pyshark` module.
- FTP and web-server file operations.

### Web Security
- Linux file editing and viewing proficiency.
- Intermediate understanding of web technologies (HTML, JavaScript, PHP).
- SQL fundamentals and database connectivity.
- REST API concepts and string manipulation with regex.

### API Security
- Basic understanding of web-based APIs using REST.
- JSON payload creation and reading.
- OAuth, JWT tokens, and CORS concepts.
- API testing tools such as Swagger, Fiddler, or Postman.

### Database Security
- Database schema familiarity with Microsoft SQL Server.
- T-SQL understanding.
- JavaScript and web-development debugging tools.
