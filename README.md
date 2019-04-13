# The Ternary Expression and Logic

## Learning Goals

* Identify the Ternary Expression

## Introduction

As conversationalists with computers, we've come so far so fast!

We now want to learn how to write an expression that expresses "conditional
thinking" or "if-then" logic.

We're about to learn **the ternary expression** which is an expression that can
provide one of two values, based on the truth (or "Boolean value" of a third
value)

>**NOTE** "Ternary" is Latin for "3 per." The previous paragraph shows three
>values being involved in the statement. Let's get to know our friend the
>ternary statement.

## Identify the Ternary Expression

The ternary statement is an _expression_ just like all the other expressions
we've already met. It looks like this:

```Python
# Position 1                 # Position 2                    # Position 3
"thing_to_return_if_true" if boolean_conditional_value else "thing_to_return_if_false"
```

If ` boolean_conditional_value` is a `True` value, then the return value of the
expression is "thing_to_return_if_true". If it is `False`,
"thing_to_return_if_false" is returned.

Here's an example to try out:

```Python
likely_to_rain = True
garment = "galoshes" if likely_to_rain else "sun hat"
```

As you see the return value of the ternary expression is assigned to `garment`.
You can use the _variable lookup expression_ to verify that the value of
`garment` is `"galoshes"`.

Try changing the variable with the _assignment expression_ from `True` to
`False`. Then run the ternary expression again. The value of `garment` should
become `sun hat`.

Amazingly, in expression we now have the ability to understand conditional
logic.

### Moving Beyond Boolean

Keep in mind that the second term in a ternary statement can also be an
expression. It does not have to be `True` or `False` (_constant expressions_)
it can be _calculated_ truth; truth calculated by an _expression_.

Recall arithmetic, recall this statement: `2 > 1` is `2` "greater than" 1? Try
putting this _expression_ into the Python interpreter: does the Python
interpreter confirm that it `evaluates` to `True`?

Try updating your original the Python interpreter code

```Python
garment = "galoshes" if 2 > 1 else "sun hat"
```

This logic makes `garment` `"galoshes"` again. Try swapping `>` for `<`, is
that what you expected?

You've now met two _comparison operators_. Comparison operators return `True`
or `False`. We'll meet the whole family of them in the next lesson. You can
always swap a "literal constant value" for "an expression that returns a value"
in programming. Thus since comparison operations return `True` or `False`, we
can use one of those expressions in Position 2 of our ternary statement.

Even more amazing, we can swap out the simple `String`s we've used in
Positions 1 and 3 of our ternary with expressions as well.

```Python
top = 2
bottom = 1
problem_count = 99
lucky_number = ( 3 + 1 ) if (top > bottom) else ( problem_count / 3 )
```

What's the value of `lucky_number`? Step through the expressions to make you
understand what happens step by step.

> **STYLE TIP**: To keep reading the expressions in the ternary statement's
> positions clear, we wrap them in `()`. It's done for readability and to
> prevent accidental order of operations bugs.

## What Provides Truth?

Obviously, given the ternary's power to express conditionals, it's really
helpful to know which operators express `True` and `False`. In our next lesson
we'll give a list of Boolean operators.

## Conclusion

It's an amazing moment when a child moves from mere _variable lookup_ and
_variable assignment_ to start surfacing the ability to reason between
hypothetical if-then outcomes. **IF** I touch the stove, I will get hurt;
**ELSE** I shall stay unhurt. **IF** I sass grandma, I will get a time-out;
**ELSE** I can eat ice cream. We've now gained the ability to express
conditional logic to Python!

## Resources
