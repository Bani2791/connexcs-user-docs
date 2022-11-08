## Introduction

Using Page Builder, you can customise the Control Panel, Customer Portal, and Web Phone. Pages help you enhance the functionality of these interfaces. 

You can add Pages to multiple areas of these interfaces, such as Carrier, Customers, and Rate cards. 

A page can be interactive, containing forms that can be completed and then processed by ScriptForge.

!!! note "**Pages work together with [Button Builder](https://docs.connexcs.com/developers/button-builder/) to display a page on any Navigation bars.**"
    
The **Elements** in the Pages are extremely powerful and increase flexibility for the features you want to include in your portal.

### Usage Cases

1. You can use Pages to redirect to any rulebook or manuals that you want to show your customers.  
2. Interaction with external links using [**Scriptforge**](https://docs.connexcs.com/developers/scriptforge/) and integration with Pages. 
3. You can use it to create interactive content. For example, getting input from the customers.  
4. Server-side and client-side validation.  
5. If you are using **Webphone**, the data can be collected in the form created in Pages.
6. Customers may create their payment processors. They can create their interface using Pages on the website. The integration of the processing system can be done using Scriptforge.  
7. Number Porting: You can create a form (using Pages) on the Customer Portal and ask for details. Once the form is submitted, the requests reach Scriptforge for validation purposes. Scriptforge can update the customer on the status of their processed request.

## Build Form
1. Navigate to Developer :material-menu-right: Scriptforge IDE :material-menu-right: Pages and click <img src="/pages/add.png" alt="add" width="60"/> to create a new form.<img src="/pages/pages-page.png" alt="pages-page" width="5000"/>
2. Complete the form's **Name** and **Title** fields, then click **Save**. <img src="/pages/name-and-title.png" alt="name-and-title" width="450"/>
3. When you see the screen with the various pages, click on the form you created (Bani in this case).
4. A screen with options such as [**Basic Field**](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/), [**Advance Field**](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/), [**Layout**](https://bani--connexcs-docs.netlify.app/developers/pages/layout/), **Component Attribute**, and [**Form Attribute**](https://bani--connexcs-docs.netlify.app/developers/pages/introduction/#form-attribute) enables you to design attractive interactive interfaces for your customers. 
<img src="/pages/fields.png" alt="fields" width="5000"/>

## [Basic Fields](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/)

!!! note "Know More"
    Click on each **Icon** to find out more about each element. 

| **Icon**                                                                                                                                                                                                                                                                     | **Description**                                                                                                                                                                                                                                                                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [<img src="/pages/input-icon.png" alt="input" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#input-and-textarea)                                                                                                                                                                                                                   | The input field allows you to enter single-line text.                                                                                                                                                                                                                                                |
| [<img src="/pages/textarea.png" alt="textarea" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#input-and-textarea)                                                                                                                                                                                                                  | A textarea is useful when you want to allow users to enter a sizeable amount of free-form text, for example, a review or feedback.                                                                                                                                                            |
| [<img src="/pages/number.png" alt="number" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#number)                                                                                                                                                                                                                      | The number field helps to start a counter from a minimum to a maximum value.                                                                                                                                                                                                                       |
| [<img src="/pages/radio.png" alt="radio" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#radio-button-and-checkbox-button)                                                                                                                                                                                                                        | The radio buttons allow one option to be selected out of the multiple options.                                                                                                                                                                                |
| [<img src="/pages/checkbox.png" alt="checkbox" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#radio-button-and-checkbox-button)                                                                                                                                                                                                                  | Checkboxes are used when there are lists of options and the user may select any number of choices, including zero, one, or several. <br><br> In other words, each checkbox is independent of all the other checkboxes in the list, so checking one box doesn't uncheck the others. |
| [<img src="/pages/select.png" alt="select" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#select)                                                                                                                                                                                                                      | The select option is a drop-down list with various options; you can either select one or many options.                                                                                                                                                                                                       |
| [<img src="/pages/time.png" alt="time" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#time)                                                                                                                                                                                                                          | The time picker allows you to pick a time (hh: mm :ss). <br> You can also select the start and end time.                                                                                                                                                                                                                                         |
| [<img src="/pages/date.png" alt="date" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#date)                                                                                                                                                                                                                          | The date picker allows you to pick a date (yyyy-mm-dd).<br> You can also select the start and end dates.                                                                                                                                                                                                                                       |
| [<img src="/pages/rate.png" alt="rate" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#rate)                                                                                                                                                                                                                          | A rating is an evaluation or assessment of something in terms of quality, quantity, or some combination of both. Therefore, you can add this wherever you want to rate the quality of a call, cost, or latency.                                                                 |
| [<img src="/pages/color.png" alt="color" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#color)                                                                                                                                                                                                                        | The color picker allows you to change the color.                                                                                                                                                                                                                                                 |
| [<img src="/pages/switch.png" alt="switch" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#switch)                                                                                                                                                                                                                      | The switch allows switching between "true" and "false" values.                                                                                                                                                                                                                             |
| [<img src="/pages/slider.png" alt="slider" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#slider)                                                                                                                                                                                                                      | The slider is a  control for selecting a single value from a continuous range of values.                                                                                                                                                                                                       |
| [<img src="/pages/text.png" alt="text" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#text)                                                                                                                                                                                                                          | Text displays a non-interactive piece of text to the user. Text elements can be used to provide captions or labels for other GUI controls or to display instructions or other text                                                                                                  |
| [<img src="/pages/html.png" alt="html" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#html)                                                                                                                                                                                                                          | HTML provides you with the option of writing the HTML code.                                                                                                                                                                                                                                 |
| [<img src="/pages/button.png" alt="button" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#button)                                                                                                                                                                                                                      | The button is responsible for performing an action when clicked, either for redirecting or for viewing purposes.                                                                                                                                                                 |
| [<img src="/pages/link.png" alt="link" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#link)                                                                                                                                                                                                                          | Link lets you add an external link to the page. When you click on the link, you will be redirected to that website, document, etc.                                                                                                                                               |
| [<img src="/pages/cascader.png" alt="cascader" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#cascader)                                                                                                                                                                                                                  | Cascader is a multi-level dropdown option. When a data set has a clear hierarchical structure, it can be viewed and selected through the cascading selector.                                                                                                                                                                                                                                            |
| [<img src="/pages/steps.png" alt="steps" width="175"/>](https://bani--connexcs-docs.netlify.app/developers/pages/basic-field/#steps)                                                                                                                                                                                                                        | Steps can be used to show the progress of a process. For each completed step, the corresponding step number will be highlighted.                                                                                                                                                               |

## [Advance Fields](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/)

!!! note "Know More"
    Click on each **Icon** to learn more about each element. 

| **Icon**                                                        | **Description**                                                                                                                                                                                                                           |
|-----------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [<img src="/pages/data-table.png" alt="data table" width="135"/>](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/#data-table-advanced-grid-and-multi-form)      | A Data table is a document composed of columns, rows, and cells that contain specific values.<br> They store information that people can retrieve later and update as required.<br> It can be used for importing or editing multiple entries.                                                              |
| [<img src="/pages/advanced-grid.png" alt="advanced-grid" width="135"/>](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/#data-table-advanced-grid-and-multi-form)     | The grid displays a grid-like layout on the various navigation bars like Customers, Carriers, etc.<br> It is more useful for editing and displaying information on the system than feeding it information.                                                                                                                                                 |
| [<img src="/pages/graph.png" alt="graph" width="135"/>](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/#graph)           | A graph allows you to display graphs of various parameters like ASR, RTP.                                                                                                                                                                          |
| [<img src="/pages/multi-form.png" alt="multi-form" width="135"/>](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/#data-table-advanced-grid-and-multi-form) | The Multi-form feature allows you to prepare multiple forms. <br> If you want multiple duplicate copies (cloning) of the created form, you can use this advanced component.                                                                          |
| [<img src="/pages/dialog.png" alt="dialog" width="135"/>](https://bani--connexcs-docs.netlify.app/developers/pages/advance-field/#dialog)| A dialog is a small window that prompts the user to make a decision or enter additional information. <br>A dialog does not fill the screen and is normally used for events that require users to take an action before they can proceed.|

## [Layout](https://bani--connexcs-docs.netlify.app/developers/pages/layout/)

!!! note "Know More"
    Click on each **Icon** to learn more about each element. 

| **Icon**                                                    | **Description**                                                                                                                                                                                                                                                                                          |
|-------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [<img src="/pages/collapse.png" alt="collapse" width="155"/>](https://bani--connexcs-docs.netlify.app/developers/pages/layout/#collapse) | The collapse option allows you to make a section, or group of fields, collapsible. It is useful when there are several sections in your form and you want them to take up less vertical space. <br><br> You may use collapsible or standard sections to adjust your form layout or conditionally hide or show a group of fields. |
| [<img src="/pages/inline.png" alt="inline" width="155"/>](https://bani--connexcs-docs.netlify.app/developers/pages/layout/#inline)     | The inline feature allows you to create a reactive layout where each element occupies only the width it requires.                                                                                                                                                                                                                     |
| [<img src="/pages/alert.png" alt="alert" width="155"/>](https://bani--connexcs-docs.netlify.app/developers/pages/layout/#alert)       | An alert occurs in response to an event and can potentially trigger a notification. It brings something to the user's attention and provides a way of sending a message that can be read without opening the app, e.g., a low-balance alert.|
| [<img src="/pages/grid.png" alt="grid" width="155"/>](https://bani--connexcs-docs.netlify.app/developers/pages/layout/#grid)         | A grid layout provides equal size for two-dimensional layouts.                                                                                                                                                                                                                      |
| [<img src="/pages/table.png" alt="table" width="155"/>](https://bani--connexcs-docs.netlify.app/developers/pages/layout/#table)       | A table allows you to arrange the elements in rows and columns. The rows and columns are added dynamically as you build the table.                                                                                                                                                                                |
| [<img src="/pages/tabs.png" alt="tabs" width="155"/>](https://bani--connexcs-docs.netlify.app/developers/pages/layout/#tabs)         | Adding tabs to a form can make it more organised and easier to use if the form contains many controls. You can place the related controls on separate pages of the tab.                                                                                                                                              |    
    
You can change the characteristics of each component. You can click on **Component Attribute** to change the properties of the elements.
   

## Form Attribute

<img src="/pages/caformattribute.png" alt="formattribute" width="260"/>

The Form attribute helps you specify values for the following parameters for all the fields in the form:

**1. Form Width**: Form width helps you decide the dimensions of the overall form.

**2. Label Position**: Label position helps you position the field labels.<br> You can decide between Left, Right and Top. 

**3. Size**: Size describes the dimensions of all the fields in the form. <br> You can choose from **Large**, **Small**, and **Mini**. 

**4. Style sheets**: You can add custom Style Sheets to make the interface look more pleasing.

**5. Data Source**: Data Source can be External, from Script Forge or a Database.

**6. Action Panel**: Action Panel allows you to specify the actions for buttons and link controls.

## Preview Options

<img src="/pages/capreviewoptions.png" alt="previewoptions" width="120"/>

Click on the **Preview** button to view the form.<br> You can choose between the **Monitor** view, **Tablet** view, and **Cellphone** view. 

**1. Get Data**: Get Data displays the raw data from the form.

**2. Reset**: Resetting will erase all the data filled in the form.

**3. Disabled or Enabled Edit**: Disabled edit will not allow your customer to enter data in the form; Enabled edit will allow you to enter the data in the form.

**4. Print Read Mode**: Print Read mode allows you to view the form before printing.

**5. Print**: The print option will let you print the filled form.

**6. Close**: Close will you exit from the preview window.

!!! note "More examples"
    [**Click here**](https://page-builder-api-docs.connexcs.com/page.html) to get a more detailed view on the examples and methods for creating Pages.
