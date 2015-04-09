---
title: Adding Images to Tabs
page_title: Adding Images to Tabs | UI for ASP.NET AJAX Documentation
description: Adding Images to Tabs
slug: tabstrip/appearance-and-styling/adding-images-to-tabs
tags: adding,images,to,tabs
published: True
position: 2
---

# Adding Images to Tabs



## 

Each __RadTab__ has a set of properties you can use to add images to the tab. You can simply add a single image to each tab, or you can add separate images that reflect the state of the tab.

The image appears to the left of the tab's text (unless you are using a [right-to-left orientation]({%slug tabstrip/appearance-and-styling/rtl-support%}), in which case it appear to the right of the tab's text). By setting the __Text__ property to an empty string, you can create tabs that are labelled solely with images.

The following properties let you add images to tabs:

* __ImageUrl__ specifies an image that is added to the tab. This image is always used, unless you set one of the other properties to specify an alternate image to use in a specific state.

* __SelectedImageUrl__ specifies an image that is used when the tab is selected.

* __HoveredImageUrl__ specifies an image that is used when the mouse is over the tab.

* __DisabledImageUrl__ specifies an image that is used when the tab is disabled.

To set the image properties at design time, use the [RadTabStrip Item Builder]({%slug tabstrip/design-time/radtabstrip-item-builder%}).

The following example uses the __ImageUrl__ and __SelectedImageUrl__ properties to create a __RadTabStrip__ that adds images to the top-level items:

````ASPNET
	 
	 <telerik:RadTabStrip
	 ID="RadTabStrip1" runat="server"
	 Skin="Office2007">
	 <Tabs>
	   <telerik:RadTab runat="server"
	     Text=" Documents A-F"
	     ImageUrl="~/Images/Folder.gif"
	     SelectedImageUrl="~/Images/Selected.gif" >
	     <Tabs>
	       <telerik:RadTab runat="server" Text="A" />
	       <telerik:RadTab runat="server" Text="B" />
	       <telerik:RadTab runat="server" Text="C" />
	       <telerik:RadTab runat="server" Text="D" />
	       <telerik:RadTab runat="server" Text="E" />
	       <telerik:RadTab runat="server" Text="F" />
	     </Tabs>
	   </telerik:RadTab>
	   <telerik:RadTab runat="server"
	     Text=" Documents G-L"
	     ImageUrl="~/Images/Folder.gif"
	     SelectedImageUrl="~/Images/Selected.gif">
	     <Tabs>
	       <telerik:RadTab runat="server" Text="G" />
	       <telerik:RadTab runat="server" Text="H" />
	       <telerik:RadTab runat="server" Text="I" />
	       <telerik:RadTab runat="server" Text="J" />
	       <telerik:RadTab runat="server" Text="K" />
	       <telerik:RadTab runat="server" Text="L" />
	     </Tabs>
	   </telerik:RadTab>
	   <telerik:RadTab runat="server"
	     Text=" Documents M-R"
	     ImageUrl="~/Images/Folder.gif"
	     SelectedImageUrl="~/Images/Selected.gif">
	     <Tabs>
	       <telerik:RadTab runat="server" Text="M" />
	       <telerik:RadTab runat="server" Text="N" />
	       <telerik:RadTab runat="server" Text="O" />
	       <telerik:RadTab runat="server" Text="P" />
	       <telerik:RadTab runat="server" Text="Q" />
	       <telerik:RadTab runat="server" Text="R" />
	     </Tabs>
	   </telerik:RadTab>
	   <telerik:RadTab runat="server"
	     Text=" Documents S-Z"
	     ImageUrl="~/Images/Folder.gif"
	     SelectedImageUrl="~/Images/Selected.gif">
	     <Tabs>
	       <telerik:RadTab runat="server" Text="S" />
	       <telerik:RadTab runat="server" Text="T" />
	       <telerik:RadTab runat="server" Text="U" />
	       <telerik:RadTab runat="server" Text="V" />
	       <telerik:RadTab runat="server" Text="W" />
	       <telerik:RadTab runat="server" Text="XYZ" />
	     </Tabs>
	   </telerik:RadTab>
	 </Tabs>
	</telerik:RadTabStrip> 
	 
````



![TabStrip With Images](images/tabstrip_withimages.png)

# See Also

 * [Controlling Appearance]({%slug tabstrip/appearance-and-styling/controlling-appearance%})

 * [Skins]({%slug tabstrip/appearance-and-styling/skins%})

 * [Overview]({%slug tabstrip/templates/overview%})

 * [Setting the CSS Class of Tabs]({%slug tabstrip/appearance-and-styling/setting-the-css-class-of-tabs%})