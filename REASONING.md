# Reasoning for the Predictions Table

Write one entry under every heading below, then commit this file together with
`predictions.tsv`, before you run a case or open `tests/expected.tsv`.

Each entry names the rule that produces the four predicted fields for that
case. One to three sentences is enough. The grader checks structure only. It
does not judge quality, and it sets no word minimum.

After you run the cases, add a short correction under each case you predicted
wrongly. Say what you predicted, what CLISP printed, and which rule you
misread. Those entries belong in the correction commits.

## P01
The expression uses prefix notation where the innermost operation is evaluated first. The multiplication of 2 and 3 is performed before adding 1. The result is 7. It is an integer with no sequence length.

## P02
The quote returns its argument without evaluating its value. This makes it so that (+ 1 2) is not evaluated as 3 but returned as itself.

## P03
The quote operator prevents the expression from being evaluated and returns nil directly. NIL represents an empty list, so its kind is classified as null and its length is 0.

## P04
T is a symbol that just evaluates to itself. It’s a symbol and not a list so the length is 0.

## P05
The symbolp function checks whether the given argument is a symbol. Since the argument is an empty list, the expression returns nil. The result has kind null and no sequence length.

## P06
The car operator returns the first symbol of a list. In this case, it was given an empty list, thus returning nil as a list of length 0.

## P07
The cons function places the first argument at the beginning of the given list. The resulting list is (1,2,3) which contains three elements. Its kind is cons and its length is 3.

## P08
The if statement asks if null is the same as an empty list, and it evaluates as true. The empty is the one that gets returned as the first symbol is what gets evaluated if the statement is true.

## P09
The and operator evaluates its arguments from left to right and stops when it encounters a false value. Since the second argument is nil, the result is nil. The result has kind null and length 0. The operator is classified as a function because it performs a logical operation.

## P10
The progn special form runs all its subforms and returns the value of the last one. defvar makes *ps3-rate* a variable with value 2, it’s able to be called with ps3-scale. let changes the value to 10 and ps3-scale sees the value of *ps3-rate* as 10, so it evaluates 3*10, and 30 is returned.

## P11
The defun expression defines a function named ps3-twice. The function accepts one parameter and multiplies that parameter by 2. The resulting value is the function name, which is a symbol and has no sequence length.

## P12
The labels special form defines functions that can call themselves. down returns ‘() when n is 0, and otherwise puts n in front of (down (- n 1)). So (down 3) builds (cons 3 (cons 2 (cons 1 '()))), which is (3 2 1), a list of length 3.

## P13
The mapcar function applies the length function to every sublist. The first sublist contains two elements, the second is empty and the third contains one element. The resulting list is (2,0,1), with three elements.

## P14
The function mapcar applies the squaring lambda to each element of (1 2 3) and collects the results into a new list, (1 4 9). The output has as many elements as the input, so the length is 3.

## P15
The lambda expression creates an anonymous function that accepts one parameter and multiplies it by 2. The result is a function object with kind function and no sequence length.

## P16
At the start, factor was given a value of 2 using let. The (let ((f (lambda (n) (* n factor)))) is under this lexical scope which makes it so that it can access factor = 2. The second value of factor is 10, but it can't be seen by f, so the result ends up as 3*2=6.