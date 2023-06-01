# TODO-s-List
i have made a TODO list using HTML, CSS,  javascript (using local storage)
![image](https://github.com/tanvi120/TODO-s-List/assets/96731580/74d038da-8b00-4be2-b77b-1f82ebf64138)


The code provided is a simple JavaScript code that allows users to add tasks to a list and save the data using local storage.

Here's a breakdown of what the code does:

The code defines two variables inputBox and listContainer that store references to the corresponding elements in the HTML using getElementById.

The addTask() function is defined. It first checks if the inputBox value is empty. If it is, an alert is displayed to remind the user to write something. Otherwise, it creates a new li element, sets its inner HTML to the value of inputBox, appends it to the listContainer, and creates a span element inside the li with the "x" symbol. Finally, it clears the value of inputBox and calls the saveData() function.

An event listener is added to the listContainer using addEventListener. When a click event occurs, it checks the tagName property of the clicked element. If the tagName is "LI", it toggles the "checked" class on the clicked li element and calls saveData(). If the tagName is "SPAN", it removes the parent li element from the DOM and calls saveData().

The saveData() function is defined. It uses localStorage.setItem() to store the innerHTML of the listContainer in the browser's local storage with the key "data".

The showTask() function is defined. It retrieves the saved data from local storage using localStorage.getItem() and sets the innerHTML of the listContainer to the retrieved data.

The showTask() function is called at the end to populate the listContainer with the saved data when the page is loaded.

Overall, this code provides a basic functionality for adding tasks to a list, marking them as completed, and removing them, while persisting the data using local storage.




