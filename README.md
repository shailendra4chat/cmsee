# CMSEE UI - User Guide

## What is CMSEE?

CMSEE is new software to manage host machines, typically but not exclusively at edge locations catering for low bandwidth and intermittent connectivity scenarios.

CMSEE has various modules and features as follows:

## Login

The Login Page allows the users to log in and every user must log in to the CMSEE portal to use the features in the application.
It has two fields, the Email, and the Password. The inputs will be compared with our user database and the password verified. Once the verification is complete, the user will proceed to the Dashboard page.

![Login Screen](https://github.com/shailendra4chat/cmsee/blob/main/login.png)

### Reset Password

If you have forgotten your password, you may reset it by clicking the "Reset Password" link. It will redirect you to the “Password Setup” page. You are then required to enter your registered email address and click "Send" to proceed to reset your password.

An email notification will be sent to you. Once you check your registered email and by clicking on the reset password "link". It will direct you to enter your desirable new password. If all steps are followed and completed, a successful password reset confirmation will be displayed. You will then be able to enter the system again. 

## Dashboard

It is the home page of the CMSEE UI.
On the right-hand side of the header, you will find a Menu with “Change Password” and “Logout” links.

![Dashboard Screen](https://github.com/shailendra4chat/cmsee/blob/main/dashboard.png)

### Change Password

By clicking the “Change Password” link in the header right-hand side menu, the user will be redirected to the change password screen.

You are then required to enter a new password, confirm a new password, and click "Change Password" to proceed to change your password.
A notification will be displayed on the screen, and the user will be logged out to use the new password while logging in to the system.

![Change Password Screen](https://github.com/shailendra4chat/cmsee/blob/main/change-password.png)

## Hosts

In the hosts page, a user can admit or manage admitted hosts.

### Admit Host

A user can admit host by UUID or MAC-Address. Multiple hosts can admitted at a time by providing multiple UUIDs or MAC-Addresses.

A user can select Organization Group, Area, Location and provide Label for the host.

A user must ensure the latest "Artisan" executable available on your host.

![Admit Host Screen](https://github.com/shailendra4chat/cmsee/blob/main/admit-host.png)

### Manage Hosts

On the Manage hosts page a user can view all the admitted hosts based on the Organization Group, Area, Location and Label filter.

Hosts grid contains the information about the admitted host and a action column with various features.

- Update label: A user can add/update host label by clicking on "Update label" icon button.
- View events: A user can navigate to the view events page to view all the events related to hosts by clicking on "View events" icon button.
- View host details: A user can view host details by clicking on "View host details" icon button.
- Decommission host: A user can decommission a host by clicking on "Decommission host" icon button.

Hosts grid also has a "Refresh hosts" icon button which will fetch the latest hosts and update the grid.

![Manage Hosts Screen](https://github.com/shailendra4chat/cmsee/blob/main/manage-hosts.png)

## Commands

In the commands page, a user can create or manage commands.

### Create Command

A user needs to fill details to create a command. Below are the fields details:

- Command: A user must provide a name of the command.
- Description: A user must provide description of the command.
- Package: A user must select desired Artisan package which will run on the host.
- Tags: A user must select desired package tag.
- Function: A user must select a function available under the selected package.
- Collection: A collection is an optional field. It helps to pre-filled the variables and secrects. A user can apply the Collection by clicking on "Apply Collection" button.

Once a user selects the desired function, based on the selected package (If package has) variables and secrects will be populated.

By default only those variables will be displayed which does not has the default value, but if a user clicks on "Show Defaults" button, all the variables will be displayed.

User can clicks on "Show Secrects" button to view the value of the secrects.

"View Field Help" button is provided to help user to understand details about variables and secrects.

After filling all the required fields a user can click on "Create Command" button to create a new command.

![Create Command Screen](https://github.com/shailendra4chat/cmsee/blob/main/create-command.png)

### Manage Commands

On the Manage commands page a user can view all the commands. In the grid, user can sort and filter commands. It has action column which contains two buttons.

- Update command: A user can update the commands by clicking on "Update command" icon button. It will redirected the user to the update command screen.
- Delete command: A user can delete a command by clicking on "Delete command" icon button.

![Manage Commands Screen](https://github.com/shailendra4chat/cmsee/blob/main/manage-commands.png)

## Jobs

In the jobs page, a user can create or manage jobs. Using the Job screen a user can run a command on a admitted host.

### Create Job

A user needs to fill details to create a job. Below are the fields details:

- Organization Group: A user must select Organization Group to get the list of hosts admitted.
- Area: A user may select Area based on the selected orgnization group to filter hosts.
- Location: A user may select Location based on the selected Area to filter hosts.
- Label: A user may filter hosts by label.
- Command: A user must select desired Command which will run on the host.
- Name: Job name will be automatically filled based on the command. A user may change the job name.
- Notes: A user may add the notes for the reference.

Once a user clicks on Apply button, all the hosts will be displayed in the Hosts grid. It has Refresh hosts icon button as well to fetch the latest hosts.

A user can select one or many hosts by clicking on checkbox againsts each host to run the desired command.

After filling all the required fields a user can click on "Create Job" button to create a new job.

![Create Job Screen](https://github.com/shailendra4chat/cmsee/blob/main/create-job.png)

### Manage Jobs

In the Manage Jobs page, a user can view all the jobs details in the grid.

User has to click on Apply to view Job(s). Grid contains Batch Id and other useful information along with action column which contains two buttons.

- View notes: A user can view the notes related to the batch by clicking on "View notes" icon button
- Download notes: A user can download notes by clicking on "Download notes" icon button.

In the Grid, Batch Id is clickable and it redirected user to the Job details page.

![Manage Jobs Screen](https://github.com/shailendra4chat/cmsee/blob/main/manage-jobs.png)

### Job Details

In the Job Details page, a user can view all the jobs details in the grid.

User can filter jobs by Organization Group, Area, and Location.

Jobs grid has a Refresh button to fetch the latest jobs status. It has action column which contains two buttons.

- View job logs: A user can view the job logs by clicking on "View job logs" icon button.
- Download job logs: A user can download job logs by clicking on "Download job logs" icon button.

In the Grid, a user can check the current status of job as well.

![Job Details Screen](https://github.com/shailendra4chat/cmsee/blob/main/job-details.png)

## Events

In the manage events page, a user can view events. User can filter events by various parameters and click on Apply button to view the filtered events.

![Events Screen](https://github.com/shailendra4chat/cmsee/blob/main/events.png)

## Collections

In the collection page, a user can create or manage Collections.

Collection helps user to create a pre-defined variables set while creating a command. On the Create Command screen, a user may apply collection.

### Create Collection

A user needs to fill details to create a collection. Below are the fields details:

- Name: A user must provide a name of the collection.
- Description: A user may provide description of the collection.
- Tags: A user may provide tag(s) for the collection.
- Key/Value: In the Key/Value table, a user must add at least one key/value to create a new collection. Add button [+] is provided to add more key/value. A Remove [x] button is also provided to remove the existing key/value pair.

After filling all the required fields a user can click on "Create Collection" button to create a new collection.

![Create Collection Screen](https://github.com/shailendra4chat/cmsee/blob/main/create-collection.png)

### Manage Collections

On the Manage collections page a user can view all the collections. In the grid, user can sort and filter collections. It has action column which contains two buttons.

- Update collection: A user can update the collection by clicking on "Update collection" icon button. It will redirected the user to the update collection screen.
- Delete collection: A user can delete a collection by clicking on "Delete collection" icon button.

![Manage Collections Screen](https://github.com/shailendra4chat/cmsee/blob/main/manage-collections.png)

## Admin

This section provides below features to the user.

### Create User

A user needs to fill details to create a user. Below are the fields details:

- Email: A user must provide an Email of the User. Email should be valid and unique.
- Manage Configuration: A user must provide at least one configuration. Based on the configuration provided, a user will be created and use the system.

After filling all the required fields a user can click on "Create User" button to create a new user.

An email notification will be sent to the user. Once user checks registered email and by clicking on the reset password "link". It will direct you to enter your desirable new password. If all steps are followed and completed, a successful password reset confirmation will be displayed. You will then be able to enter the system again. 

![Create User Screen](https://github.com/shailendra4chat/cmsee/blob/main/create-user.png)

### Manage Users

In the Manage Users page, a user can view all the users details in the grid.

Grid contains Configuration and other useful information along with action column which contains two buttons.

- Manage configurations: A user can add/update configuration by clicking on "Manage configurations" icon button.
- Delete user: A user can delete a user by clicking on "Delete user" icon button.

![Manage Users Screen](https://github.com/shailendra4chat/cmsee/blob/main/manage-users.png)

### View Locations

In the View Locations page, a user can view all the orgnization group, area and locations in the TREE view.

A user can clicks on location to view all the host available in that particular location.

Host table also provides information about if host connectivity and last seen along with hostname and label.

![View Locations Screen](https://github.com/shailendra4chat/cmsee/blob/main/view-locations.png)

### Refresh Locations

In the Refresh Locations page, a user can update the current logistics information like orgnization group, area and location.

To update locations, excel workbook in the correct format should be uploaded in the system. It will be validated and if no host is already exist in any location it will provide a configuration to go ahead and all the logistics information will be updated based on the excel workbook data.

![Refresh Locations Screen](https://github.com/shailendra4chat/cmsee/blob/main/refresh-locations.png)

