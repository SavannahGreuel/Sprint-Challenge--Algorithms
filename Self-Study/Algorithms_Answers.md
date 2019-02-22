## Excercise I

```
a) 

a= 0 : constant time or O(1)
a < n * n * n : O(n^2)
a = a + n * n :  is O(n)

So problem a would be O(n^2) because it is the largest (or slowest) of the three
```

```
b)
 sum = 0 :                               O(1)

    for i in range(n):                   `O(n)`
      i += 1                             O(1)
      for j in range(i + 1, n):          `O(n)`
        j += 1                           O(1)
        for k in range(j + 1, n):        `O(n)`
          k += 1                         O(1)
          for l in range(k + 1, 10 + k): `O(n)`
            l += 1                       O(1)
            sum += 1                     O(1)

The outer loop runs n number of times, and every time the outer loop executes, the inne loop runs x number of times, and so on. There are 3 nested for loops in This problem, so it would be would be O(n^3)
```

```
c)  def bunnieEars(bunnies):
      if bunnies == 0: O(1)
        return 0:      O(1)

      return 2 + bunnyEars(bunnies-1): O(n)

bunnies decrements by one each time the runction recurses, giving it a O(n) value 
```

## Excercise II

1) find the midpoint of the number of stories
2) if the egg breaks at the midpoint, make a list of all the stories under the midpoint
3) if the egg doesnt break, make a list of all the stories above the midpoint
4) repeat above steps until you find the value of _f_.

conclusion: this algorithm would be very similar to how binary search would work, making this a O(log n)
