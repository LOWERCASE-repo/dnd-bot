https://discord.com/api/oauth2/authorize?client_id=551378788286464000&scope=bot

# guide
- roll syntax is `roll <dice> <modifier> <repeats>`
- `<dice>` is the number and size of the dice to roll, e.g. `2d6`, `1d20`
- `<modifier>` is what to add at the end of the roll, e.g. `+5`, `-5`
- `<repeats>` is how many times to repeat the roll, e.g. `x2` for advantage, or `x3` for rolling three attacks at once

# examples
- `roll 1d20 +6` or `roll 6` rolls a skill check with a +6 modifier
- `roll 2d6 +5 x3` or `2d6 5 x3` rolls greatsword damage with a +5 modifier three times
- `roll 1d20 1d4 -3 x2` or `d20 d4 -3 x` rolls a stealth check with a -3 modifier, guidance, and disadvantage

# advanced
- plus signs can be omitted
	- e.g. `roll 1d20 +6 x2` is the same as `roll 1d20 6 x2`
- if `<dice>` doesn't specify a count, it defaults to `1`
	- e.g. `roll 1d20 6 x2` is the same as `roll d20 6 x2`
- if `<dice>` is omitted entirely, it defaults to `1d20`
	- e.g. `roll d20 6 x2` is the same as `roll 6 x2`
- `roll` can be omitted entirely if at least two parameters are provided
	- e.g. `roll 6 x2` is the same as `6 x2`
- if `<repeats>` doesn't specify a count, it defaults to `2`
	- e.g. `6 x2` is the same as `6 x`
