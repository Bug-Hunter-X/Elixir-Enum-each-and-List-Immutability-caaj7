# Elixir List Immutability in Enum.each

This example demonstrates a common mistake in Elixir when working with lists and the `Enum.each` function.  Because Elixir lists are immutable, attempting to modify a list directly within an `Enum.each` loop will not affect the original list.

The `bug.exs` file shows the problematic code, and `bugSolution.exs` provides a corrected version using `Enum.filter` to create a new list.

## How to Reproduce

1.  Save the code in `bug.exs`.
2.  Run it from your Elixir shell: `elixir bug.exs`
3.  Observe that the list is not modified as expected.

## Solution

The solution involves using functional techniques like `Enum.filter` to create a new list containing only the desired elements.