# 🪙 Interchained (ITC) CPU Mining Guide

## 🌐 Overview
This quick guide explains how to mine **Interchained (ITC)** using **cpuminer** on the official pool:  
👉 [mining.interchained](https://mining.interchained.org)

Please make sure to replace all example wallet addresses with **your own ITC address** (`itc1...`).

---

## ⚙️ Configuration

| Parameter | Value / Example |
|------------|-----------------|
| **Username** | Your Interchained wallet address (`itc1...`) |
| **Password** | Anything (e.g., `x`) |
| **Algorithm** | `interchained` |
| **Pool URL (diff 1)** | `stratum+tcp://hash.interchained.org:4888` |

---

## 💻 Example Command

```
./cpuminer-avx -a interchained -o stratum+tcp://hash.interchained.org:4888 -u itc1q7j7edc5wh0qyllhlzhv2sqmxwssfzan9pc53rc.Ecrypt -p x -t 24
```


## 🧩 Parameters:

-a → algorithm name (interchained)

-o → mining pool URL

-u → your wallet address + optional worker name (.Ecrypt)

-p → password (any string)

-t → number of CPU threads (tune for your CPU cores)


> 💡 Tip: Experiment with -t value to find the optimal performance for your CPU.

---

## 📦 Download cpuminer

Use the RPlant fork of cpuminer-opt, which supports the Interchained algorithm.

🔗 Releases:
https://github.com/rplant8/cpuminer-opt-rplant/releases/


---

## 🧠 Notes

Make sure your CPU supports AVX / AVX2 / AES for best performance.

Mining rewards are automatically sent to your ITC wallet.

You can monitor your hashrate and earnings on the pool dashboard.

