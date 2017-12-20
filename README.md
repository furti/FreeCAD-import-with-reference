# Import with reference

The macro lets you import parts or bodies from another FreeCAD document. As it works on parts and bodies it is 0.17 only. The reference to the original object and file will be stored inside the clone. So you can also use the same macro to refresh a object when you made changes to the original one.

## Importing objects

When you execute the macro without any objects selected a file selection dialog will show up. Select the FreeCAD file you want to import a object from and hit "Open".

A dialog will be shown in the Task panel.

![Dialog](Dialog.png?raw=true)

1. Here you can select the part or body to import.
2. If you check "At origin", the part will be imported at the origin idependent from the placement in the original file.
3. IF you check "Import relative" the location to the file will be stored relative to the active document. So if the file you want to import from is in the same folder as your active document, the reference will be still intact when you move the whole folder to another location.

## Reloading objects

To reload a object simply select it in the tree view and execute the macro. If the object was currently imported by this macro it will be updated. The newly imported object will be placed at the same location as the previous one. The old object will be removed after the new one is ready.

## License
The macro is available under the MIT License.