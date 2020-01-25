#lang sicp

(define (abs x)
  (if (> x 0) x
      (- x)))

(define (avg-of-2 x y)(/ (+ x y) 2))

(define (square x)(* x x))

(define (good-enough? guess x)
  (< (abs (- (square guess) x)) 0.001))

(define (improve-guess guess x)(avg-of-2 guess (/ x guess)))

(define (try guess x)
  (if (good-enough? guess x) guess
      (try (improve-guess guess x) x)))

(define (sqrt x)(try 1 x))
