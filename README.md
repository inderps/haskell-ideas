# haskell-ideas
Basic ideas which can be taken from Haskell to implement in other languages


## Type Signatures

```haskell

x :: Int
x = 3

f :: Int -> Int -> Int -> Int
f x y z = x + y + z

```


## Guards

```haskell

hailstone :: Integer -> Integer
hailstone n
  | n `mod` 2 == 0 = n `div` 2
  | otherwise      = 3*n + 1

isEven :: Integer -> Bool
isEven n 
  | n `mod` 2 == 0 = True
  | otherwise      = False

```
