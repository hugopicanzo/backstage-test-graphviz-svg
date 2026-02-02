# Testing XSS in inline SVG

graph G {
  "XSS" [label="<img src=x onerror=alert(document.domain)>", URL="javascript:alert('XSS_via_Link')"];
}
