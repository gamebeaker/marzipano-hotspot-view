# marzipano-hotspot-view
This tool helps to set the view per hotspot from panorama tours created with https://www.marzipano.net/tool/

Example:
You have 3 rooms: A, B, C

-> is the navigation per hotspot from one room to another

A -> B -> C

C -> B -> A

navigate from A -> B the initial view is to room C

navigate from C -> B the initial view is to room C but should be to room A

This project aims to fix this problem.

Tutorial:
1. Download the latest release version here: [https://github.com/gamebeaker/marzipano-hotspot-view/releases/tag/0.0.1](https://github.com/gamebeaker/marzipano-hotspot-view/releases/download/0.0.1/marzipano-hotspot-view.zip)

2. Open the marzipano Project in your file explorer and extract the downloaded zip in app-files/

3. If promted confirm overwriting existing files.

4. Open index.html in an editor of your choice (i am using vscode).

5. Scroll to the end of the file to the line:

<script src="index.js"></script>

6. change this line to 

<script src="index-edit-view.js"></script>

![image](https://github.com/user-attachments/assets/e568b719-8bd7-4b27-8d1c-b08902aece85)

7. Open your marzipano project in your browser

Now you have 2 more buttons in your Project "Save new view" and "Download data.js"

![image](https://github.com/user-attachments/assets/f1577868-1323-4b92-853b-37237a55143d)

In top middle you can see from which picture you came from. If you navigate using the list on the left it will say null->your_picture.

![image](https://github.com/user-attachments/assets/59d10f83-700b-4164-9665-149e07cf7997)

8. Navigate to your starting point
In this example the starting point is picture C
9. Navigate with the hotspot button to your destination
In this example navigate C->B
In the top middle it looks like that in the example

![image](https://github.com/user-attachments/assets/31438892-25f1-413b-b18d-58a02c32f0e4)

wich means C->B

10. Move the view in the position that should be used after C->B and click the button "Save new view"
11. To check if it worked navigate C->B now it should be the new initial view.
This new initial view is only from C->B not from A->B. A->B is still the old view.
12. Save all new views for all the hotspots you want
13. click "Download data.js" and save the data.js file in your app-files folder overwriting the old data.js
14. Revert the change in index.html to
<script src="index.js"></script>
![image](https://github.com/user-attachments/assets/9ccc6f1d-e44b-49ee-8e91-a7a208e05a36)

14. Enjoy and report bugs
