# XSS-in-Formidable-4.09.04
Formidable 4.09.04 allows to inject certain HTML Tags like &lt;audio>,&lt;video>,&lt;img>,&lt;a> and&lt;button>.This could allow an unauthenticated, remote attacker to exploit a HTML-injection byinjecting a malicous link. The HTML-injection may trick authenticated users to follow the link. If the Link gets clicked, Javascript code can be executed. The vulnerability is due to insufficient sanitization of the „data-frmverify“ tag for links inthe web-based entry inspection page of affected systems. A successful exploitation incomibantion with CSRF could allow the attacker to perform arbitrary actions on an affected system with the privileges of the user. These actions include stealing the users account by changing his password or allowing attackers to submit their own code through an authenticated user resulting in Remote Code Execution. If an authenticated user who is able to edit Wordpress PHP Code in any kind, clicks the malicious link PHP code can be edited.

[Read Writeup here](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/degoes-consulting/lambdaconf-2015/master/speakers/jdegoes/intro-purescript/presentation.pdf)

# References
* https://drive.google.com/file/d/1R9HyLzJeX4t-CVo8O7kDK3NqVchrTya0/view?usp=drivesdk
* https://drive.google.com/file/d/1R9FSbMS4_i8s_NsUbdQet7PW8fYnV519/view?usp=drivesdk
* https://youtu.be/kBmXCXUInPQ
* https://youtu.be/kx5P6jz6SWo
* https://github.com/Strategy11/formidable-forms/blob/master/changelog.txt
* https://github.com/Strategy11/formidable-forms/pull/335/files
