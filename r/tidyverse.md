# tidyverse-cheatsheet
## Commands
| Command |Desc |
|  -| - |
| `dataset %>% select(var1, var2, var3)`|Use tidyverse to select a portion of a table by variables|
| `dataset %>% select(var1, var2, var3) %>% filter(var1 = "value1")` | Use tidyverse to select a portion of a table but filter by a condition|
| `dataset %>% select(var1, var2, var3) %>% filter(var1 = "value1") %>% na.omit()` | Removing N/A's|
| `dataset %>% select(var1, var2, var3) %>% filter(var1 == "value1") %>% na.omit() %>% mutate(var2 = var2/100)` |Change something about your data|
| `dataset %>% select(var1, var2, var3) %>% filter(var1 == "value1") %>% na.omit() %>% mutate(newVar = var2/var1)` |Add something to your data|
| `dataset %>% select(var1, var2, var3) %>% filter(var1 == "value1") %>% na.omit() %>% mutate(newVar = var2/var1) %>% group_by(var3) %>% summarise(var4 = mean(var3))` | Display the new data|
| `dataset %>% arrange(var)` | Sort by order (ascending) |
| `dataset %>% arrange(desc(var))` | Sort by order (descending)|
| `dataset %>% slice(1:10)` | Get top 10|


## Examples
| Command |Desc |
|  -| - |
| `starwars %>% select(gender,mass,height,species) %>% filter(species == "Human") %>% na.omit() %>% mutate(height = height / 100)  %>% mutate(BMI = mass / height^2) %>% group_by(gender) %>% summarise(Average_BMI = mean(BMI))`| Compare the average BMI between Males and Females