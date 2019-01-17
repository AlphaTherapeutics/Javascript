# Javascript

## Iterators

data as flows

any format of data can be a flow of data == iterables

```
const numbers = [4,5,6]
for (let i = 0; i < numbers.length; i++){
  console.log(numbers[0]
}
```

```
/* function */
function createNewFunction(){
  function add2 (num){
    return num+2;
  }
  return add2;
};

const newFunction = createNewFunction();

const result = newFunction(3);
```

```
/* function 2 */
function createFunction(array){
  let i = 0
  function inner(){
    const element = array[i];
    i++;
    return element;
  }
  return inner
}

const returnNextElement = createFunction([4,5,6])
const element1 = returnNextElement() // returns 4 very important to understand this line
const element2 = returnNextElement() // returns 5
```

## Vocabulary
Global Memory/ Global Execution Context
Local Execution Context
Call Stack
uninitialized
backpack of data called in dev community is called == [
  1. Closed Over Variable Environment (C.O.V.E), 
  2. Persistent Lexically Scoped Referenced Data (P.L.S.R.D),
  3. Closure
  ]
  its attached to hidden thing called [[scope]]
functions are 3 parts
  1. code
  2. permanant memory
  
  "abstraction" - hiding
  
  when we abstract in programming, we make it easier by hiding code to make it easier to understand
