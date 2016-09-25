# PCalc Hybrid layout and some functions

![Screenshot](/screenshots/hybrid_layout.png)

## Hybrid layout

The Hybrid layout is a heavily changed *Programming* layout. It is designed to be used in RPN mode.

- numbers, operations, and other keys have bigger fonts
- removed some operations I didn't need
- renamed `bin`, `oct`, `dec` and `hex` to `2`, `8`, `10`, `16`
- added a key `logᵧx`
- added `+¹⁰` and `×¹⁰` (See *Sum 10 times* and *Multiply 10 times* functions) at the place of `+` and `×` in 2nd mode

#### Issues and TODO

- `logᵧx`: the *ᵧ* should be a *y*

## Functions

*Hybrid* package contains:
- *Binomial Coefficient (y, x)*
- *Logᵧx*
- *Multiply 10 times*: it's like pressing `×` 10 times, it multiplies the first 11 values of the RPN stack
- *Random [0-1]*
- *Random Integer [0-100]*
- *Random Integer [x-y]*
- *Ratio*: solves equations *x:a=b:c* and *a:x=b:c*. Put a *0* instead of *x*. For example: *S2=a*, *S1=0*, *y=b*, *x=c*, then you can execute it
- *Sum 10 times*: it's like pressing `+` 10 times, it sums the first 11 values of the RPN stack.

*Clipboard* package contains:
- *Add to Clipboard*
- *Copy to Clipboard*
- *Paste Clipboard*
- *Subtract from Clipboard*

See the implementation inside [screenshots/](https://github.com/diegobit/PCalc-Hybrid-Layout/tree/master/screenshots)

#### Issues and TODO
- *Ratio* doesn't solve equations *a:b=x:c* and *a:b=c:x*
- make *Sum 10 times* and *Multiply 10 times* work for any RPN stack depth (not possible with current PCalc instructions)

## Instructions
Just download and open the layout and the two function packages with PCalc.

The hybrid layout is designed to use the latest version of each function package available before the next layout version (example: `Hybrid 0.9.pcalclayout` uses `Hybrid 0.9.1.pcalcfunctions` and `Clipboard 0.8.pcalcfunctions`, while `Hybrid 0.8.pcalclayout` uses `Hybrid 0.8.pcalcfunctions` and `Clipboard 0.8.pcalcfunctions`).
Always use the latest version of each package unless you prefer an older layout. For example `Hybrid 0.8.pcalclayout` is the last one with the button `Ratio`.

#### Legacy versions
- Latest with RPN key: 0.10
- Latest with algebraic support: 0.10
- Latest with clipboard keys: 0.10
- Latest with Ratio key: 0.8

## Recommended settings
#### *(to make PCalc look like the screenshot)*
- RPN : ON
- Show Ticker Tape : OFF
- Theme > Samurai
- Digits > Thin
- Display > Vertical Number of Lines : 7
- Smart Resize : ON
- Accessibility > Use Dynamic Type : OFF
- Accessibility > Large Key Text : OFF
- Accessibility > Bold Key text : OFF
- Accessibility > Large Tape Text : OFF
- Advanced Settings > Hide Status Bar : OFF

## Changelog
**1.0:**
- layout: removed algebraic support (removed RPN toggle key)
- layout: removed clipboard keys (long tap display)
- layout: moved other keys
- functions: remove algebraic versions
- functions: added *Random [0-1]*

**0.10:**
- layout: changed some sizes and colours (Thanks to PCalc 3.6.1)
- layout: fixed round and trunc
- layout: added `roll up` key
- layout: renamed clipboard and memory keys to use PCalc default naming
- layout: added `×¹⁰` key
- functions: added *Multiply 10 Times*

**0.9.1:**
- functions: added *Binomial Coefficient (y, x)* function

**0.9:**
- layout: added `+¹⁰` key
- functions: added *Sum 10 times*

**0.8:**
- layout: removed *Ratio* key and rearranged the second and third row of the layout.
