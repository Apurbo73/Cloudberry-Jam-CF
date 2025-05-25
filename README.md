# Cloudberry Jam CF:

### 🔍 Problem Explanation:

You're making jam using **cloudberries** and **sugar**. You need:

* **1 kg of berries** + **1 kg of sugar** to make jam.
* But **25%** of the total jam **evaporates** during cooking.

So, from `x` kg berries and `x` kg sugar, you get:

* Initial mix = `2x` kg
* Final jam = `0.75 × 2x = 1.5x` kg

Now, if you want to prepare `n` jars of **3 kg jam**, that’s `n × 3 = 3n` kg of jam.

Let’s reverse the calculation:

* Final jam = `1.5 × x` (where x is amount of berries)
  ⇒ `1.5x = 3n`
  ⇒ `x = 2n`

So, you need **2n kg of cloudberries** for `n` jars.

---

### ✅ Example:

If `n = 1`, you need `2` kg of berries
If `n = 3`, you need `6` kg of berries

---

### 💻 Code Breakdown:

```cpp
#include <bits/stdc++.h>  // Includes all standard libraries
using namespace std;

int main() {
    int n;           // Number of test cases
    cin >> n;        // Input t (number of test cases)

    while (n--) {    // Run the loop t times
        int a;       // Number of jars needed for current test case
        cin >> a;    
        cout << a * 2 << endl;  // Output 2 * a, the amount of berries needed
    }
}
```

---

### 🚀 Output Explanation:

For each test case, it simply prints `2 * n`, the kilograms of **berries** needed to make `n` jars of jam.

Let me know if you'd like a [visual diagram](f) of the process or [Python version](f) of the code.
