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
Replace this line with the rule behind this case's four fields.

## P03
The quote operator prevents the expression from being evaluated and returns nil directly. NIL represents an empty list, so its kind is classified as null and its length is 0.

## P04
Replace this line with the rule behind this case's four fields.

## P05
The symbolp function checks whether the given argument is a symbol. Since the argument is an empty list, the expression returns nil. The result has kind null and no sequence length.

## P06
Replace this line with the rule behind this case's four fields.

## P07
The cons function places the first argument at the beginning of the given list. The resulting list is (1,2,3) which contains three elements. Its kind is cons and its length is 3.

## P08
Replace this line with the rule behind this case's four fields.

## P09
The and operator evaluates its arguments from left to right and stops when it encounters a false value. Since the second argument is nil, the result is nil. The result has kind null and length 0. The operator is classified as a function because it performs a logical operation.

## P10
Replace this line with the rule behind this case's four fields.

## P11
The defun expression defines a function named ps3-twice. The function accepts one parameter and multiplies that parameter by 2. The resulting value is the function name, which is a symbol and has no sequence length.

## P12
Replace this line with the rule behind this case's four fields.

## P13
The mapcar function applies the length function to every sublist. The first sublist contains two elements, the second is empty and the third contains one element. The resulting list is (2,0,1), with three elements.

## P14
Replace this line with the rule behind this case's four fields.

## P15
The lambda expression creates an anonymous function that accepts one parameter and multiplies it by 2. The result is a function object with kind function and no sequence length.

## P16
Replace this line with the rule behind this case's four fields.
