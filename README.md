# Boutros lab style guide for plots and figures material of published manuscripts

----------------------------------------------

This Style guide should serve as a general guideline. 

The **Rmarkdown** file serves as template for creating tidy graphics of the most
used data visualizations. The general color scheme should be used for highlights 
in figures. The interaction scheme, for everything related to genetic interactions. 

## General advice on color and data visualization

Consider Gestalt principles:
1. figure-ground  
 The figure-ground principle states that people instinctively perceive objects as either being in the foreground or the background.

2. similarity  
 The principle of similarity states that when things appear to be similar to each other, we group them together. And we also tend to think they have the same function.
 
3. proximity  
 The principle of proximity states that things that are close together appear to be more related than things that are spaced farther apart.

4. common region  
 The principle of common region is highly related to proximity. It states that when objects are located within the same closed region, we perceive them as being grouped together.

5. continuity  
 The principle of continuity states that elements that are arranged on a line or curve are perceived to be more related than elements not on the line or curve.

6. closure  
 The principle of closure states that when we look at a complex arrangement of visual elements, we tend to look for a single, recognizable pattern.
 
7. focal point 
 The focal point principle states that whatever stands out visually will capture and hold the viewer’s attention first.

[Color Coding by Bang Wong](https://www.nature.com/articles/nmeth0810-573)

## R Styles

General color scheme. <br><div style='background-color: #4285f4; width:20px; height:20px;'>test</div><div style='background-color: #008744; width:20px; height:20px;'></div><div style='background-color: #ffa700; width:20px; height:20px;'></div><div style='background-color: #d62d20; width:20px; height:20px;'></div>


```r

b110_grey   = '#808080'
b110_grey_light   = '#909090'
b110_transparent_black = alpha('#000000',0.5)

b110_blue= '#4285f4'
b110_green= '#008744'
b110_yellow= '#ffa700'
b110_red= '#d62d20'

```

Genetic interaction color scheme.

```r

sgi_blue    = '#5087C8'
sgi_yellow1 = '#F2EE35'
sgi_yellow2 = '#FED98E'

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

Gestalt list was adapted from [Usertesting](https://www.usertesting.com/blog/gestalt-principles/)