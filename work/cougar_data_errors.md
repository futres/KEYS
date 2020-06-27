grepl function not working
```
## f -> female & m -> male
cougar_sex <- function(x, y) {
  if(isTRUE(grepl("f|F|female", x))){
    x[,y][x[,y]] <- "Male"
  }
  else{
    x[,y][x[,y]] <- "Female"
  }
}
```
piping not working 
```
cougar_data %>%
cougar_status("Status")%>%
cougar_sex("Sex")%>%
cougar_melt("Length", "Weight")%>%
cougar_add_col()%>%
cougar_measurement_unit("measurementUnit", "variable")
```
