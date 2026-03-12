[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18934949.svg)](https://doi.org/10.5281/zenodo.18934949)

k-adic Collatz Constellations
Prime-Preserving k-adic Collatz Chains on a Logarithmic Spiral
Hiroshi Harada — March 10, 2026

Overview
--------
This dataset contains prime-preserving k-adic Collatz-type sequences
(2-adic through 7-adic) and their corresponding logarithmic-spiral
visualizations. Each sequence consists entirely of prime numbers and
was verified using SymPy’s deterministic primality test.

In the logarithmic polar coordinate system, each integer n is mapped as:

    r = ln(n)
    θ = 2π ln(n)

If a recurrence multiplies n by approximately a, the angular displacement
satisfies:

    Δθ ≈ 2π ln(a)

When ln(a) lies close to a rational number p/q, the sequence rotates
nearly p full turns every q steps, producing self-similar expanding
geometric figures (“prime constellations”).

The general k-adic Collatz-type map used in this project is:

    F(n) = ((k + 1)n + b) / k

where b is chosen according to n mod k so that the numerator
(k + 1)n + b becomes divisible by k.

Included Prime Chains
---------------------
All chains consist entirely of prime numbers.

2-adic (Pentagram, L9)
    35014031359 → 52521047039 → 78781570559 → 118172355839 →
    177258533759 → 265887800639 → 398831700959 →
    598247551439 → 897371327159

3-adic (Heptagram, L8)
    46000363 → 61333817 → 81778423 → 109037897 →
    145383863 → 193845151 → 258460201 → 344613601

4-adic (Enneagram, L7)
    559188056938807297 → 698985071173509121 → 873731338966886401 →
    1092164173708608001 → 1365205217135760001 →
    1706506521419700001 → 2133133151774625001

5-adic (Hendecagram, L7)
    76933159 → 92319791 → 110783749 → 132940499 →
    159528599 → 191434319 → 229721183

6-adic (Tridecagram, L8)
    1099687 → 1282969 → 1496797 → 1746263 →
    2037307 → 2376859 → 2773003 → 3235171

7-adic (Pentadecagram, L9)
    68542687 → 78334499 → 89525141 → 102314447 →
    116930797 → 133635197 → 152725939 →
    174543931 → 199478779

Files Included
--------------
Prime_Chain_Collatz_Title.pdf
Prime_Chain_Collatz_Report_EN.pdf
Prime_Chain_Collatz_Report_JP.pdf
prime_chain_collatz_constellation.py
README.txt
LICENSE.txt 

How to Reproduce the Plots
--------------------------
1. Install Python 3.10+  
2. Install required libraries:
       pip install sympy matplotlib numpy
3. Run:
       prime_chain_collatz_constellation.py

License
-------
© 2026 Hiroshi Harada — MIT License.
This dataset, code, and documentation are released under the MIT License.
