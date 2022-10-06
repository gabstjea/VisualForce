# VisualForce
## Basics
* To append GET parameter to URL: &=_recordId_
* Utilize {!} for literal expressions
* Global variables: $User
* IF (expression, true, false)

## Standard Components
* [Standard Component Reference](https://developer.salesforce.com/docs/atlas.en-us.224.0.pages.meta/pages/pages_compref.htm?_ga=2.130643531.557902492.1665069460-1334770197.1660755932)

### Important Components
* `<apex:page></>` - Specifies how the page is processed. Is the main wrapper component
* `<apex:page standardController="sObject"></>` - Displays the standard controller for a standard or custom object
* `<apex:pageBlock ></>` - The main wrapper component for visual styling 
  * `<apex: pageBlockSection></>` - A wrapper component used with pageBlock to enable the looks and feel of its children components. Similar to div
* `<apex:detail relatedList="_boolean_"/>` - Displays a high level view of a standard/custom objects detail containing feild data and related object data
  * `<apex:relatedList list="_SObject_" />` - Displays a specified related list
    *  `<apex:enhancedList>` and `<apex:listViews>` - alternatives with more advanced features
  * `<apex:outputField value="_fieldNamespace_"></>` - Displays individual field data
### Iterator Components
* `<apex:pageBlockTable value="_collection_" var="_variable_"></>`- Creates a table with each column being a field of the object. Uses Salesforce Classic Styling
* `<apex:dataTable>` - Does not use Salesforce Classic Styling 
* `<apex:dataList>` - Does not use Salesforce Classic Styling 
* `<apex:repeat>` - Generates an arbitray markup of a collection of components

### Form Creation
* `<apex:field>` - Creates a form field used for creating, editing, retrieving, and saving records to the database
  *  Automatically performs form handling but error messages must be enabled with <apex:pageMesages />
 * `<apex:inputField value="">` - A form field
    * auto renders data based on the field's type
    * respects user permissions and validation rules
 * `<apex:commandButton action="" value="">` - fires an action for the form
 * `<apex:pageMessages />` - displays form handling information
 * To view, edit, and delete related records: [related records form]()
     *  To accomplish this use `<apex:outputLink />` in combination with `<apex:pageBlockTable>`
