# Testing XSS in inline SVG

{% dot attack.svg
  digraph G {
  rankdir=LR
    Earth [peripheries=2]
    Mars
    Earth -> Mars
    "XSS" [label="<img src=x onerror=alert(document.domain)>", URL="javascript:alert('XSS_via_Link')"];
  }
%}
