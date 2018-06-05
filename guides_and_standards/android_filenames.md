## 1.1 Most important rule

No shortend words anywhere unless otherwise specified - e.g. no btn, attr, ic, or anything else. Use full word all the time everywhere.

## 1.2 File naming

### 1.2.1 Class files'
Class names are written in [UpperCamelCase](http://en.wikipedia.org/wiki/CamelCase).

For classes that extend an Android component, the name of the class should end with the name of the component; for example: `SignInActivity`, `SignInFragment`, `ImageUploaderService`, `ChangePasswordDialog`.

### 1.2.2 Resources files

Resources file names are written in __lowercase_underscore__.

#### 1.2.2.1 Drawable files

Naming conventions for drawables:


| Asset Type   | Prefix            |		Example               |
|--------------| ------------------|-----------------------------|
| Action bar   | `actionbar_`             | `actionbar_stacked.9.png`          |
| Button       | `button_`	            | `button_send_pressed.9.png`    |
| Dialog       | `dialog_`         | `dialog_top.9.png`          |
| Divider      | `divider_`        | `divider_horizontal.9.png`  |
| Icon         | `icon_`	            | `icon_star.png`               |
| Menu         | `menu_	`           | `menu_submenu_bg.9.png`     |
| Notification | `notification_`	| `notification_bg.9.png`     |
| Tabs         | `tab_`            | `tab_pressed.9.png`         |

Naming conventions for icons:

| Asset Type                      | Prefix             | Example                      |
| --------------------------------| ----------------   | ---------------------------- |
| Icons                           | `icon_`              | `icon_star.png`                |
| Launcher icons                  | `icon_launcher`      | `icon_launcher_calendar.png`   |
| Menu icons and Action Bar icons | `icon_menu`          | `icon_menu_archive.png`        |
| Status bar icons                | `icon_status_notify`   | `icon_status_notify_msg.png`     |
| Tab icons                       | `icon_tab`           | `icon_tab_recent.png`          |
| Dialog icons                    | `icon_dialog`        | `icon_dialog_info.png`         |

Naming conventions for selector states:

| State	       | Suffix          | Example                     |
|--------------|-----------------|-----------------------------|
| Normal       | `_normal`       | `button_order_normal.9.png`    |
| Pressed      | `_pressed`      | `button_order_pressed.9.png`   |
| Focused      | `_focused`      | `button_order_focused.9.png`   |
| Disabled     | `_disabled`     | `button_order_disabled.9.png`  |
| Selected     | `_selected`     | `button_order_selected.9.png`  |


#### 1.2.2.2 Layout files

Layout files should match the name of the Android components that they are intended for but moving the top level component name to the beginning. For example, if we are creating a layout for the `SignInActivity`, the name of the layout file should be `activity_sign_in.xml`.

| Component        | Class Name             | Layout Name                   |
| ---------------- | ---------------------- | ----------------------------- |
| Activity         | `UserProfileActivity`  | `activity_user_profile.xml`   |
| Fragment         | `SignUpFragment`       | `fragment_sign_up.xml`        |
| Dialog           | `ChangePasswordDialog` | `dialog_change_password.xml`  |
| AdapterView item | ---                    | `item_person.xml`             |
| Partial layout   | ---                    | `partial_status_bar.xml`       |

A slightly different case is when we are creating a layout that is going to be inflated by an `Adapter`, e.g to populate a `ListView`. In this case, the name of the layout should start with `item_`.

Note that there are cases where these rules will not be possible to apply. For example, when creating layout files that are intended to be part of other layouts. In this case you should use the prefix `partial_`.

#### 1.2.2.3 Menu files

Similar to layout files, menu files should match the name of the component. For example, if we are defining a menu file that is going to be used in the `UserActivity`, then the name of the file should be `activity_user.xml`

A good practice is to not include the word `menu` as part of the name because these files are already located in the `menu` directory.

#### 1.2.2.4 Values files

Resource files in the values folder should be __plural__, e.g. `strings.xml`, `styles.xml`, `colors.xml`, `dimensions.xml`, `attributes.xml`

# Attribution

This was taken from Ribot Ltd's Android Project and Code Guidlines document. 
https://github.com/ribot/android-guidelines/blob/master/project_and_code_guidelines.md
