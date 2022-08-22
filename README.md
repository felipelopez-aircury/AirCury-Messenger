# Aircury-Messenger
*Aircury-Messenger* is an application that allows Aircury employees to chat with each other.
Non-Aircury users will not be able to take part in the application.

The system has three types of `users`:
* `User`
* `Admin`
* `SuperAdmin`

`Users` can send a `Message` (including files), to any other employee of the company.

They can also create groups.

`Messages` can be deleted and/or edited by the user who sent it.

`Messages` can be forwarded to any user/group.

`Users` can also react to any message sent by any user, including the same user.

They can also see all the reactions on that message.

Any `Message` can be replied individually, so in the case that we reply to a response it would form a tree of `messages`.

If these messages are forwarded, they should be displayed in the same way as in the original chat, including replies and/or reactions.

When creating a group, the `User` automatically becomes the `Admin` of that group.

In this case, the `Admin` of this group can also kick other `Users` out of the group.

The `Admin` of the group can also turn other `Users` of the group into `Admin`.

Every group has a public URL to join the group.

In order to join a group, there are 2 ways:
* Clicking on the public URL of the group sent by another `User`.
* Being added by the admin of the group.

`SuperAdmin` can do 2 more actions in addition to the `Admin` user within a group:
* They are able to read the deleted messages.
* They are able to read every version of the edited messages.

### Actions allowed depending on the role
Action|User|Admin|SuperAdmin
------|:---:|:---:|:---:
Send messages|✔|✔|✔
Reply to messages/replies|✔|✔|✔
Edit own messages|✔|✔|✔
Delete own messages|✔|✔|✔
Forward messages|✔|✔|✔
Send reactions to messages|✔|✔|✔
See reactions to a message|✔|✔|✔
Set/change profile picture|✔|✔ |✔
Create groups|✔|✔ |✔
Set/change group picture|✔|✔|✔
Set other group users as admins||✔|✔
Kick out other users of the group||✔|✔
Add new users to a group|✔|✔|✔
Read deleted messages|||✔
Read every version of an edited message|||✔

