# Front office Positions

* Front office Positions
  * [Moving a module within a hook](front-office-positions.md#FrontofficePositions-Movingamodulewithinahook)
  * [Attaching a module to a hook: Transplanting](front-office-positions.md#FrontofficePositions-Attachingamoduletoahook:Transplanting)
  * [Editing an attached module](front-office-positions.md#FrontofficePositions-Editinganattachedmodule)
  * [Removing a module from a hook](front-office-positions.md#FrontofficePositions-Removingamodulefromahook)
  * [Moving a module visually: Live Edit](front-office-positions.md#FrontofficePositions-Movingamodulevisually:LiveEdit)
    * [Where to move modules?](front-office-positions.md#FrontofficePositions-Wheretomovemodules?)
  * [Transplanting a module by modifying its code](front-office-positions.md#FrontofficePositions-Transplantingamodulebymodifyingitscode)

A modules can have to views: one on the back office (its options, or even a configuration screen), and one on the front office. The front office view is how and where the module is displayed within your shop's theme.

The position of a module in your theme can be changed, because you might want one module's block to be placed much higher (or lower) in the page that others. In PrestaShop's parlance, this is called "transplanting", and is done using the tool available in the "Positions" page, under the "Modules" menu. In effect, this enables you to attach a module to one of the many available hooks in the current theme, without writing any code.

The "Positions" page displays all the available hooks, and their attached modules. Many are empty by default, but some of the most useful ones have a dozen of modules (the displayHeader hook has 33 modules by default).

![](<../../../.gitbook/assets/23789645 (1).png>)

At the top of the page, a drop-down menu enables you to only display the hook in which you are interested.\
&#x20;By default, this page only displays the hooks on which you can position functions. Checking the "Display non-positionable hooks" box below displays all the hooks, even those where you cannot position something.

The header of the table for each hook displays the hook's name, its technical name (and for some, a quick description), and its number of attached modules. The table lists the modules that are attached to that hook.

The modules are displayed in the order in which they appear in the hook.

## Moving a module within a hook <a href="#frontofficepositions-movingamodulewithinahook" id="frontofficepositions-movingamodulewithinahook"></a>

You have two ways of changing a module's position within a hook:

* Click the up or down arrow. The page will reload and display the new order.
* Drag and drop the module's row itself:
  1. Place the mouse cursor on the position number to have it change into a "move item" cursor.
  2. Click and hold while moving the cursor over the row/position where you want the module to be: the module's row changes position accordingly.
  3. Release the mouse button: the current position for the module is saved.

For most modules, transplantation can easily be done directly via the back office. Some modules require you to alter their code in order to transplant them.

## Attaching a module to a hook: Transplanting <a href="#frontofficepositions-attachingamoduletoahook-transplanting" id="frontofficepositions-attachingamoduletoahook-transplanting"></a>

In PrestaShop, "transplanting" is the action of attaching a module to a hook. You can add a module to more than one hook.

Two things to know before transplanting a module:

* Some modules are written to only be attached to a given set of hooks.
* Some hooks are written to not accept some specific kinds of modules.

Therefore, be aware that you cannot always transplant any module to any hook.

Make sure to disable the cache when testing the effect of a new module on the front-end. You can do this in the "Preferences" page, under the "Advanced parameters" menu.

The transplanting process has its own interface:

1. Go to the "Modules" menu, and its "Positions" page.
2. Click the "Transplant a module" button at the top right. The transplanting interface appears.
3. In the "Module" drop-down list, select the module you want to transplant.
4. In the "Hook into" drop-down list, select where you want to transplant the module to. There are many available hooks. You can change your setting later if needed.
5. In the "Exceptions" field, type the name of the file(s) of the pages in which you do not want the module to appear.\
   You can perform a multiple selection simply by clicking on the file names while keeping the Ctrl key pressed. You can deselect files in the same manner: Ctrl+click.
6. Do not forget to save your changes.

![](<../../../.gitbook/assets/23789646 (1).png>)

The "Hook into" drop-down menu gives you a good idea where module can be placed.

Even though the "Hook into" drop-down list gives a comprehensive overview of the available hooks, it might not always be clear which is the one to which you want to attach your module. Do not hesitate to try another hook if the result of your selection if not what you expect.\
&#x20;The list gives some detail: some hook have a description after the hook's name, for instance "Add fields to the form 'attribute value'" for `displayAttributeForm`. Peruse them all in order to choose your hook correctly.

## Editing an attached module <a href="#frontofficepositions-editinganattachedmodule" id="frontofficepositions-editinganattachedmodule"></a>

Each module has two icons on the right side of its row: one to edit its settings, the other to delete the module.

Editing a module's setting uses the same interface as the one used for the transplanting a module. The major difference is that you cannot change the "Module" and "Hook into" settings, as they are disabled, and thus grayed out. You can only edit the exception setting, which works just as described in the "Attaching a module to a hook" method above.\
&#x20;While you cannot edit the "Module" and "Hook into" settings, they can serve as a handy reminder of their current position, should you want to put them back there later on.

![](<../../../.gitbook/assets/23789649 (1).png>)

If you want to move a module to another hook, you must use the transplanting interface:

1. Click the "Transplant a module" button at the top right. The transplanting interface appears.
2. In the "Module" drop-down list, select the module you want to move to another hook.
3. In the "Hook into" drop-down list, select where you want to transplant the module to.
4. In the "Exceptions" field, type the name of the file(s) of the pages in which you do not want the module to appear.
5. Save your changes. The hook list appears.
6. Go to the hook where you have transplanted the module: it should appear in there. Change its position if necessary.
7. Go to the hook where the module first was, and click the trashcan icon in order to remove it from that hook. This prevents you from having the same module appear twice.

Always check your front-office to make sure the module is indeed where you intended it to be.

## Removing a module from a hook <a href="#frontofficepositions-removingamodulefromahook" id="frontofficepositions-removingamodulefromahook"></a>

There are two ways to remove a module from a hook:

* Removing a single module: click the trashcan icon on the right of the module's row.
* Removing a batch of modules: select the modules by checking the box on the right of their row, and then click the "Unhook" button, found at the top and the bottom of the list of hooks.

## Moving a module visually: Live Edit <a href="#frontofficepositions-movingamodulevisually-liveedit" id="frontofficepositions-movingamodulevisually-liveedit"></a>

Another way to move modules around on the shop's homepage is the Live Edit mode, which embeds said homepage into a tool that lets you visually decide where to place your modules. You can access it from the "Position" page, by clicking the "Run Live Edit" button.

![](<../../../.gitbook/assets/23789650 (1).png>)

When clicked, PrestaShop opens the homepage in a new browser windows/tab, with the Live Edit script on top:

* All module blocks have a dotted red border, enabling you to see which blocks you can move.
* At their top left side, a block-specific icon appears, along with the block's name, enabling you to always find your way among blocks.
* At their top right side, they have two icons:
  1. A "move" icon: click on it to start moving the module around.
  2. A "trash" icon: click it to remove the block from the home.

![](<../../../.gitbook/assets/23789653 (1).png>)

At the top of the Live Edit mode, a toolbar presents you with two buttons: "Close Live Edit" and "Save".

The first one is quite self-explanatory; the second one cancels all changes you might have made to your modules' position during this live-editing session.

Once you have removed a module, if you want to bring it back, you will have to go to the "Positions" page and use the "Transplant a module" form.

### Where to move modules? <a href="#frontofficepositions-wheretomovemodules" id="frontofficepositions-wheretomovemodules"></a>

Modules cannot be moved just about anywhere: it depends on both the theme's hooks, and each module's hook support (as seen in the above section). Therefore, you mostly can only move modules within their understood context: column modules can be moved within a column as well as from one column to the other (right to left, for instance), while regular homepage modules (the ones at the center) can only be moved within their specific column.

In order to give you a visual hint about where a given module can be moved, it will display an empty green block if the location is correct, and an empty red block if not.

## Transplanting a module by modifying its code <a href="#frontofficepositions-transplantingamodulebymodifyingitscode" id="frontofficepositions-transplantingamodulebymodifyingitscode"></a>

This is for experts only: you must have a good knowledge of PHP and HTML before attempting anything with the code of a module.

Some modules cannot be transplanted into other sections of the front-office simply because they lack the necessary code.

For example, the "Quick Search" block (`/blocksearch`) contains templates for both column display and header display, whereas the "Currencies" block (`/blockcurrencies`) only has one template file which only works with the header section. Likewise, the default "Featured Products" block (`/homefeatured`) can only be placed in the center content section of the main page.

If you want to display simple modules such as the "Currencies" block in a position for which it was not built, you will have to edit its template files.\
&#x20;More complex module, such as the "Featured" block, can also be made to be displayed in other sections of the page, but they might have to be partly rewritten in order to have their design work with that new location.

To customize the transplantation ability of a module, you must give it the correct PHP function for the new target hook. For example, the "Currency" block has this function:

```
function hookTop($params)
  {
  ...
  }
```

In order to transplant the "Currency" block into the right column, for instance, you need to add the `hookRightColumn()` function:

```
function hookRightColumn($params)
  {
  ...
  }
```

Afterwards, you must write the code that displays the content on the front page. At best, that means copy/pasting the content of the `hookTop()` function; at worst, you need to rework the content of `hookTop()` function into something that will work for the new location.
