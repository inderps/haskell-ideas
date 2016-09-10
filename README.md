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


## Enumeration types

```haskell

data Thing = Shoe 
           | Ship 
           | SealingWax 
           | Cabbage 

data FailableDouble = Failure
                    | OK Double
                    
ex01 = Failure
ex02 = OK 3.4

data Person = Person String Int Thing
        

```

### Credits

All the examples here are taken from [Brent Yorgey](https://byorgey.wordpress.com/)'s [course](http://www.seas.upenn.edu/~cis194/spring13/lectures.html)
