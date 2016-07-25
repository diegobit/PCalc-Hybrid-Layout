# PCalc Hybrid layout and some functions

### 1. Hybrid layout

The Hybrid layout is based on a heavily changed built-in *Programming layout*. It is designed with RPN in mind but supports also the Algebraic mode.

- numbers, operations, 2nd and RPN have bigger font
- removed some operations I didn't need
- renamed *bin*, *oct*, *dec* and *hex* to *2*, *8*, *10*, *16*
- added buttons to copy use the clipboard with the same behaviour as the memory
- added a button $log_y x$
- moved most buttons

#### Issues:

- some buttons are duplicated, one visible only in RPN and the other in Algebraic mode due to some limitations in the layout editor (I could edit the layout manually, but...):
  - *clip str* (RPN 1st, Alg 1st) / *clip +* (RPN 2nd, Alg 2nd)
  - *clip rec* (RPN 1st, Alg 1st) / *clip -* (RPN 2nd, Alg 2nd)
  - $log_y x$: RPN and Algebraic use different functions
- $log_y x$: the *y* is actually a *ᵧ*
- no *trunc* button for Algebraic mode
- the *trunc* button hides *x~m* in RPN 2nd mode
- bad parenthesis and *÷* sign placement in Algebraic mode

### 2. Functions

*Clipboard* contains:

- Add to Clipboard
- Copy to Clipboard
- Paste Clipboard alg
- Paste Clipboard rpn
- Subtract from Clipboard

*Hybrid* contains:

- Logᵧx alg
- Logᵧx rpn
- Random [0-100]
- Random [x-y] alg
- Random [x-y] rpn
- Ratio: solves equations $x:a=b:c$ and $a:x=b:c$. Put a *0* instead of *x*. For example: S2=a, S1=0, y=b, x=c, then you can execute it. Available only in RPN mode.

#### Issues and TODO:
- Ratio doesn't solve equations $a:b=x:c$ and $a:b=c:x$
- to make Ratio for Algebraic mode

### Changelog
**0.8:** Removed ratio and rearranged the second and third row.