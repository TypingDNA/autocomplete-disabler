# Autocomplete Disabler
Disable **autocomplete** and **autofill** (in *some* browsers), and disable **copy**, **cut**, and **paste** from the target inputs.


## Usage

Firstly you need to include the `autocomplete-disabler.js` script in your project and import it in the page with the inputs you want to use it on. If you want to use the typing pattern visualizer, you also need to include and import the `typing-visualizer.js` script.

**AutocompleteDisabler class**


1. Create a new instance of the `AutocompleteDisabler` class:

    var autocompleteDisabler = new AutocompleteDisabler({ showTypingVisualizer: true, showTDNALogo: true });

The options are:

- `showTypingVisualizer` - (default ***false***) indicates if the **TypingDNA** typing pattern visualizer will appear. 
- `showTDNALogo` - (default ***true***) indicates that if the visualizer will appear then the **TypingDNA** logo will be displayed alongside the typing pattern visualization.

The `AutocompleteDisabler` will target all the inputs with the `.disable-autocomplete` class. For example:

    <input id="password" class="disable-autocomplete" autocomplete="password" type="password" name="password" placeholder="" value="" />


2. To disable **autocomplete** call the `.disableAutocomplete()` method:

    autocompleteDisabler.disableAutocomplete();


3. To disable **copy**, **cut**, and **paste** call `disableCopyPaste()`:

    autocompleteDisabler.disableCopyPaste();

## License
Apache License, [Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)
