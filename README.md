# PCalc Hybrid layout and some functions

![Screenshot](/screenshots/hybrid_layout.png)

## Hybrid layout

The Hybrid layout is based on a heavily changed built-in *Programming* layout. It is designed with RPN in mind but it also supports the Algebraic mode.

- numbers, operations, `2nd` and `RPN` have bigger fonts
- removed some operations I didn't need
- renamed `bin`, `oct`, `dec` and `hex` to `2`, `8`, `10`, `16`
- added keys to manage the clipboard with the same behaviour as the memory
- added a key `logᵧx`
- added `+¹⁰` and `×¹⁰` (See *Sum 10 times* and *Multiply 10 times* functions) at the place of `+` and `×` in 2nd mode

#### Issues

- some keys are duplicated, one visible only in RPN mode and the other in Algebraic mode due to some limitations in the layout editor (I could edit the layout manually, but...):
  - `clip str` (RPN 1st, Alg 1st) / `clip +` (RPN 2nd, Alg 2nd)
  - `clip rec` (RPN 1st, Alg 1st) / `clip -` (RPN 2nd, Alg 2nd)
  - `logᵧx`: RPN and Algebraic use different functions
- `logᵧx`: the *ᵧ* should be a *y*
- bad parenthesis and `÷` placement in Algebraic mode

## Functions

*Clipboard* package contains:
- *Add to Clipboard*
- *Copy to Clipboard*
- *Paste Clipboard alg*
- *Paste Clipboard rpn*
- *Subtract from Clipboard*

*Hybrid* package contains:
- *Binomial Coefficient (y, x)*. Available only in RPN mode
- *Logᵧx alg*
- *Logᵧx rpn*
- *Multiply 10 times*: it's like pressing `×` 10 times, it multiplies the first 11 values of the RPN stack. Available only in RPN mode.
- *Random [0-100]*
- *Random [x-y] alg*
- *Random [x-y] rpn*
- *Ratio*: solves equations *x:a=b:c* and *a:x=b:c*. Put a *0* instead of *x*. For example: *S2=a*, *S1=0*, *y=b*, *x=c*, then you can execute it. Available only in RPN mode
- *Sum 10 times*: it's like pressing `+` 10 times, it sums the first 11 values of the RPN stack. Available only in RPN mode.

#### Issues and TODO
- *Ratio* doesn't solve equations *a:b=x:c* and *a:b=c:x*
- *Ratio* for Algebraic mode
- make *Sum 10 times* and *Multiply 10 times* work for any RPN stack depth (not possible with current PCalc instructions)

## Instructions
Just download and open the layout and the two function packages with PCalc.

The hybrid layout is designed to use the latest version of each function package available before the next layout version (example: `Hybrid 0.9.pcalclayout` uses `Hybrid 0.9.1.pcalcfunctions` and `Clipboard 0.8.pcalcfunctions`, while `Hybrid 0.8.pcalclayout` uses `Hybrid 0.8.pcalcfunctions` and `Clipboard 0.8.pcalcfunctions`).
Always use the latest version of each package unless you prefer an older layout. For example `Hybrid 0.8.pcalclayout` is the last one with the button `Ratio`.

## Recommended settings
#### *(to make PCalc look like the screenshot)*
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
**0.10:**
- changed some sizes and colours (Thanks to PCalc 3.6.1)
- fixed round and trunc
- added `roll up` key
- renamed clipboard and memory keys to use PCalc default naming
- added `×¹⁰` key and *Multiply 10 Times* function

**0.9.1:**
- Added *Binomial Coefficient (y, x)* function

**0.9:**
- Added *Sum 10 times* function and button `+¹⁰`

**0.8:**
- Removed *Ratio* and rearranged the second and third row of the layout.
