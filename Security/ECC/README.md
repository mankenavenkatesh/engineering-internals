For a given elliptic curve, we take a `G generator`
and apply the cycle group operation `k(privatekey)` number of times to generate `p(publickey)`
and idea here is - It's very difficult to compute `k`

Question is
when any user generates his keyPairs `(k, p)`, will he also also executes cyclic group `k` number of times? if so, why can't attacker do the same?

Turns out, that the public key is not calculated by adding G to itself k (private key) times. It is calculated by first changing the k to binary form and multiplying the public key variable by 2 (adding to itself) for each bit while adding G if the current bit has value of one.
https://en.wikipedia.org/wiki/Elliptic_curve_point_multiplication
