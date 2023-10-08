# List View
- It is a view which groups several items and display them in vertical scrollable list.  
- Items are automatically inserted to the list by the help the of adapters from source such as database or array.
- Adapter actually acts as a bridge between UI component and source.
- Adapter holds the data from the source and store it into adapter view, the view can take the data from adapter view and display it on the screen.
```java
ArrayAdapter = new ArrayAdapter<String>(this, R.layout.ListView, StringArray)
```

```xml
<Linear Layout xmls:android="http://schemas.android.com/apk/res/android">
	<List View 
		android:id="@+id/list" />						
</ Lineat Layout>
```
![List View](https://media.geeksforgeeks.org/wp-content/uploads/20200629182237/IMG20200629181735.jpg)

# Grid View
- It is a subclass of **Adapter View** that is used to display items in two-dimensional scrolling grid.
- Items are inserted into grid layout are from database or from array.
- **setAdapter()** method is used to join the adapter with GridView.
- The main function of the adapter in GridView is to fetch data from a database or array and insert each piece of data in an appropriate item that will be displayed in GridView.
- **XML Attributes of grid view:** `android:numColumn`, `android:verticalSpacing`, `android:horiozntalSpacing`
```xml
<Linear Layout = "https://schemas.android.com/apk/res/android">
	<Grid View
		android:id="@+id/gridView"
		android:numColumns="2"
		android:horizontalSpacing="5dp"
		android:verticalSpacing="5dp"
</Linear Layout>
```
![Grid View](https://media.geeksforgeeks.org/wp-content/uploads/20201115011853/grid.jpg)

# Card View
- It is a widget in android that can be used to display any short of information in rounded corners.
- Rich feels and can display the view on top of each other.
- The main part is, it can extend frame layout and displayed on all platform.
```xml
<com.android.material.card.MasterCardView
	android:id="@+id/card"
	android:layout_width="match parent"
	android:layout_height="match parent">
	<Linear Layout>
		<!-- Item of Cards -->
	</Linear Layout>
</com.android.material.card.MasterCardView>
```
![Card View](https://media.geeksforgeeks.org/wp-content/uploads/20201128134017/Screenshot20201128133902450comgtappdevelopersfrescoimageloading1.jpg)

# Recycler View
- It is a view group added to android studio as a successor of grid and list view.
- It is an improvement of Grid and List View.
- This improvement is achieved by recycling the views that are outside the visibility of the user.
- **For example**, if a user scrolled down to a position where items 4 and 5 are visible; items 1, 2, and 3 would be cleared from the memory to reduce memory consumption.
![Recycle View](https://media.geeksforgeeks.org/wp-content/uploads/gfg1-1.jpg)

# Adapters
- It basically connects user interface with the data source.
- Adapter object acts as a bridge between adapter view and data source.
- Adapter view is an object can is extended from `AdapterView` Class.
- Data source is a place where data is stored in a structured manner.
![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/03/adapter-in-android.jpg)
## Base Adapter
- It is the general implementation of an adapter that is extended in other android adapters for their use.
- Other android adapters extend it to create a custom Adapter for displaying a common custom list item.
```java
public class MyAdapter extends BaseAdapter{
	// Code
}
```
## Array Adapter
- It is used when we used to display data that is stored in array format.
- It uses `Object.toString()` for each data object to create a view, and then place the result in a Text View.
```java
String CourseList[] = {'java', 'kotlin', 'xml', 'dart', 'swift'};
ArrayAdapter arrayAdapter = new ArrayAdapter(this, R.layout.list_view, R.id.textView, courseList[]);
```

# View Holder

# Dialog  Box
- It shows the alert message and gives the message in yes or no.
- An alert dialog displays to warn you and then according to your response takes the next step.
- Android alert dialog is built up of **Text**, **MessageArea**, and **Action Button.**
- Alert Dialog code has 3 methods: `setTitle()`, `setMessage()`, `setIcon()`.
- We can add buttons, `setPositiveButton`, `setNegativeButton` to out Alert Dialog Box.
![Dialog Box](https://media.geeksforgeeks.org/wp-content/uploads/alert-dialog-box.png)

# Toast
- It is used to display information for a short period of time.
- It displays feedback message.
- It takes very little space, while the whole activity is visible and interactive to the user.
- It disappears automatically.
- Another type of toast is **custom toast**, in which an image can be used instead of a message.
- `Toast.makeText(getApplicationContext(), "Toast Message", Toast.Lenght_Sort).show()`.
![Toast](https://media.geeksforgeeks.org/wp-content/uploads/Toast.jpg)

# Popup
- Android Popup Menu displays the menu below the anchor text if space is available, otherwise above the anchor text.
- It disappears if you click outside the popup menu.
![](https://static.javatpoint.com/images/androidimages/popup1.png)![](https://static.javatpoint.com/images/androidimages/popup2.png)
# Fragment
- It is a part of activity, also known as sub activity.
- An activity consists of multiple fragment.
- It provides flexibility to auto-adjustable based on the device screen size to make user interaction better.
- The fragment exists inside the activity and its lifecycle depends on that of activity.
- Fragments attaches and detaches with activity to work.
- Each fragment has its own lifecycle.
![Fragment Life Cycle](https://media.geeksforgeeks.org/wp-content/uploads/20230120013956/AndroidFragmentLifecycle.png)

# Material Design
- These components(MDC) offers designers and developer a way to implement material design into their application.
- Material design is inspired by the physical world and its texture like how they look like and hoe cast shadow.
- It reimagines the surface of ink and paper.
- It is developed by the core team and the UX designer at Google.
- Enables reliable development workflow to build beautiful and functional UI.
- These designs are fully guided the Google.
- **These documentation covers:**
	1. Color and theming.
	2. Typography.
	3. Material design component.
	4. Shaping the material design component.
- **Navigation**, **Tool Bar**, **Floating Button**.
