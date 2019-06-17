[[styleguide-material-for-figures]]
Boutros lab style guie for plots and figures material of published manuscripts
----------------------------------------------

# B110 Style guide

This Style guide should serve as a general guideline. 

The **Rmarkdown** file serves as template for creating tidy graphics of the most
used fata vizualizations.


## RSytles

General color scheme.

```r

sgi_blue    = '#5087C8'
sgi_yellow1 = '#F2EE35'
sgi_yellow2 = '#FED98E'
b110_grey   = '#808080'
b110_grey_light   = '#909090'
b110_transparent_black = alpha('#000000',0.5)

```

General plotting style.

```r

theme_b110<-function(){
  theme_classic() +
  theme(
    axis.text=element_text(size = 16), 
    axis.title=element_text(size = 16),
    plot.title = element_text(size = 22,hjust = 0.5,face="bold"),
    legend.title = element_text(size = 22),
    legend.text = element_text(size =16),
    legend.position = "bottom"
    )
}

```

## CSS styles for web-pages and apps

```css
#allcontent {
      font-family: 'Open Sans', sans-serif;
      width: 800px;
      text-align: left;
      /*font-family: Verdana, Arial, sans-serif;*/
      font-size: 12px;
      margin-left: auto;
      margin-right: auto;
}

td.header{      border:0px;
                        background-color: #2662C3;
                        font-family: 'Open Sans', sans-serif;
                font-size: 16px;
                text-align: center;
                border-radius: 5px
        }
td.header:hover{background-color: #5692F3;}

a:link {
      color: #333;
      font-family: 'Open Sans', sans-serif;
      /*font-family: Verdana;*/
      text-decoration: underline;
}

a:visited {
      color: #333;
      font-family: 'Open Sans', sans-serif;
      /*font-family: Verdana;*/
      text-decoration: underline;
}
```
And more to be added...