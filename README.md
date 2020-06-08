# hola-mundo
<actions>
   <add path="configuration/SharePoint/SafeControls">
      <SafeControl
         Assembly="System.Web, Version=1.0.5000.0, Culture=neutral, 
            PublicKeyToken=b03f5f7f11d50a3a"
         Namespace="System.Web.UI.WebControls"
         TypeName="*"
         Safe="True"/>
   </add>
   <remove path="configuration/SharePoint/RuntimeFilter"/>
   <add path="configuration/SharePoint">
      <RuntimeFilter
         Assembly="Company.Product, Version=1.0.1000.0, 
            Culture=neutral, PublickKeyToken=1111111111"
         Class="MyRuntTimeFilter",
         BuilderUrl="MyBuilderUrl"/>
   </add>
</actions>
