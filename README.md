# LispTode
translates a lisp dialect into color code (v7)

```
// Atom
hello
>> hello

// List
(hello world)
>> (hello world)

// Variable
(define greeting (hello world))
>> (define greeting (hello world))

// Resolve
greeting 
>> (hello world)

// Quote
'greeting
>> greeting

// Lambda
(lambda (name) '(hello name))
>> (lambda (name) (hello name))

// Call
((lambda (name) '(hello name)) luke)
>> hello luke

// Function
(define greet (lambda (name) '(hello name)))
>> (define greet (lambda (name) (hello name)))

(greet luke)
>> hello luke

// JavaScript
({{ (name) => "(goodbye " + name + ")"}} luke)
>> (goodbye luke)

(define shout {{ (word) => word + "!"}})
>> (define shout {{ (word) => word + "!"}})

(shout hello)
>> hello!
```
