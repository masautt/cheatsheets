# r-cheatsheet
## ggplot-cheatsheet

|dataset|col1|col2|col3|col4|col5|
|-|-|-|-|-|-|
|row1|||||||
|row2|||||||
|row3|||||||
|row4|||||||
|row5|||||||

| Command         | Desc                 |
| --------------- | -------------------- |
|`ggplot(data=dataset) + geom_bar(mapping = aes(x=col1))`| Plot a bar graph of one column |
|`ggplot(data=dataset) + geom_bar(mapping = aes(x=col1)) + scale_x_continuous(breaks = 1:10)`| Plot bar graph and divide the x axis by 10 |
| `ggplot(data=dataset) + geom_point(mapping = aes(x=col1, y=col2))` | Plot a scatterplot with 2 columns |
| `ggplot(data=dataset) + geom_point(mapping = aes(x=col1, y=col2)) +  scale_x_continuous(limits = c(1,10), breaks = 1:10) +  scale_y_continuous(limits = c(1,10), breaks = 1:10)` | Plot a scatterplot with 2 columns and set the x and y axis limits to 10 |
| `ggplot(data=dataset) + geom_point(mapping = aes(x=col1, y=col2)) + labs(title="col1 vs col2")` | Plot a scatterplot with 2 columns and add a tile |
| `ggplot(data=dataset) + geom_point(mapping = aes(x=col1, y=col2)) + xlab("Column1") + ylab("Column2")` | Plot a scatterplot with 2 columns and add labels to x and y axis |
|`ggplot(data=dataset) + geom_boxplot(mapping = aes(x=col1, y=col2))`|Plot a boxplot with 2 columns|