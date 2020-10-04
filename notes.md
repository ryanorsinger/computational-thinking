## now we now

- functions have an implicit return
- raw"whateverstring" makes raw strings
- `?` starts Julia help and runs instantly inside of Pluto notebooks

## Pattern for solving area of Sierpinski triangle
```
   if n == 0
       # return (1 - 1/4)^0
       return 1
   elseif n == 1
       return (1 - 1/4)^1
   elseif n== 2
       return (1 - 1/4)^2
   elseif n == 3
       return (1-1/4)^4
   end
```

```
function area_sierpinski(n)
    return (1 - 1/4)^n
```


```
mean(x) = ones(length(x))'x / length(x)

function demean(x)
    μ = mean(x)
    
    # Perform elementwise subtraction with the .- operator
    return x .- μ
end
```
