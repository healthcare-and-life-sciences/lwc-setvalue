![](images/ahlsbanner.png)
<h1>A-HLS LWC - SetValues as Hyperlink Documentation</h1>

<h2>Overview</h2>

The SetValues as Hyperlink LWC enables a user to quickly fill in pre-determined data for an OmniScript. 

You have two styling options within an OmniScript: overriding the CSS via a file stored in a static resource (https://confluence.internal.salesforce.com/display/INDUSTRYARCH/CSS+style+a+SetValues+%27quick+fill%27+demo+button), or by adding (or extending) an LWC. There are pros and cons to both approaches.

Some prefer the former, as you don't have to compile/activate to see changes, although there's a good argument to be made for insulating the CSS to the specific control a la an LWC. This document outlines the latter case.

This custom LWC overrides the default OmniScript Set Values component so that when it is rendered within an OmniScript step is shown as a clickable hyperlink instead of the button.

![](/images/setvalues.png)

<h2>Business Objective</h2>

Useful for workflows where it is often efficient to auto-fill pre-determined data into a given OmniScript step. This method provides a more subtle approach versus a button.

<h3>Business Value and Benefits</h3>

* Decreased development time
* Faster speed to value
* Improved user experience


<h2>Package Includes:</h2>

*OmniScript (1)*

* Demo SetValue Link_OS.json (https://github.com/healthcare-and-life-sciences/lwc-setvalue/blob/main/omnistudio/Demo%20SetValue%20Link_OS.json)

*Custom LWC Components (3)*

* demo_setvalue_link
* demo_setvalue_next
* demo_setvalue_prev


<h2>Configuration Requirements</h2>

<h3>Install Steps</h3>

1. Install the LWC found at https://github.com/healthcare-and-life-sciences/lwc-setvalue/tree/main/src/lwc
2. Import the Omnistudio datapack found at https://github.com/healthcare-and-life-sciences/lwc-setvalue/tree/main/omnistudio

<h3>Post-Install Configuration Steps:</h3>

1. To use this, simply add a Set Values Element in your OmniScript of choice.
2. Then, set the "LWC Component Override" equal to: demo_setvalue_link


<h2>Assumptions</h2>

1. You are an Omnistudio developer who knows how to use LWC in Omniscript and Flexcard. You should be familiar with SF LWC development and Git
2. You are working in a Salesforce org which has OmniStudio installed.


<h2>Revision History</h2>

* *Revision Short Description (Month Day, Year)*

    * Initial Commit (August 31, 2022)

