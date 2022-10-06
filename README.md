# VisualForce
## Standard Components
* [Standard Component Reference](https://developer.salesforce.com/docs/atlas.en-us.224.0.pages.meta/pages/pages_compref.htm?_ga=2.130643531.557902492.1665069460-1334770197.1660755932)
### Important Components
* `<apex:page></>` - The template tag for a visual force page
* `<apex:page standardController="sObject"></>` - Displays the standard controller for a standard or custom object
* `<apex:pageBlock ></>` - A container component
  * `<apex: pageBlockSection></>` - A wrapper component used with pageBlock to enable the looks and feel of its children components
* `<apex:detail relatedList="boolean"/>` - Displays a high level view of a standard/custom objects detail containing feild data and related object data
  * `<apex:relatedList list="SObject" />` - Displays a specified related list
    *  `<apex:enhancedList>` and `<apex:listViews>` - alternatives with more advanced features
  * `<apex:outputField value="field"></>` - Displays individual field data
### Iterator Components
* `<apex:pageBlockTable value="collection" var="variable"></>`- Creates a table with each column being a field of the object. Uses Salesforce Classic Styling
* `<apex:dataTable>` - Does not use Salesforce Classic Styling 
* `<apex:dataList>` - Does not use Salesforce Classic Styling 
* `<apex:repeat>` - Generates an arbitray markup of a collection of components
