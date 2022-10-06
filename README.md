# VisualForce
# Components
## Important Components
* `<apex:page></>` - The template tag for a visual force page
* `<apex:pageBlock></>` - A container component
  * `<apex: pageBlockSection></>` - A wrapper component used with pageBlock to enable the looks and feel of its children components
* `<apex:page standardController="sObject"></>` - Displays the standard controller for a standard or custom object
* `<apex:detail></>` - Displays a high level view of a standard/custom objects detail containing feild data and related object data
  * `<apex:realtedList list="SObject"></>` - Displays a specified related list
  * `<apex:outputField value="field"></>` - Displays individual field data
## Iterator Components
* `<apex:pageBlockTable value="collection" var="variable"></>`- Creates a table with each column being a field of the object. Uses <apex:column value="field"> as its child
