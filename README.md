# ΣpinZero

**ΣpinZero** is a web app for balancing centrifuge rotors using number theory and complex roots of unity.

Enter the number of slots and tubes, choose a mode (elegant, cursed, random, or manual), and the app visualizes whether your configuration is balanced (Σspin = 0) — or dangerously chaotic.


---

### How it works

For **rotors with up to 30 slots**, ΣpinZero **brute-forces all possible configurations** to find truly balanced ones. This might take a few seconds — especially for larger values of `n` and `k`.

For **n > 30**, the app switches to **manual mode**: you place the tubes yourself, and it calculates whether your arrangement is balanced based on the sum of unit vectors.

---

**Try it here:**  
[https://yamir-1138.github.io/SpinZero/](https://yamir-1138.github.io/SpinZero/)

---

### Credits & Math

Based on beautiful mathematical insights by:

- [Gary Sivek – *Vanishing Sums of Roots of Unity*](https://www.kurims.kyoto-u.ac.jp/EMIS/journals/INTEGERS/papers/k31/k31.pdf)  
- [Matt Baker – *The Balanced Centrifuge Problem*](https://mattbaker.blog/2018/06/25/the-balanced-centrifuge-problem/)

---

**Disclaimer:**  
The math is correct. The code might not be.  
Use at your own risk :)
