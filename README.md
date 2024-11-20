# Back-Of-The-Envelope Estimation

## Keywornd
- **DAU:** Daily Active User.
- **UDAU:** Usage per DAU.
- **MDAU:** Memory per DAU.
- **RQPS:** Read Query Per Second.
- **WQPS:** Write Query Per Second.
- **RPS:** Request Per Second.

## Load

$$
QPS (per second) = \frac{DAU \cdot UDAU}{10^5}
$$

- $${10^5}$$: second perday ($$\approx 86400$$ seconds).

_**Example:**_
I have Digital Wallet application which have 100 milion active user per day. Each user create 10 transactions/day. Then QPS will be:

$$
QPS (per second) = \frac{10^8 \cdot 10}{10^5} = 10^4/second 
$$

## Storage

$$
Storage Estimation (per day) = DAU \cdot UDAU \cdot MDAU
$$

- $${10^5}$$: second perday ($$\approx 86400$$ seconds).

_**Example:**_

I have a **Digital Wallet application** with **100 million active users per day**.  
Each user creates **10 transactions per day**.  
For each transaction, we generate a **PDF invoice of approximately 2 MB**.

$$
\text{Storage Estimation (per day)} = 10^8 \cdot 10 \cdot 2 \, \text{MB} = 2 \cdot 10^9 \, \text{MB}
$$

Converting to GB:

$$
2 \cdot 10^9 \, \text{MB} = 2 \cdot 10^6 \, \text{GB} = 2 \, \text{PB (Petabytes)}
$$
