# r-cheatsheet
## main-cheatsheet

|dataset|col1|col2|col3|col4|col5|
|-|-|-|-|-|-|
|row1|||||||
|row2|||||||
|row3|||||||
|row4|||||||
|row5|||||||

| Command         | Desc                 |
| --------------- | -------------------- |
| `?dataset`      | More info on dataset |
| `dataset <- read.csv("dataset.csv")` | Load a csv as a variable |
| `nrow(dataset)` | Get the number of rows of a dataset|
| `data()`        | View all datasets   |
| `View(dataset)` | Select dataset      |
| `` | Get the numeric columns |
| `` | Get the factor columns |
| `mean(dataset$col1)` | Get the mean value of a column|
| `mean(dataset[dataset$col2=="val1", "col1"])` | Get the mean of a column based on the value of a second column |
| `sum(dataset$col1 == "val1")` | Get the number of times a column is equal to a value |
| `dataset[dataset$col1 == "oldValue", "col1"] = "newValue"` | Replace specific values in columns with new value |
| `` | |


