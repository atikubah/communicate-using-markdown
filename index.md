### Projects I want to work on
- [ ] Music streaming App
- [ ] Real Estate P2P app
- [ ] Logistics App
- [x] Notekeeper App

![baby groot and octobot](https://user-images.githubusercontent.com/36367844/232263661-b7fe1c1a-ef88-40af-a01e-ede696cb4936.jpg)

# `Here is some sample code from my Notekeeper App`

```
val adapterCourses = ArrayAdapter<CourseInfo>(this,
                android.R.layout.simple_spinner_item,
                DataManager.courses.values.toList())
        adapterCourses.setDropDownViewResource(android.R.layout.simple_spinner_dropdown_item)
        spinnerCourses.adapter = adapterCourses

        notePosition = savedInstanceState?.getInt(NOTE_POSITION, POSITION_NOT_SET) ?:
            intent.getIntExtra(NOTE_POSITION,POSITION_NOT_SET)

        if (notePosition != POSITION_NOT_SET)
            displayNote()
        else{
            DataManager.notes.add(NoteInfo())
            notePosition = DataManager.notes.lastIndex
        }
 ```
