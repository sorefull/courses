# Переменные руби. Операторы Ruby. Комментарии. Условные операторы

## Переменные

```ruby
  age = 22            # Integer (Fixnum | Bignum)
  temperature = 36.6  # Float
  name = 'Oleg'       # String
  language = "Ruby"   # String too, difference later
  smokes = true       # Boolean
```
## Операторы
### Арифметические операторы:

```ruby
  age = age + 2       # age => 24
  age = age * 2       # age => 48
  age = age / 2       # age => 24
  age = age ** 2      # age => 576
  age = age % 2       # age => 0
```

### Операторы сравнения:

```ruby
  a = 1 > 3           # a => false
  b = 0 < 4           # b => true
  c = 1 == 3          # c => false
  d = 2 != 1          # d => true
```

### Операторы присвоения:

```ruby
  a = 10              # a => 10
  a += 5              # a => 15
  a -= 10             # a => 5
  a *= 4              # a => 20
  a /= 5              # a => 4
  a **= 2             # a => 16
  a %= 5              # a => 1
```

### Паралельное присвоение:

```ruby
  a, b, c = 10, 15, 25  # a => 10, b => 15, c => 25
```

### Логические операторы:

```ruby
  a = 5 > 10 && true    # a => false
  b = 2 < 0 || 5 != 4   # b => true
  c = !(a || b)         # c => false
```
 [There](https://stackoverflow.com/questions/1426826/difference-between-and-and-in-ruby) are more operators: `and`, `or`, `not`. They look prettier, but they'r priority is low, so use `&&` and `||` to be sure that your code do what you expect.

## Комментарии

От многострочных комментариев вскоре планируют отказаться так что советую пользоваться однострочным вариантом.

```ruby
  # Single-line comment

  =begin
    Multy-lined comment
  =end
  # Don't know why github's markdown can't see them
```

## Условные операторы

```ruby
  if age < 21
    # not allowed to buy drinks
  else
    # Cheers!
  end

  if time > 22
    # go sleep
  end

  unless condition
    # do something
  end

  result = if password == '1234'
    'secret data'
  else
    'wrong password!'
  end

  result = password == '1234' ? 'secret data' : 'wrong password!'
```
