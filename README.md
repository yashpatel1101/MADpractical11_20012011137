# MADpractical11_20012011137

AIM: Create Note Android Application that can add Note, edit Note, delete Note, and set reminder date & time of note. By using Broadcast Receiver, AlarmManager set reminder of note. By using SQLite, store all notes data.

Create two Activities like MainActivity, NoteViewActivity according to below UI design.

Use RecyclerView Code from Practical-9 to display Note Data.

Use Broadcast Receiver, Time Picker Dialog, service & AlarmManager code from Practical-7

Create Note class with member variables like id, title, subTitle, Description, modifiedTime, reminderTime:Long, isReminderEnable:Boolean & create membor methods like getCurrentDateTime(), getMillis(), setReminder(), isValid(), getReminderText(), saveNote(), getHour(), getMinute(), calculateReminder()

Create DatabaseHelper Class for SQlite with member methods like insertNote(), getNote(id), getAllNotes(), getNotesCount(), updateNote(), deleteNote().

Use Databinding in gradle file to easy way integrate xml into kotlin file

Use Material 3 design for UI

create class NotesData with companion object and it will store column name of table and create table query.

Create NoteViewActivity. It will show while reminder notification is turned up and user click on notification. It will also show when click on Note in recyclerView. After clicking on notification NoteViewActivity should be open with full description of that note.

Note should be deleted by clicking on icon of Delete. Note should not be added if any one field of note is empty.

Some notes have reminder time so add reminder time in alarmManager with note id & it should be receive in broadcast receiver & in broadcast receiver notification should be generated with title & description of note.

If More than one notes have reminder time then notification should be displayed for each note separately.

Create Common Custom Dialog Box for add, edit note.

Create RecyclerView & its adapter to display all notes.

![Screenshot_20221119_135924](https://user-images.githubusercontent.com/110656617/202842236-b5b24505-53f9-44c3-9cf4-005bfa88019c.png)

![Screenshot_20221119_135630](https://user-images.githubusercontent.com/110656617/202842242-64626cdc-11af-4a3c-81d6-41a462913f2d.png)

![Screenshot_20221119_135709](https://user-images.githubusercontent.com/110656617/202842244-880f6eae-f5af-4f0f-846d-144388d5ca5b.png)

