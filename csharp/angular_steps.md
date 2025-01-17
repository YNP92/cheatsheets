Steps for creating an angular app with bash shell and VS Code.

## 1. Create the app and open VS Code

From bash shell, go to your dev folder and type the following (but replace "myapp" with the name of your app):

```bash
ng new myapp
cd myapp
code .
```

## 2. Clean out app.component.html
Open app.component.html
1. Select everything
2. Delete what's in it.
3. Save it.

## 3. Launch a couple terminals
Launch a terminal from within VS Code by clicking **Terminal -> New Terminal**. *(Tip: You might want to make at least two terminals, one for the server, one for your ng commands.)*

## 4. Add FormsModule if it isn't already there

You will probably need to add the FormsModule to app.module.ts. To do so:

1. expand src -> app, and open app.module.ts.
2. In the "imports" section, add a comma to BrowserModule, and on the next line add FormsModule. Get the casing right. (Type only part of it, and press Tab, and the import statement will get added automatically.)
3. Save this file and close it.

## 5. Start the server
Launch the server in the terminal by typing

```
ng serve -o
```

**Error?** If you see an error about port in use, you probably have another angular app running. Go find that angular app's terminal, and stop the server by pressing Ctrl+C.

## Other Stuff

When you want to create an interface, **make sure you're in the angular application's main folder** and type the following (but replace "pet" with the name of your interface):
```bash
ng generate interface pet
```

When you want to create a component, **make sure you're in the angular application's main folder** and type the following (but replace "show-pet" with the name of your component):
```bash
ng generate component show-pet
```

