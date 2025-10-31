# CP_Templates

A comprehensive collection of competitive programming templates designed for speed and efficiency in contests.

## 🚀 Quick Start

```bash
git clone https://github.com/mahmoudabozied4/CP_Templates.git
cd CP_Templates
```

## 📁 Template Categories

### 🔧 Data Structures
| Template | Time Complexity | Use Case |
|----------|-----------------|----------|
| **Fenwick Tree** | O(log n) | Prefix sums, point updates |
| **Segment Tree** | O(log n) | Range queries with lazy propagation |
| **Sparse Table** | O(1) query | Static range queries (RMQ, GCD) |
| **Ordered Set** | O(log n) | k-th element, order statistics |
| **Merge Sort Tree** | O(log²n) | Range order statistics |
| **Monotonic Stack/Queue** | O(n) | Sliding window extrema |

### 🧮 Algorithms
| Category | Templates Included |
|----------|-------------------|
| **Graph** | DFS, BFS, Dijkstra, Floyd-Warshall, MST |
| **Dynamic Programming** | Common patterns, optimization tricks |
| **Mathematical** | GCD, LCM, modular arithmetic, primes |
| **String** | KMP, Z-algorithm, hashing |

### ⚡ Utilities
- Fast I/O with buffer optimization
- Debug macros for development
- Coordinate compression
- Modular arithmetic operations
- Grid navigation utilities

## 🎯 Core Template Structure

```cpp
#include <bits/stdc++.h>
#include <ext/pb_ds/assoc_container.hpp>
using namespace std;
using namespace __gnu_pbds;
#define ll long long
#define int long long
typedef unsigned long long ull;
#define endl '\n'
typedef pair<int, int> pii;
#define elif else if
#define endd(s) return void(cout << s << "\n")
#define Ceil(n, m) (((n) / (m)) + ((n) % (m) ? 1 : 0))
#define X first
#define Y second
#define fixed(n) fixed << setprecision(n)
#define sz(s) int32_t(s.size())
#define dbg(x) cout << #x << ": " << (x) << "\n";
#define getline(s) getline(cin >> ws, s)
#define Time cerr << "Time Taken: " << (float)clock() / CLOCKS_PER_SEC << " Secs" << "\n";
#define all(vec) vec.begin(), vec.end()
#define rall(v) v.rbegin(),v.rend()
#define mul_mod(a, b) (((a % M) * (b % M)) % M)
#define add_mod(a, b) (((a % M) + (b % M)) % M)
#define sub_mod(a, b) (((a % M) - (b % M) + M) % M)
const int N = 1 >> 17, M = 1'000'000'007, OO = 0X3F3F3F3F3F3F3F3F;
const double EPS = 1e-9, pi = 3.141592653589793;
#define kill return 0
typedef vector<int> vi;
typedef vector<vi> vvi;
#define pb push_back
vector<string> RET = {"NO", "YES"};
#define IO(NAME) \
cin.tie(0)->sync_with_stdio(0); \
if(fopen(NAME ".in","r")) freopen(NAME ".in","r",stdin), \
freopen(NAME ".out","w",stdout);
template<class T>
using ordered_set = tree<T, null_type, less<T>, rb_tree_tag, tree_order_statistics_node_update>;

void Zied() {
    ios_base::sync_with_stdio(false), cin.tie(nullptr), cout.tie(nullptr);
#ifndef ONLINE_JUDGE
    freopen("input.txt", "r", stdin), freopen("output.txt", "w", stdout);
#endif
}

template<typename T = int>
istream &operator >>(istream &in, vector<T> &v) {
    for (auto &x: v) in >> x;
    return in;
}

template<typename T = int>
ostream &operator <<(ostream &out, const vector<T> &v) {
    for (const T &x: v) out << x << ' ';
    return out;
}

template<typename A, typename B>
istream &operator>>(istream &fin, pair<A, B> &p) {
    fin >> p.X >> p.Y;
    return fin;
}

template<typename A, typename B>
std::ostream &operator<<(std::ostream &fout, const std::pair<A, B> &p) {
    fout << p.first << " " << p.second;
    return fout;
}

enum dir { d, r, u, l, ul, dr, ur, dl };

int dx[8] = {1, 0, -1, 0, -1, 1, -1, 1};
int dy[8] = {0, 1, 0, -1, -1, 1, 1, -1};


void preprocessing() {

}

auto Solve(int &n) -> int {
    
}

bool solve_test(const int test_number) {
    int n = 1;
    // string n;
    if (!(cin >> n))
        return false;
    // Solve(n);
    auto ans = Solve(n);
    cout << ans << endl;
    return true;
}

void Stress() {
    // for (int n = 2; n <= 1; ++n)
    //     cerr << n << ' ' << Solve(n) << '\n';
}

int32_t main() {
    Zied();
    Stress();
    // freopen("document.in", "r", stdin);
    // freopen("document.out", "w", stdout);
    preprocessing();
    int test_cases = 1;
    // cin >> test_cases;
    for (int tc = 1; tc <= test_cases; tc++) {
        // cout << "Case " << tc << ": " << endl;
        if (!solve_test(tc))break;
        //                cout << endl;
    }
    kill;
    //    Time
}

/*
              ,   .-'"'=;_  ,
              |\.'-~`-.`-`;/|
              \.` '.'~-.` './
              (\`,__=-'__,'/)
           _.-'-.( d\_/b ).-'-._
         /'.-'   ' .---. '   '-.`\
       /'  .' (=    (_)    =) '.  `\
      /'  .',  `-.__.-.__.-'  ,'.  `\
     (     .'.   V       V  ; '.     )
     (    |::  `-,__.-.__,-'  ::|    )
     |   /|`:.               .:'|\   |
     |  / | `:.              :' |`\  |
     | |  (  :.             .:  )  | |
     | |   ( `:.            :' )   | |
     | |    \ :.           .: /    | |
     | |     \`:.         .:'/     | |
     ) (      `\`:.     .:'/'      ) (
     (  `)_     ) `:._.:' (     _(`  )
     \  ' _)  .'           `.  (_ `  /
      \  '_) /   .'"```"'.   \ (_`  /
       `'"`  \  (         )  /  `"'`
   ___   MZ   `.`.       .'.'        ___
 .`   ``"""'''--`_)     (_'--'''"""``   `.
(_(_(___...--'"'`         `'"'--...___)_)_)
*/

```

## 🛠️ Key Optimizations

### Performance Enhancements
- **Optimized I/O**: Custom operators for vectors and pairs
- **Efficient Memory**: Smart constant definitions
- **Fast Compilation**: Minimal includes for speed
- **Modular Design**: Easy to copy specific components

### Code Quality
- **Clear Structure**: Organized sections with headers
- **Consistent Naming**: Standardized variable conventions
- **Debug-Friendly**: Built-in debugging utilities
- **Contest-Ready**: Preprocessor directives for online judges

## 📊 Template Usage Guide

### Basic Problem Solving
```cpp
void solve() {
    int n;
    cin >> n;
    vi a(n);
    cin >> a;
    
    // Solution logic
    cout << result << endl;
}
```

### Multiple Test Cases
```cpp
int32_t main() {
    fast_io();
    
    int t;
    cin >> t;
    
    while (t--) {
        solve();
    }
    
    return 0;
}
```

### Interactive Problems
```cpp
void solve() {
    int n;
    cin >> n;
    
    // Interactive solution
    cout << "? " << query << endl;
    cout.flush();
    
    int response;
    cin >> response;
    
    cout << "! " << answer << endl;
    cout.flush();
}
```

## 🎯 Specialized Templates

### Graph Problems
```cpp
vector<vi> adj;
vector<bool> visited;

void dfs(int u) {
    visited[u] = true;
    for (int v : adj[u]) {
        if (!visited[v]) {
            dfs(v);
        }
    }
}
```

### Dynamic Programming
```cpp
vector<vi> dp;

int solve_dp(int i, int j) {
    if (base_case) return base_value;
    
    if (dp[i][j] != -1) return dp[i][j];
    
    // Recurrence relation
    return dp[i][j] = transition;
}
```

## 🏆 Contest Platforms Tested

- ✅ Codeforces
- ✅ AtCoder  
- ✅ CodeChef
- ✅ LeetCode
- ✅ HackerRank
- ✅ SPOJ

## 📚 Learning Resources

### Essential Reading
- [Competitive Programming 4](https://cpbook.net/) - Steven Halim
- [USACO Guide](https://usaco.guide/) - Comprehensive tutorials
- [CP-Algorithms](https://cp-algorithms.com/) - Algorithm implementations

### Practice Platforms
- [Codeforces](https://codeforces.com/) - Regular contests
- [AtCoder](https://atcoder.jp/) - High-quality problems
- [USACO](http://www.usaco.org/) - Olympiad preparation

## 🔧 Advanced Features

### Policy-Based Data Structures
```cpp
ordered_set<int> os;
os.insert(x);
os.order_of_key(x);  // 0-indexed position
*os.find_by_order(k); // k-th element
```

### Coordinate Compression
```cpp
vi vals = {original_values};
sort(all(vals));
vals.erase(unique(all(vals)), vals.end());

auto compress = [&](int x) {
    return lower_bound(all(vals), x) - vals.begin();
};
```

### Binary Search Template
```cpp
auto binary_search = [&](int l, int r) {
    while (l < r) {
        int mid = l + (r - l) / 2;
        if (check(mid)) r = mid;
        else l = mid + 1;
    }
    return l;
};
```

## 🚀 Performance Tips

1. **Use `int` as `long long`** for contest safety
2. **Minimize memory allocations** in tight loops
3. **Use references** to avoid unnecessary copies
4. **Prefer `'\n'` over `endl`** for faster output
5. **Use `reserve()`** for vectors with known sizes


## 📞 Contact & Contributions

Feel free to contribute improvements or report issues!

---

**Happy Competitive Programming!** 🏆
