# Menu Package

This is a package for printing and getting user input for menus. It is written in Go.

The package contains two files: `constants.go`, which contains constants and `menu.go`, which contains the package's functions.

## Functions included in the package

- PrintMenu

  - `PrintMenu` prints out menu options. The function's `menu` parameter must be of type `map[string]string` but the function will always print items in the same numerical order. The `showNumber` parameter can be set to true or false to set whether or not menu options are printed with numbers.

- GetUserInput

  - `GetUserInput` gets the user's input and sanitizes it. The function returns the user input without leading or trailing whitespace.

- GetMenuSelection

  - `GetMenuSelection` checks if the user's input matches an option in the menu and calls `GetUserInput` again if it does not. The function returns the value corresponding to the key that matches the user input in the menu map.
