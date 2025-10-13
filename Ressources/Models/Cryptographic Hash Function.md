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
\mathrm{Ver}(\mathrm{Message,Signature,PublicKey})=\begin{cases}1\,\,\mathrm{if}
$$
# Example

---