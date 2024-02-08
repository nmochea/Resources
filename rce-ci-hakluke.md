### Remote Code Execution vs. Remote Command Execution vs. Code Injection vs. Command Injection vs. RCE

**Command Injection** is a type of vulnerability that allows an attacker to inject operating system commands directly into an application and have them execute (the type of commands that one would enter into a Bash or Powershell terminal).

**Code Injection** is a type of vulnerability that allows an attacker to inject server-side code directly into an application and have it execute. For example, injecting PHP, Python or server-side JavaScript into eval().

**Remote Code Execution** is the impact of a vulnerability that allows an attacker to execute code remotely, but it is not the actual vulnerability itself. The vulnerability does not necessarily need to be a Code Injection vulnerability, it could be something else, such as an arbitrary file upload that allows an attacker to upload a web shell.

**Remote Command Execution** is the impact of a vulnerability that allows an attacker to execute commands remotely, but it is not the vulnerability itself. Again, the vulnerability does not necessarily need to be a Command Injection vulnerability, it could be any vulnerability that results in an attacker being able to execute commands.

It should be noted that typically, if a vulnerability allows remote code execution, then it will also allow remote command execution, and vice versa.

**RCE** is a generic term that can refer to either Remote Code Execution OR Remote Command Execution. In other words, RCE is the impact of a vulnerability that allows an attacker to execute code and/or commands remotely.

**TL;DR:** Injection is a type of vulnerability, execution is a type of impact. Command is a shell command, while code is some type of server-side code other than shell commands, such as PHP. RCE is used interchangeably to mean remote (code|command) execution.
