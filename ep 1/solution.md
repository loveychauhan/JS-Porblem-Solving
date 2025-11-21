 ## print number between 1 and N

```
const form = document.querySelector('form')
const inputnumber = document.querySelector('#number')
const showNumber = document.querySelector('.showNumbers')

let number;
inputnumber.addEventListener('input', (e) => {
number = e.target.value
})

form.addEventListener('submit', (e) => {
e.preventDefault()
showNumber.innerText = ''
if (number) {
for (let i = 1; i <= number; i++) {
showNumber.append(i, ',')
}
} else {
showNumber.append('enter a number')
}

})
```


## Print number from N to 1 without changing the loop condition

```
const num = prompt("Enter A Number:-")

for (let i = 1; i <= num; i++) {
console.log(num - i + 1)
}

// Print all even number from 1 to N
{
const num = 20;

    //1,2,3,4,5,6,7,8,9,10
    for (let i = 1; i <= num; i++) {
        if (i % 2 === 0) console.log(i)
    }

}

```


## Print sum of all natural number
```
const num = 5;
let sum = 0
for (let i = 1; i <= num; i++) {
sum = sum + i
}

    console.log(sum)

}

const n = 5;

console.log(n \* (n + 1) / 2)
```
## Factorial of n

```
const form = document.querySelector('form')
const inputnumber = document.querySelector('#number')
const showNumber = document.querySelector('.showNumbers')

    let number;
    inputnumber.addEventListener('input', (e) => {
        number = e.target.value
    })

    form.addEventListener('submit', (e) => {
        let factorial = 1
        e.preventDefault()
        showNumber.innerText = ''

        if (number > 20) {
            return showNumber.append(`Enter a smaller number `)
        }
        if (number) {
            for (let i = 1; i <= number; i++) {
                factorial *= i
            }
        } else if (number === 0) {
            factorial = 0
        }
        else {
            showNumber.append('enter a number')
        }
        showNumber.append(`Factorail => ${factorial}  `)
    })

```

## Sum of all even number

```
let evensum = n / 2 \* (n / 2 + 1)

    console.log(evensum)

```

## sum of all number divide by 3 and 5
```
const n = 30 // 20 + 18 + 16 + 14 + 12 + 10 + 8 + 6 + 4 + 2

    for (let i = 1; i <= n; i++) {
        if (i % 3 == 0 && i % 5 == 0) {
            console.log(i)
        }
    }

```

## sum of odd number upto n

```
const num = 10

    const terms = num % 2 === 0 ? num / 2 : (num + 1) / 2
    const sum = terms ** 2

    console.log(sum)

```

## print cube of first n number

```
const num = 5

    for (let i = 1; i <= num; i++) {
        console.log(Math.pow(i, 3))
    }

```

## print number that are prefect square and even
```
const num = 100
let i = 2
let square = 4;

while (i ** 2 <= num) {
square = i ** 2
if (square % 2 === 0) {
console.log(square)
}
i++;

}
```