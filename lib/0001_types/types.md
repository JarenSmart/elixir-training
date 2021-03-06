# Types in Elixir

Elixir has several types.

The types are as follows:

1. atom - an atom starts with a : and comes from Erlang, the language that Elixir was built on top of. It is a constant whose name is its own value. Can also be called a symbol.
  * `:hello`
  * `:ok`
  * `:example`

2. string - a string is wrapped in quotes. They can be either one line or multiline.
  * `"hello"`
  *
  ```
  """
  This is
  a multiline
  string.
  """
  ```

3. integer - an integer is any number that has no decimal.
  * `0`
  * `1234567`
  * `-50283`

4. float - a float is any number that has a decimal.
  * `1.0`
  * `1234567.12345`
  * `-50283.912`

5. boolean - a boolean is either `true` or `false`.
  * `true`
  * `false`

6. Tuple - a tuple is a grouping of other types and is wrapped in `{` and `}`.
  * `{:ok, true}`
  * `{1, "two", :three, 4.0}`

7. List - a list can contain any other kind of type (they don't have to be the same type) and is wrapped in `[` and `]`.
  * `[1, 2, 3]`
  * `[:hello, 2.0, false]`
  * `[{:ok, 1}, 5]`

8. Map - a map takes two types as a key value pair. The key must be either a string or atom. This means that a map can be created a couple different ways. It is wrapped in `%{` and `}`
  * `%{test: 1}` - most common
  * `%{:test => 1}`
  * `%{"key with spaces": true}`
  * `%{"key with spaces" => [1, 2, 3]}`

9. Struct - a struct is a map that has defined parameters. They are typically defined in a module using `defstruct`. They give you the ability to know what keys to expect in a map. A struct is defined as `%<STRUCT_NAME>{` and `}`
  * `%User{first_name: "Billie", last_name: "Jean", gender: :female, my_lover: false}` is a User struct
  * `%Book{title: "Great Expectations", author: "Charles Dickens", pages: 544}` is a Book struct
