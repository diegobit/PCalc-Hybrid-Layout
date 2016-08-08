# PCalc Hybrid layout and some functions

![Screenshot](/screenshots/hybrid_layout.png)

## Hybrid layout

The Hybrid layout is based on a heavily changed built-in *Programming* layout. It is designed with RPN in mind but also supports the Algebraic mode.

- numbers, operations, `2nd` and `RPN` have bigger fonts
- removed some operations I didn't need
- renamed `bin`, `oct`, `dec` and `hex` to `2`, `8`, `10`, `16`
- added buttons to manage the clipboard with the same behaviour as the memory
- added a button `logᵧx`
- added `+¹⁰` (See *Sum 10 times* function) at the place of `+` in 2nd mode
- moved most buttons

#### Issues

- some buttons are duplicated, one visible only in RPN mode and the other in Algebraic mode due to some limitations in the layout editor (I could edit the layout manually, but...):
  - `clip str` (RPN 1st, Alg 1st) / `clip +` (RPN 2nd, Alg 2nd)
  - `clip rec` (RPN 1st, Alg 1st) / `clip -` (RPN 2nd, Alg 2nd)
  - `logᵧx`: RPN and Algebraic use different functions
- `logᵧx`: the *ᵧ* should be a *y*
- no `trunc` button for Algebraic mode
- the `trunc` button hides `x~m` in RPN 2nd mode
- bad parenthesis and `÷` placement in Algebraic mode

## Functions

*Clipboard* package contains:
- *Add to Clipboard*
- *Copy to Clipboard*
- *Paste Clipboard alg*
- *Paste Clipboard rpn*
- *Subtract from Clipboard*

*Hybrid* package contains:
- *Logᵧx alg*
- *Logᵧx rpn*
- *Random [0-100]*
- *Random [x-y] alg*
- *Random [x-y] rpn*
- *Ratio*: solves equations *x:a=b:c* and *a:x=b:c*. Put a *0* instead of *x*. For example: *S2=a*, *S1=0*, *y=b*, *x=c*, then you can execute it. Available only in RPN mode
- *Sum 10 times*: sums the first 11 values of the RPN stack. Available only in RPN mode.

#### Issues and TODO
- *Ratio* doesn't solve equations *a:b=x:c* and *a:b=c:x*
- *Ratio* for Algebraic mode
- make *Sum 10 times* work for any RPN stack depth (not possible with current PCalc commands)

## Recommended settings
#### *(to make PCalc look like the screenshot)*
- Show Ticker Tape : OFF
- Theme > Samurai
- Digits > Thin
- Display > Vertical Number of Lines : 4 or 7
- Smart Resize : ON
- Accessibility > Use Dynamic Type : OFF
- Accessibility > Large Key Text : OFF
- Accessibility > Bold Key text : OFF
- Accessibility > Large Tape Text : OFF
- Advanced Settings > Hide Status Bar : OFF

## Changelog
**0.9:** Added *Sum 10 times* function and button `+¹⁰`
**0.8:** Removed *Ratio* and rearranged the second and third row of the layout.