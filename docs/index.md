# Testing XSS in inline SVG

{% dot attack.svg
  digraph G {
  rankdir=LR
    Earth [peripheries=2]
    Mars
    Earth -> Mars
  }
%}
