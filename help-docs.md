# Simply Taskful Help Documentation

## Table of Contents

- [Getting Started](#getting-started)
- [Local Mode & Cloud Sync](#local-mode--cloud-sync)
- [Task Management](#task-management)
- [Categories](#categories)
- [List Sharing](#list-sharing)
- [Notifications & Reminders](#notifications--reminders)
- [Repeating Tasks](#repeating-tasks)
- [Views & Filters](#views--filters)
- [Widgets & Shortcuts](#widgets--shortcuts)
- [Useful Tools](#useful-tools)
- [Completion Stats](#completion-stats)
- [Tips & Tricks](#tips--tricks)
- [App Support & Feedback](#app-support--feedback)

---

## Getting Started

Welcome to Simply Taskful! This guide will help you get the most out of your task management experience.

### Getting Started

- When you first open the app, you'll see the login screen
- You can sign in with an existing account, create a new account, or continue without an account
- If you continue without an account, the app will use local mode (see Local Mode & Cloud Sync section)
- Once you're in the app, you can start creating tasks immediately

### Creating Your First Task

- Tap the plus (+) button in the bottom menu
- Enter a task title (required)
- Optionally add a description
- Set a due date and time if needed
- Choose a priority level
- Select a category
- Tap "Save" to create your task

### Navigating the App

- Tasks View: View all your tasks organized by category
- Calendar View: See tasks grouped by due date
- Lists View: Manage list-type items and shopping lists
- Use the search icon to find tasks quickly
- Use filters (All, Pending, Overdue, Completed) to view tasks in different stages of completion.

---

## Local Mode & Cloud Sync

Simply Taskful offers two ways to use the app: Local Mode (no account required) and Cloud Mode (with account for syncing across devices).

### Local Mode

- Use the app without creating an account
- Tap "Continue without Account" on the login screen
- All your tasks, categories, and data are stored locally on your device
- Your data is private and never leaves your device
- Perfect for users who want to use the app without cloud sync
- All core features work in local mode (tasks, categories, notifications, calendar import, etc.)

### Cloud Mode

- Sign in or create an account to enable cloud sync
- Your data is synced across all your devices
- Access your tasks from any device where you're signed in
- Enables list sharing with other users
- Your data is securely stored in the cloud
- Automatic backups ensure your data is safe

### Switching Between Modes

- You can switch from local mode to cloud mode at any time by signing in
- When you sign in, your local data will be automatically migrated to the cloud
- You can exit cloud mode by signing out, but your cloud data will remain
- If you sign back in later, your cloud data will be restored
- Local mode data and cloud data are kept separate until you sign in

### Features by Mode

**Local Mode Features:**
- Create, edit, and delete tasks
- Manage categories
- Set up notifications and reminders
- Import calendar events
- Use keyword filtering
- View completion stats
- Use widgets and Siri shortcuts
- Archive and manage tasks

**Cloud Mode Features (includes all Local Mode features plus):**
- Sync data across devices
- Share lists with other users
- Access pending invitations
- Automatic cloud backups

### Data Storage

- **Local Mode:** Data is stored on your device using iOS UserDefaults
- **Cloud Mode:** Data is stored securely in Firebase Firestore
- When you sign in, local-only data is automatically copied to the cloud
- Your local data remains on your device even after signing in
- You can see your current mode in the Profile Menu (tap your profile icon)

---

## Task Management

### Viewing Task Details

- Tap anywhere on a task card to view full details
- The details screen shows all task information including priority, due date, category, repeat settings, and description
- Links in descriptions are automatically detected and made clickable
- If a task description contains a link, a "Site Preview" section will show a preview of the linked website with thumbnail and title

### Completing Tasks

- Tap the circle icon on any task card to mark it as complete
- Completed tasks show a checkmark and are struck through
- Repeating tasks will automatically create a new instance based on your repeat settings

### Editing Tasks

- Long press on any task card to open the action menu
- Select "Edit" from the menu
- Make your changes and tap "Save"
- You can also tap on a task card to view full details, then tap the edit icon in the top right

### Deleting Tasks

- Long press on a task card and select "Delete"
- A confirmation dialog will appear asking you to confirm the deletion
- Deleting a task permanently removes it from your account
- This action cannot be undone

### Marking Tasks as Did Not Complete

- Long press on a task card and select "Did Not Complete"
- Confirm the prompt to mark the task as not completed
- The current task will be archived and removed from your active list
- If the task is repeating, the next scheduled occurrence will be created automatically

---

## Categories

Categories help you organize your tasks. You can create task categories or list categories for different types of items.

### Creating Categories

- Go to Settings → Manage Categories
- Tap "Add Category"
- Enter a category name
- Choose whether it's a task category or a list category
- Categories with tasks cannot be deleted until all tasks are removed or reassigned

### Task Categories vs List Categories

- Task Categories: Used for regular tasks and items
- List Categories: Used for shopping lists and other list-type items
- The Lists View shows tasks from list categories
- Use categories consistently to keep your tasks organized

---

## List Sharing

Share your categories with others to collaborate on tasks. Categories are shared through an invitation system that requires approval from the invited user. **Note: List sharing requires cloud mode (sign in with an account).**

### Sharing a List (Owner)

- Go to Settings → Manage Categories
- Long press on a category
- Select "Share" from the menu
- Enter the email address of the person you want to share with
- Tap "Add" to send an invitation
- The invitation will appear in your "Pending Invitations" section
- You'll receive a notification when the invitation is accepted or declined
- Shared lists show a blue badge for owners

### Pending Invitations

- Pending invitations appear at the top of the Manage Categories screen
- Owners can see invitations they've sent and cancel them if needed
- Invited users can see invitations they've received
- The invitation count badge shows the number of pending invitations

### Accepting an Invitation (Collaborator)

- You'll receive a notification when someone invites you to a list
- Go to Settings → Manage Categories
- Tap "Pending Invitations" if you have pending invitations
- Review the invitation details (list name, owner name, owner email)
- Tap "Accept" to join the list or "Decline" to reject the invitation
- Once accepted, the list appears in your views immediately
- The owner will be notified when you accept or decline

### As a Collaborator

- After accepting an invitation, shared lists automatically appear in your views
- Shared lists show a green badge to indicate you're a collaborator
- You can add, edit, and delete tasks in shared lists
- All changes sync in real-time with all collaborators
- Tasks from shared lists appear in Lists View

### Collaborator Permissions

- Can add tasks to the shared list
- Can edit any task in the shared list
- Can delete any task in the shared list
- Can complete and archive tasks
- Can receive notifications for tasks in the shared list
- Cannot edit the list name or settings
- Cannot delete the list itself
- Cannot share the list with others

### Leaving a Shared List

- Go to Settings → Manage Categories
- Long press on a shared list where you're a collaborator
- Select "Leave List" from the menu
- Confirm that you want to leave
- The list will disappear from your view immediately
- You can be added back by the owner at any time

### Managing Collaborators (Owner)

- Go to Settings → Manage Categories
- Long press on your shared list and select "Share"
- View all current collaborators in the Share List screen
- View pending invitations you've sent
- Cancel pending invitations if needed
- Remove collaborators by tapping the delete icon next to their name
- A confirmation dialog will appear before removing a collaborator
- Add new collaborators by searching for their email and sending an invitation

### Important Notes

- Sharing uses an invitation system - users must accept invitations to join
- Invitations can be cancelled by the owner before they're accepted
- Only list categories can be shared - task categories remain private
- Shared lists appear in Lists View, not Tasks View or Calendar View
- All changes are synced in real-time
- If you reinstall the app, your shared lists will automatically reappear when you log in
- Both owners and collaborators receive notifications for tasks in shared lists
- Owners receive notifications when invitations are accepted or declined

---

## Notifications & Reminders

### Task Reminders

- Tasks with due dates automatically receive reminder notifications
- Notifications are sent at the due date/time
- Tasks without a specific time use your All Day Task Notification time preference (defaults to 8:00 AM)
- You can set an "Early Reminder" to be notified minutes before the due date
- Custom notification sounds are available in settings

### All Day Task Notifications

- Go to Settings → Notification Settings → All Day Task Notifications
- Choose what time all-day reminders should be delivered when "Use Time" is off
- Applies to tasks you create/edit and calendar events imported as all-day events
- Changing this setting updates future reminders automatically

### Daily Summaries

- Enable daily summaries in Notification Settings
- Set your preferred time to receive a summary
- Daily summaries include tasks due today and past due tasks in a single notification
- The notification message will show:
  - "You have X tasks due today!" (if only tasks due today)
  - "You have X tasks due today and Y tasks past due!" (if both)
  - "You have X tasks past due!" (if only past due tasks)
- Summaries are automatically updated based on your active tasks
- Use the "Test" button in Notification Settings to send a test daily summary notification

### Notification Settings

- Go to Settings → Notification Settings
- Enable/disable custom sounds
- Configure the All Day Task Notifications time for tasks without a due-time
- Configure daily summary time
- Use the "Test" button to send a test daily summary notification
- Manage notification permissions
- Use "Clear & Rebuild Notifications" if reminders aren't working properly

---

## Repeating Tasks

Create tasks that automatically repeat on a schedule. When you complete a repeating task, a new instance is created based on your repeat settings.

### Repeat Options

- Daily: Task repeats every day
- Weekly: Choose specific days of the week
- Monthly: Repeat on a specific day of each month, or a specific weekday (e.g., "1st Monday")
- Yearly: Task repeats once per year on the same date

### How It Works

- When you mark a repeating task as complete, a new task is automatically created
- The new task uses the next occurrence date based on your repeat pattern
- All task details (priority, category, early reminders) are preserved
- The due date time is preserved for tasks with times

---

## Views & Filters

### Calendar View

- View tasks organized by due date
- Only tasks with due dates are shown
- Tasks are grouped by date instead of category
- Tap a date header to expand/collapse that date's tasks
- Long press a date header to access "Expand All" or "Collapse All" options
- Your collapsed/expanded state is remembered even after closing the app
- Perfect for seeing what's due on specific days

### Tasks View

- View tasks from non-list categories organized by category
- Tasks are grouped into collapsed sections by category
- Tasks from list categories are not shown here (see Lists View)
- Tap a category header to expand/collapse
- Long press a category header to access "Expand All" or "Collapse All" options
- Your collapsed/expanded state is remembered even after closing the app
- Use filters to show All, Pending, Overdue, or Completed tasks
- Search for tasks using the search icon

### Lists View

- View tasks from list categories (like shopping lists)
- Organized by category
- Tap a category header to expand/collapse
- Long press a category header to access "Expand All" or "Collapse All" options
- Your collapsed/expanded state is remembered even after closing the app
- Use for managing items that aren't traditional tasks

### Search & Filters

- Tap the search icon to search for tasks by title
- Use filter tabs to view:
  - All: Show all tasks
  - Pending: Tasks that aren't completed
  - Overdue: Completed tasks that are past due
  - Completed: All completed tasks

---

## Widgets & Shortcuts

### Home Screen Widget

- Add the Simply Taskful widget to your home screen
- Widget shows your upcoming tasks
- Past-due tasks are displayed in red
- Tap the plus icon to quickly add a new task
- Widget shows task count in the top right

### Siri Shortcuts

- Use Siri Shortcuts to add tasks and list items
- Shortcuts can access your categories for quick task creation
- Create custom shortcuts for frequently used actions
- Access shortcuts from the Shortcuts app or by asking Siri

---

## Useful Tools

### Siri Shortcuts

- Access pre-made Siri Shortcuts to quickly add tasks, list items, and shopping items
- Shortcuts integrate with your categories for seamless task creation
- Tap a shortcut link to add it to your Shortcuts app
- Use shortcuts from the Shortcuts app or by asking Siri
- **Works in both local mode and cloud mode**

### Import iOS Calendar Events

- Automatically import new or updated iOS calendar events as tasks
- Only new events or events that have been modified will be imported
- Enable the "Enable Import" toggle to start monitoring for calendar events
- The toggle is disabled if calendar access is not granted in iOS Settings
- Use "View iOS settings" link to manage calendar permissions
- Imported events are automatically assigned to the "General" category
- Events are only imported once per occurrence (prevents duplicates for recurring events)
- If a calendar event is deleted from your iOS calendar, the corresponding task will also be deleted from the app
- Import history is stored locally in local mode, and synced to the cloud in cloud mode
- **Works in both local mode and cloud mode**

### Keyword Filtering

- Add keywords to filter out calendar events before they're imported as tasks
- Events containing these keywords in their title or notes will not be imported
- Keywords are matched as exact phrases (e.g., "team meeting" matches "team meeting" but not "team" or "meeting" individually)
- Matching is case-insensitive
- Add, edit, or delete keywords using the "Keyword Filtering" button
- Use this to prevent importing events you don't want as tasks (e.g., "block out", "busy", etc.)
- **Works in both local mode and cloud mode**

### Import History & Cleanup

- The app tracks all imported calendar events to prevent duplicates
- The import history count shows how many events are currently tracked
- Use "Clean Import History" to remove orphaned entries (events that no longer exist in your calendar or tasks that were deleted)
- The cleanup process also removes stale processing entries and adds missing event titles to history entries
- Import history is stored locally in local mode, and synced between devices in cloud mode
- The cleanup process shows a progress indicator while running
- **Works in both local mode and cloud mode**

### Share Lists

- Share your list categories with other users for collaboration
- **Requires cloud mode (sign in with an account)**
- See the "List Sharing" section for detailed instructions
- **Not available in local mode**

### Pending Invitations

- View and manage invitations to shared lists
- **Requires cloud mode (sign in with an account)**
- See the "List Sharing" section for detailed instructions
- **Not available in local mode**

### Manage Tasks

- Archive all completed tasks to hide them from your main task list
- Archived tasks can be restored later
- Use "View Archived Tasks" to see and manage archived items
- Unarchive tasks if you need to access them again
- Permanently delete all archived tasks if you no longer need them
- Deleting archived tasks cannot be undone
- A confirmation dialog will appear before deletion
- **Works in both local mode and cloud mode**

### Clear & Rebuild Notifications

- Removes all pending task reminders and re-creates them for current active tasks
- Refreshes Daily Summary notifications if configured
- Useful if notifications aren't working properly or if you've made many changes
- This helps ensure all your tasks with due dates have proper reminders
- **Works in both local mode and cloud mode**

---

## Completion Stats

Track your productivity with completion statistics. View your task completion rates and see how you're performing over time.

### Overview Cards

- Total Tasks: Count of all tasks that have both a due date and due time (`Use Time` enabled). Includes archived tasks.
- Active Tasks: Tasks with a due date/time that are still open (not completed) and not archived.
- Past Due: Open, unarchived tasks whose due date/time has already passed.
- Completed On-Time: Percentage of completed tasks whose completion date is on or before the due date. Includes archived tasks.
- Completed Late: Percentage of completed tasks whose completion date is after the due date. Includes archived tasks.
- Never Completed: Number of archived tasks that were never completed. Tap this card to jump straight to the Archived Tasks view.

> **Note:** All statistics only include tasks where the due date has `Use Time` enabled.

### Daily Breakdown

The Daily Breakdown shows a 7-day window (today plus the previous 6 days) with completion statistics for each day.

For each day, the stats show:
- Total: Number of tasks that have a due date on that specific day
- Completed: Number of those tasks that were completed (either on that day or before)
- Completion Rate: Percentage of tasks completed out of total tasks due on that day

For example, if 10 tasks are due on Monday and 7 of them were completed (on Monday or earlier), it will show: Total: 10, Completed: 7, Completion Rate: 70%

### Navigation

- Use "Prev 7 Days" to view earlier 7-day periods
- Use "Next 7 Days" to move forward (only available when viewing past periods)
- The date range is displayed at the top of the Daily Breakdown section
- Today is always shown at the top of the list when viewing the current 7-day period

### Important Notes

- Only tasks with due dates and due times are included in the statistics
- Tasks without due dates or without due times are not counted
- If a task is completed early, it still counts toward the due day's completion rate
- The completion rate is calculated based on tasks that were due on that day, not tasks completed on that day

---

## Tips & Tricks

### Organization

- Use consistent category names for better organization
- Set priorities to focus on important tasks first
- Archive completed tasks regularly to keep your views clean
- Use the Tasks and Lists reorder tools to arrange categories in the order that works best for you

### Productivity

- Set due dates for time-sensitive tasks
- Use early reminders for tasks that need advance notice
- Enable daily summaries to plan your day
- Use repeating tasks for routine items to save time

### Quick Actions

- Long press any task for quick access to Edit, Delete, or mark as Did Not Complete. The Did Not Complete option archives the current task and, if it repeats, creates the next occurrence automatically.
- Tap a task card to view full details
- Use the widget to quickly add tasks without opening the app
- Search for tasks when you have many items
- Long press on the bottom menu (Calendar, Tasks, Lists, Settings) to reorder menu options
- Customize your menu order by dragging options in the reorder screen
- Your menu order is saved and persists across app restarts

---

## App Support & Feedback

For any questions or feedback regarding Simply Taskful please contact [dskinner@lightshiftdesigns.com](mailto:dskinner@lightshiftdesigns.com).

