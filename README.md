# about grid layout
grid is 2 d layout template

#grid-template-columns
Defines the columns and rows of the grid with a space-separated list of values.

grid-template-rows
We can also specify height of each row by using grid-template-rows property


grid-row -gap
To get gap between each item, we can use grid-row-gap

gird-column-gap
To get gap between each item, we can use grid-column-gap


#short hand notation
grid-template-columns: 100px 100px;
grid-template-rows: 50px 50px;
/* grid-row-gap:20px;
grid-column-gap: 20px; */
gap:20px 20px

repeat():
The  repeat() CSS function represents a repeated fragment of the track list,
allowing a large number of columns or rows that exhibit a recurring pattern to be
written in a more compact form.
Syntax : repeat(no_of_times,size)
for eg:
grid-template-columns: 100px 100px can be written as repeat(2,100px)


line-based-placement
row-start-line - 1
column-start-line - 2
row-end-line - 2
column-end-line - 3

#container > div:nth-child(2) {
grid-area:1/1/2/2;
}

#grid-template-area:
For building that what might be the steps student has followed
Identifying colors they need to pick up, based on label(color)
Placing those colored blocks wherever it is needed
In this case, we have placed boxes in this order
"blue green yellow
red maroon pink"
#container > div:nth-child(2) {
background-color: green;
grid-area:grn /* label - name */
}
#container > div:nth-child(3) {
background-color: yellow;
grid-area:ylw
}
#container > div:nth-child(4) {
background-color: red;
grid-area:rd
}

#Units of grid-template-columns:
Pixels
grid-template-columns: 100px 100px or repeat(2,100px)
Percentages
grid-template-columns: 50% 50% or repeat(2,50%)
// each column will take 50% width in reference to its parent
grid-template-columns: 1fr 1fr or repeat(2,1fr)
// each column will take 1 fraction width in reference to its parent



