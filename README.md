# ΣpinZero

**ΣpinZero** is a web app for balancing centrifuge rotors using number theory and complex roots of unity.

Enter the number of slots and tubes, choose a mode, and the app visualizes whether your configuration is balanced (Σspin = 0) — or dangerously chaotic.


---

### How it works

For **rotors with up to 24 slots**, ΣpinZero **brute-forces all possible configurations** to find truly balanced ones. This might take a few seconds — especially for larger values of `n` and `k`.

For **n > 24**, the app automatically disables computationally intensive modes (Elegant, Cursed, Random) and only allows efficient algorithms to avoid computational explosion.
---
#### Balancing Modes

- **Cycle Decomposition**
  - **The smartest and mathematically coolest approach**
  - Uses prime factorization of `n` to create cycles that mathematically guarantee balance
  - Each cycle corresponds to a root of unity that sums to zero
  - Efficient for large rotors where brute force is impossible
  - Shows the underlying mathematical beauty of the problem
  - Unlike brute-force methods, won't tell you how many possible solutions exist
  - *Available for all n values*

- **Elegant**
  - Finds the most symmetrical and well-spaced balanced configuration
  - Optimizes for maximum symmetry and largest minimum distance between tubes
  - Perfect for _AESTHETICS_
  - *Automatically disabled for n > 24 (too computationally intensive)*

- **Cursed**
  - Locates balanced configurations with the maximum variety of spacing between tubes
  - Creates chaotic yet mathematically perfect balance
  - For when you want to balance on the edge of chaos
  - *Automatically disabled for n > 24 (too computationally intensive)*

- **Evil** ☠️
  - Finds the most deceptive arrangement possible
  - Delivers the smallest possible non-zero imbalance
  - Creates a configuration that looks balanced but will still wreck your centrifuge
  - Classic chotic evil alignment
  
- **Random**
  - Selects a random balanced arrangement from all possibilities
  - Perfect when you just need any valid solution
  - *Automatically disabled for n > 24 (too computationally intensive)*

- **Heuristic Random**
  - Employs a smart random search with timeout protection
  - Runs multiple parallel search attempts to find solutions quickly
  - Perfect balance for reasonable computation time
  - Falls back to cycle decomposition when possible
  - *Available for all n values*

- **Manual Mode**
  - Place tubes yourself and see if your arrangement is balanced in real-time
  - Full vector visualization shows exactly how balanced (or unbalanced) your configuration is
  - Great for educational purposes and hands-on experimentation
  - *Available for all n values*

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
