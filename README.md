1. Key Screens and Their Functions
a. App.tsx
Navigation Setup: The entry point of the application, this file configures the navigation stack using React Navigation. It defines four main screens:
SecondPage: Displays available courses.
AddDishPage: Provides an interface for adding new dishes.
CourseDetailPage: Shows details for a selected course.
AddMenuPage: Allows users to compile selected dishes into a menu.
Type Definitions: Uses TypeScript to define parameter types for the screens, ensuring type safety across navigation.
b. SecondPage.tsx
Purpose: This screen serves as the primary interface for selecting courses.
Features:
Display of Courses: Lists different courses available (e.g., Starters, Mains, Desserts) in a clickable format.
Navigation to Add Dish: Includes a button to navigate to the AddDishPage, where users can input new dish details.
Dynamic State Management: Maintains the list of dishes and updates when new dishes are added.
c. AddDish.tsx
Purpose: Provides a form for users to enter details of new dishes they wish to add to the menu.
Features:
Input Fields: Fields for dish name, description, price, and category.
Submission: Upon submitting the form, the new dish is added to the existing list, and users receive a confirmation alert.
Callback Functionality: Utilizes a callback function to communicate the new dish back to the SecondPage for state updates.
d. CourseDetail.tsx
Purpose: Displays detailed information about a selected course and its associated dishes.
Features:
Dynamic Data Fetching: Retrieves dishes related to the selected course from the state.
List Rendering: Utilizes a FlatList to efficiently display each dish’s name, description, and price.
User Interaction: Allows users to click on dishes to view more details (if implemented in the future).
e. AddMenu.tsx
Purpose: Enables users to select multiple dishes and compile them into a new menu.
Features:
Selection Mechanism: Users can select dishes by clicking on them, which toggles their selection status.
Total Cost Calculation: As users select dishes, the app calculates and displays the total cost of selected items.
Confirmation: Provides an option to confirm the selection and navigate to a different screen, such as a summary or home page.
