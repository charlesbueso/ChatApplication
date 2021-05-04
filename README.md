# ChatApplication
COMP 363 Chat Application Carlos Bueso Luis Santos

First we set up the project:
- Connected to Firebase database
- Created main activity as well as supporting activities
- Added basic esthetic design

The worked on authentication with email and password:
- StartActivity class (lets you choose between register and login)
- Added basic design
- Created LoginActivity.java 
- Lets you input an email and a password for existing users
- RegisterActivity.java lets you input 3 fields (username, email, password)
- We took care of certain exceptions like password length, and not typing anything
- Users get stored in Firebase database.

Then we added User.java to show user information, as well as to implement
functionalities like autologin and logout. 

We also added a class that will later be of more use, called Fragment, which will
inherit UsersFragment and ChatsFragment. These classes will allow to store all
fragments needed for both the Users panel in the Tab Layout, as well as the 
Chats panel in the Tab Layout.

Then to display the users, the class UserAdapter was created to include all the
users that the current logged in account has added. Small design was added
to this display. Later more design will be implemented to be able to open the
user's account, information, and shared files with that person.

Then class MessageActivity was created to start working on sending messages
between users, through Firebase.Simple design was implemented to create
individual chat activities for each user. 

We still have a long way to go, and the things to be implemented are:
- Displaying messages between users.
- Display specific users with whom you share a conversation.
- Obtain the profile of the user as well as shared files.
- Change your profile picture as well as access all shared files.
- Show online/offline status.
- Search algorithms for added users.
- Add function to be able to see if receiver has seen a message.
- Implementing initial esthetic design.


UPDATE
For Displaying Messages, 
We worked a bit more on the design background chat items,
chat item layouts, MessageAdapter class, 
MessageActivity class. (Show MessageAdapter.java, MessageActivity.java)

Then we displayed users with whom you have messages.
We worked on the design fragment chats, selecting users
from chat and also the method readChats. (Show ChatsFragment)

For creating the user profile, we created a fragment and 
added it to the tablayout. Also showing the user info. (Show ProfileFragment) 

To add profile photo we added the library and permissions from firebase to
store the images on the database. (Profile fragment)

To add the search bar for users we updated the user fragment, and also 
added search values on firebase database. We also added a function to mark
messages as seen but we are still having trouble with that.

Finally, added the functionality of reseting password, where we created 
the layout (resetPassword) as well as the Activity. Firebase also allows 
a very user-friendly option to implement it.
