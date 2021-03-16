This folder contains sample implementations of the XSDs into C# via the Visual Studio xsd.exe tool.   
This is in order to validate completeness and ability of a tool to implement the XSDs.       
   
These files were created via:
```batch
cd Xml
xsd /c TargetMarketDeterminations.xsd Common.xsd /order /out:"C#"
xsd /c Dealings.xsd Common.xsd /order /out:"C#"
xsd /c Complaints.xsd Common.xsd /order /out:"C#"
```