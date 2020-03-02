---
title: "Baics of DOM"
description: "Learn about dom"
date: "2020-03-2"
categories: ['js', 'dom']
published: false
---

Well, I write this article because lately I was dealing with source code in js that had an excessive amount of if statement,
at levels that I had never seen. That is why I think it is very important to share these simple techniques that will help us to write code without having to think about the "if" when deciding.

I am going to explain 6 ways on how to do this. The idea of ​​this is not to enter into paranoia of never using IF, it is to open the head to new ways of thinking about our decisions in JS.

## Categories:

- [Ternary operator](https://hello.com)

### 1) Ternary operator:
We are talking about this "condition ? expr1 : expr2", very easy.

Example 1:
Code with IF:

```js
function saveCustomer(customer) {
  if (isCustomerValid(customer)) {
    database.save(customer)
  } else {
    alert('customer is invalid')
  }
}
```