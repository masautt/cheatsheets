# r-cheatsheet
## tidyverse-cheatsheet

|dataset|col1|col2|col3|col4|col5|
|-|-|-|-|-|-|
|row1|||||||
|row2|||||||
|row3|||||||
|row4|||||||
|row5|||||||
## Commands
| Command |Desc |
|  -| - |
| `dataset %>% select(col1, col2, col3)`|Use tidyverse to select a portion of a table by column|
| `dataset %>% select(col1, col2, col3) %>% filter(col1 = "val1")` | Use tidyverse to select a portion of a table but filter by a condition|
| `dataset %>% select(col1, col2, col3) %>% filter(col1 = "val1") %>% na.omit()` | Removing N/A's|
| `dataset %>% select(col1, col2, col3) %>% filter(col1 == "val1") %>% na.omit() %>% mutate(col2 = col2/100)` |Change something about your data|
| `dataset %>% select(col1, col2, col3) %>% filter(col1 == "val1") %>% na.omit() %>% mutate(newcol = col2/col1)` |Add something to your data|
| `dataset %>% select(col1, col2, col3) %>% filter(col1 == "val1") %>% na.omit() %>% mutate(newcol = col2/col1) %>% group_by(col3) %>% summarise(col4 = mean(col3))` | Display the new data|
| `dataset %>% arrange(col`)` | Sort by order (ascending) |
| `dataset %>% arrange(desc(col`))` | Sort by order (descending)|
| `dataset %>% slice(1:10)` | Get top 10|


## Examples
| Command |Desc |
|  -| - |
| `starwars %>% select(gender,mass,height,species) %>% filter(species == "Human") %>% na.omit() %>% mutate(height = height / 100)  %>% mutate(BMI = mass / height^2) %>% group_by(gender) %>% summarise(Average_BMI = mean(BMI))`| Compare the average BMI between Males and Females