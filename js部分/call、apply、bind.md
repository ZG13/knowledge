### call
function.call(context, aaa, bbb)
改变指定函数中的 this 指向

```
const obj = {
  name: 'Apple',
  greeting: function() {
    console.log('Hi! This is', this.name);
  }
}

const obj1 = {
  name: 'Banana',
}

obj.greeting(); // Hi! This is, Apple
obj.greeting.call(obj1); // Hi! This is, Banana

```

### apply
function.apply(context, [aaa, bbb])
改变指定函数中的 this 指向

除参数外使用方法与call一致


### bind
function.bind(thisArg, arg1, arg2, ...)

```
const obj = {
  name: 'Alice',
  greeting: function(city, country) {
    console.log(`Hello, my name is ${this.name} and I am from ${city}, ${country}`);
  }
};

const person = {
  name: 'Bob'
};

const boundGreeting = obj.greeting.bind(person, 'London');

boundGreeting('UK'); // 输出 "Hello, my name is Bob and I am from London, UK"

```
