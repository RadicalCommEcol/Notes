# Radical Style
Remember to check readbility and color-blindness compatibility!
### 3 colors:
- <span style="color: #008000;">Office green</span>
    - hex: #008000
    - rgb: [0, 128, 0]
- <span style="color: #4682b4;">Steel blue</span>
    - hex: #4682b4
    - rgb: [70, 130, 180]
- <span style="color: #b8860b;">Dark goldenrod</span>
    - hex: #b8860b
    - rgb: [184, 134, 11]

And alternative to dark goldenrod: 
- <span style="color: #e66826;">Orange</span>
    - hex: #b8860b
    - rgb: [230,	104,	38]



### More colors:
The `RColorBrewer` package offers several color palette for R. For Diverging palettes we can use `Set2`.

```
install.packages("RColorBrewer") # CRAN version

library(RColorBrewer)

colors <- RColorBrewer::brewer.pal(n = my_n, name = "Set2") 
````


### Icons:
Better use them in vectorial format.

#### Plants:
- [Chamaemelum fuscatum](https://www.phylopic.org/images/39335c0c-f879-4df6-90d5-e4f65d90d04e/chamaemelum-fuscatum)
- [Parapholis incurva]()
#### Pollinators:
- [Bombus terrestris](https://www.phylopic.org/images/750eeb4f-7ca5-49ff-a814-27a12d0cb13a/bombus-terrestris)


### Interesting links:
- [Data viz](https://drive.google.com/file/d/1LouVvISCRlWkItZgzoHcgoU5Q1VyHT4U/view) by Dan Larremore.
- [How to make your data POP](https://www.youtube.com/watch?v=UP08IWT0uXw) by Paula Martín (EBD seminar series).  