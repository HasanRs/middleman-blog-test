---
title: Journey to the Cryptography
date: 2020-07-01T17:20:32.054Z
description: Imagine that two people who share an important secret have to
  leave. So they need to share private information remotely. But let's say that
  Fatma, who eavesdrops, also wants this information and can reach the messages
  of the two.
image: /images/uploads/93473.jpg
---
Imagine that two people who share an important secret have to leave. So they need to share private information remotely. But let's say that Fatma, who eavesdrops, also wants this information and can reach the messages of the two. Therefore, Ayşe decides to communicate with a letter written in different secret codes. Ayşe first locks her message in a box and then only she and Ahmet knows the combination of the lock she uses. We call this encryption. Then the locked message is sent to Ahmet. When Ahmet receives the box, he opens it with the code they found before.
We call decoding. When we do not use physical locks and start using passwords instead, cryptography happens. You can think of them as virtual locks. Cryptos enable Ayşe and Ahmet to mess up their messages and then resolve it. So even if Fatma reaches the message, the message will be safe because the message will be meaningless to her. Cryptography has been used for thousands of years. It was used in wars and is still at the heart of the worldwide communications network. To better understand the great story of cryptography, we need to understand two old ideas about number and probability theories. 

![](/images/uploads/white-digital-matrix-binary-code-numbers-background_1017-25332.jpg "Probability")

Let me talk about some basic principles.

For a given event A, probability p (A) is represented by a number ranging from 0 to 1. For an impossible event, the probability is 0 and the probability of an event that will happen is 1.

<br>

| Event                             | Probability                                                                                                                                                                                                                                                                                                                     |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Probability for event A           | ![{\\displaystyle \\mathbb {P} (A)\\in \[0,1\]\\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/d6413f6dd54ea8f1f55b4b983d32be9c0a4228ed)                                                                                                                                                                           |
| Probability for no A event        | ![{\\displaystyle \\mathbb {P} (A^{c})=1-\\mathbb {P} (A)\\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/748635725631ca0f591fbc87ef69c025ad87865c)                                                                                                                                                                |
| The probability to be **A or B**  | ![{\\displaystyle {\\begin{aligned}\\mathbb {P} (A\\cup B)&=\\mathbb {P} (A)+\\mathbb {P} (B)-\\mathbb {P} (A\\cap B)\\\\\\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/6579fe8e780ce85c26aed879192cded995fb38fa)                                                                                    |
| The probability to be **A and B** | ![{\\displaystyle {\\begin{aligned}\\mathbb {P} (A\\cap B)&=\\mathbb {P} (A\|B)\\mathbb {P} (B)\\\\&=\\mathbb {P} (A)\\mathbb {P} (B)\\qquad {\\mbox{eger A ve B bagimsizlarsa}}\\\\\\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/e05205e10db664e244d81101c61ed1d13eeb65ed)(if A and B independent) |
| A given B (B conditional A)       | ![{\\displaystyle \\mathbb {P} (A\|B)={\\frac {\\mathbb {P} (A\\cap B)}{\\mathbb {P} (B)}}\\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/1946ffded341798cabae8215a1ab9a13f83bb41d)                                                                                                                               |

<br><br>

*A new problem arises in the twentieth century. What if Ayşe and Berk never come together to share the key?*

> Source: Khan Academy Turkey, Wikipedia