---
layout: post
title: "Multipurpose Internet Mail Extensions (MIME) Security with PGP or SMTP"
description: "Uses of PGP/MIME and S/MIME in MIME security"
comments: true
keywords: "pgp, mime, email, smime, pgpmime"
---

This page is about Multipurpose Internet Mail Extensions (MIME) Security with PGP (PGP/MIME) or SMTP (S/MIME).

Originally, I had PGP/MIME set up but what about if a recipient does not have PGP/MIME set up on their end?  I started looking into S/MIME and have since started signing my emails.

Since you cannot run PGP/MIME and S/MIME together, you only have a choice of implementing one rather.


# What is PGP/MIME (or MIME with PGP)

RFC 3156 illustrates this form of MIME security.

PGP/MIME is integrating PGP (Pretty Good Privacy) with MIME. 

There are three content types to implement:
1. application/pgp-encrypted
2. application/pgp-signature
3. application/pgp-keys


## Setting up PGP/MIME



# What is S/MIME (or MIME with SMTP)


## Setting up S/MIME



# What is the differences between the two?



# Which one should I implement?



> Your mileage may vary.  This content is constantly under development and may change at any time.
