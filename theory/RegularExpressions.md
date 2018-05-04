## Find regexes that match the following:

 - "antelope rocks out" & "antelopes rock out" - `/antelopes? rocks? out/g`
 - "goat" & "moat" but not: "boat" - `/[^b]oat/g`
 - Dates in YYYY-MM-DD format - `/\d{1,4}-\d{1,2}-\d{1,2}/g`