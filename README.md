# Party Parrot Language

![Parrot](http://cultofthepartyparrot.com/parrots/hd/parrot.gif)

The future is parrot. 

## Installation

```bash
$ pip3 install git+git://github.com/TariqAHassan/PartyParrot@master
```

## General Usage

```python
from party_parrot import to_parrot, from_parrot
```

### To Parrot:

```python
parrot = to_parrot("hello world!", copy=True)
print(parrot)
# :triplets_parrot::witness_protection_parrot::confused_parrot::confused_parrot::conga_parrot: :deal_with_it_parrot::conga_parrot::popcorn_parrot::confused_parrot::chill_parrot:!
```

We can use `copy=True` to copy the output to our clipboard, so we can simply
paste the output elsewhere with `Command + V` on Mac or `Control + V` on Windows.

### From Parrot:

```python
print(from_parrot(parrot))
# hello world!
```

## Secret Parrot Messages

```python
parrot = to_parrot("hello world!", key=88)
print(parrot)
# :blonde_sassy_parrot::parrot_dad::bored_parrot::bored_parrot::goth_parrot: :coffee_parrot::goth_parrot::margarita_parrot::bored_parrot::ship_it_parrot:!
```

```python
# Wrong key:
print(from_parrot(parrot))  # default key = 1.
# xdzzv fvhzc!

# Correct Key:
print(from_parrot(parrot, key=88))
# hello world!
```
