# QCV

Typst template for CV

![](https://github.com/GuilloteauQ/qcv/blob/main/example.png)

## Example

```typst
#import "qcv.typ": *

#show: qcv.with()

#header("John Doe",
      email: "John.Doe@mail.com",
      webpage: "https://john.doe.org",
      orcid: "1111-1111-1111-1111")

#let max_year = 2024
#let min_year = 2017

#let entry(..args) = {
  raw_entry(min_year, max_year, ..args)
}

= Education

#entry(2020, 2023, title:"Phd Student", details: lorem(30))
```

See the PDF output [here](https://github.com/GuilloteauQ/qcv/blob/main/main.pdf)
