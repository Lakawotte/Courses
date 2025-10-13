---
aliases:
tags:
category:
cssclasses:
  - hide-meta
---
---
# Definition
## I. Statement

>[!hint] Definition
>$$
>$$

## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
### A. Keys
### ==*Example*==
Let assume that four individuals recorded transaction data on a **[[Blockchain|Ledger]]**. Then, to prevent any false record, individuals should really "sign" their transactions.
One problem could be to ensure that "signatures" aren't copied, i.e computers cannot read any form of key used by the individuals.
### A. Keys
To make *signatures* foolproof, the idea is to store a ==*private key*== and a ==*public key*==. This is, the *private key* is a *string* stored somewhere safe, and on the other hand everyone on the [[Blockchain]] could access the *public key* which is later used to make transactions.
For *signatures* to work, they shall respect two principles :
1. The *signature* is different for each transaction made by the owner
2. The *signature* is based on the *private key*
This is, we can define the function $\mathrm{Sign}$ such that
$$
\mathrm{Sign}(\mathrm{Message,Private Key})=\mathrm{Signature}
$$
To ==verify== the *signature*, one shall use the transaction message and the public key and signature of the sender to recognize them. Thus we have
$$
\mathrm{Ver}(\mathrm{Message,Signature,PublicKey})=\begin{cases}1\,\,\mathrm{if\,Signature\,is\,true}\\0\,\,\mathrm{else}\end{cases}
$$
Now, one could use *brute force* to find the *signature* and thus access all transactions ; so *signatures* are encoded as $256$ bits long messages.

Another problem arises : now messages are transcribed using solid protocol, but even if one does not know the *private key* of the sender, they could just copy the message and still respect the $\mathrm{Ver}$ function.
To counter this, every message is combined with a unique ID, which enters as an argument of the $\mathrm{Sign}$ function.
### B. 
The heart of *hash functions* is that they are "discontinuous". This is, a slight change in the input, and the output is completely different.
#### *==Example==*
Here we will use the $\mathrm{SHA256}$ function. First, let "hello world" be $m_1$ and "hello w0lrd" be $m_2$ :
$$
\begin{split}
\mathrm{SHA256}(m_ 1)_{64}&=\mathrm{d59b1e3bd000b1884b836dda7af86cc4142ad05168cd42db5c788769222a90a9}\\
\mathrm{SHA256}(m_ 2)_{64}&=\mathrm{cd7644d357db04cc63b48f9ccbfe5d2b18df720a128c41664a8c4f1951d3f201}\\
\end{split}
$$
Note how different each output is.
### B.
This is very powerful. The only option for finding the input based on the output is by *brute force*.
#### *==Note==*
In fact, it is theorically poss

---