In the MainActivity, the code initializes UI components for username and password input, buttons for login, sign-up, and forgot password. It establishes a connection with a DatabaseHelper for user authentication. The login function validates user credentials using the database and, if successful, saves the session data using SharedPreferences. If credentials are invalid, it displays a toast message. The SignUpPage button redirects users to the registration page, while the ForgotPassword button navigates to the password recovery page. The code facilitates login management, navigation to sign-up, and password recovery.

<img width="260" alt="Screenshot 2024-09-16 at 2 24 15 PM" src="https://github.com/user-attachments/assets/1e4c609f-24c6-4304-8ac1-0c2e94cb00df">

In the SignUpActivity, the code initializes UI components for user input, including fields for username, password, contact details, profile photo, and gender selection via a spinner. It implements an image picker for the profile photo and a date picker for the birthday, which also calculates the user’s age. Basic validations for input fields are performed, including checks for email format and phone number length. The registration process saves user details in the database, ensuring unique username, email, and phone number. The profile picture, if available, is converted to bytes before saving in the database.

![PHOTO-2024-09-16-14-34-50](https://github.com/user-attachments/assets/2eabfa52-0351-4e4a-ac81-59dc73a6522c)

![WhatsApp Image 2024-09-16 at 16 55 19](https://github.com/user-attachments/assets/c1b2f311-6fd3-4ff4-aa5b-baa594ed24ad)


In the ForgotPasswordActivity, the code initializes UI components for inputting username/email and date of birth, with a date picker for selecting the birthdate. The resetPassword method validates inputs and checks the database for a matching user and date of birth. If a match is found, a dialog prompts the user to set a new password, updating the database upon confirmation. If inputs are empty or do not match, appropriate toast messages are displayed. The activity ensures user identity verification and secure password reset functionality.

![WhatsApp Image 2024-09-16 at 14 41 13](https://github.com/user-attachments/assets/bc7aca35-fd53-4a01-bac2-5f2743c812e1)

![WhatsApp Image 2024-09-16 at 14 41 48](https://github.com/user-attachments/assets/dd68dc06-0d8a-4551-8609-9c5c419cc800)

The call_dial activity allows users to input, call, and save phone numbers. It initializes UI components like EditText for phone input and buttons for clearing, calling, and saving contacts. The "Clear" button resets the input, while the "Call" button checks if the user has the necessary permission to make calls and requests it if not. The makePhoneCall method hides the keyboard and initiates the call. The "Save" button navigates to the contacts screen. Additionally, the inputNumber method appends digits to the phone number when the corresponding buttons are clicked

![WhatsApp Image 2024-09-16 at 16 28 12](https://github.com/user-attachments/assets/5e81eff6-a6d6-42d3-9946-8a3f66dc5175)

The Contacts activity manages a list of contacts with functionalities for adding, editing, and deleting entries. It initializes the UI, including a ListView and buttons for adding contacts or navigating to the dial pad. Contacts are stored in SharedPreferences and are loaded or saved as JSON using Gson. The activity supports adding contacts through a dialog and validating phone numbers. It also handles contact editing and deletion with confirmation dialogs, and can make phone calls if the appropriate permission is granted.

![WhatsApp Image 2024-09-16 at 16 34 07](https://github.com/user-attachments/assets/619d83bf-4c32-4323-90c9-50138b3288f3)


The ToDoList activity manages a list of tasks, allowing users to add, view, edit, and delete tasks. It uses SharedPreferences to persist tasks and loads them into a ListView using an ArrayAdapter. Tasks can be added with a name, description, due date, and due time, and are stored as concatenated strings. The activity includes date and time pickers for setting task deadlines and supports marking tasks as completed or deleting them with confirmation dialogs. Tasks are updated in the view and saved to preferences upon changes.

![WhatsApp Image 2024-09-16 at 16 46 57](https://github.com/user-attachments/assets/e0283bff-1137-48d1-8646-afbb96a9c76d)

The List activity allows users to manage a list of items with features for adding and deleting items. It initializes views, including an EditText for input, an ImageView for adding items, and a ListView for displaying the list. Items are persisted using SharedPreferences, with the list updated accordingly. Users can add new items, which are saved and displayed, and delete items via a long-click context menu. Changes to the list are saved to SharedPreferences to persist between sessions.

![WhatsApp Image 2024-09-16 at 16 53 32](https://github.com/user-attachments/assets/b8583c4b-5bdc-41b5-9cac-5b6640599bc2)

The ProfileActivity displays detailed user profile information retrieved from a database. It initializes various TextView elements and an ImageView to show user details like username, full name, email, phone, birthday, and more. Depending on the type of identifier (username, email, or phone number), it queries the database and displays the user's information. It also includes functionality to handle profile picture loading and provides an option to navigate to an EditProfileActivity for modifications.!

![WhatsApp Image 2024-09-16 at 16 55 19](https://github.com/user-attachments/assets/b4b17257-b152-4eff-ba2d-0bf7a05f660d)
