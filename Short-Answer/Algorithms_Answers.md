#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  O(n) even if the while loop runs as long as `a` is less then n^3, because inside the loop the `a` variable gets increased by the num squared >> O(n^2) therefore bringing the all iteration process back to just O(n) following a linear pattern, which increases at the same rate as the n input does.

b) O(log n) even thou there are two nested loops which would normally make it a O(n^2) the nested while loop will double at each iteration, which will basically run less and less times the larger the `n` is, therefore following a logarithmic curve

c) O(1) as there is no invokation for the actual function which means that it will never run therefore the time complexity will be a constant no matter what the size of the input, but in the case that there was an invocation of the function, it will result in O(n) value, as it will continue to iterate recursively depending on the size of the input (in this case bunnies), forming a linear curve

## Exercise II

# start from middle of the building 
    base = 0
    mid = n // 2
    top = n
    broken_egg = true
# iterate over length of `n` while egg keeps breaking
    # throw egg, if egg breaks, make `n` = mid
    # else cut bottom half by making base = mid
    # repeat process for next iteration till egg stops breaking

I assume that this process that follow a typical binary search pattern is the best solution in this case as at each iteration the number of floors will be halved till the egg breaks no more, therefore following a O(log n) time complexity even in the worst case scenario