# Overriding-Boomi-s-default-time-zone

The time zone for schedules and default time zone is based on where molecule or atom is installed.
In order to override the boomi's default time zone we need to add a addition advanced account property as for eg :" **Default Time Zone for Account Schedules** : CST "

![image](https://user-images.githubusercontent.com/97012694/148570409-d80c65c5-6f86-4282-b55b-9097f660f23d.png)

Infact There are some others ways by which we can change the time zones

**Change via server**

The timezone is reflective of the system clock of the server the atom is installed on. If you change the server's timezone then it will be reflected in the atom after restarting the atom.

**Change via atom**

If you cannot change the server clock, you can do it with the atom properties.

- On the local atom go to the <<atom_installation_directory>>\bin directory
- Edit the atom.vmoptions file
- Add this statement to set the timezone for the atom, in this example the Chicago timezone ID is used-
-   "-Duser.timezone=America/Chicago" 
-  Restart the atom

All available Java 8 timezone IDs and UTC offset information can be found in the attached file, Time_Zone_ID.csv or other sources .

Please refer to the attachment for all time zones
