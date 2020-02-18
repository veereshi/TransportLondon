# TransportLondon
TransportLondon


This application is a .net core console app and built on latest .net core 3.1 framework

Step 1:  install .net core 3.1 .NET Core 3.1 SDK from the below link 
https://dotnet.microsoft.com/download

step 2: unzip the project folder to local directory ( ex : c:\vProject\TransportLondon)
go to command line and root to project folder as shown in the below example
c:\Users\v> cd “: c:\vProject\TransportLondon” (press enter)
then type DIR. you should able to see to below list of files 

c:\vProject\TransportLondon>DIR   
13-01-2020  00:37    <DIR>          .
13-01-2020  00:37    <DIR>          ..
12-01-2020  22:47               147 appsettings.json
13-01-2020  00:37    <DIR>          bin
12-01-2020  23:21    <DIR>          DataModel
13-01-2020  00:37    <DIR>          obj
13-01-2020  00:20             1,097 Program.cs
12-01-2020  23:52    <DIR>          Properties
13-01-2020  00:44               163 README.md
13-01-2020  00:37               811 RoadStatus.csproj
12-01-2020  23:52               332 RoadStatus.csproj.user
13-01-2020  00:19    <DIR>          Service
13-01-2020  00:25             1,630 TransportLondon.sln
               6 File(s)          4,180 bytes
               7 Dir(s)  421,586,653,184 bytes free

Step 3: run “dotnet restore RoadStatus.csproj” command to restore nuget packages 
C:\Users\veere\source\repos\TransportLondon> dotnet restore RoadStatus.csproj

Ste 4: to publish the project run “dotnet publish RoadStatus.csproj” command 
C:\Users\veere\source\repos\TransportLondon> dotnet publish RoadStatus.csproj

Step5: go the publish folder location under bin directory to verify the published files.
for above example path available under “TransportLondon\bin\Debug\netcoreapp3.1\publish”

step 6: now open the command path under the publish folder location as below and type DIR to check list of files 
C:\Users\veere\source\repos\ TransportLondon\bin\Debug\netcoreapp3.1\publish>DIR
You should able see below output:
13-01-2020  00:59    <DIR>          .
13-01-2020  00:59    <DIR>          ..
12-01-2020  22:47               147 appsettings.json
01-01-1980  00:00            21,368 Microsoft.Extensions.Configuration.Abstractions.dll
01-01-1980  00:00            25,464 Microsoft.Extensions.Configuration.Binder.dll
01-01-1980  00:00            27,512 Microsoft.Extensions.Configuration.dll
01-01-1980  00:00            22,904 Microsoft.Extensions.Configuration.FileExtensions.dll
01-01-1980  00:00            21,880 Microsoft.Extensions.Configuration.Json.dll
01-01-1980  00:00            17,784 Microsoft.Extensions.FileProviders.Abstractions.dll
01-01-1980  00:00            35,704 Microsoft.Extensions.FileProviders.Physical.dll
01-01-1980  00:00            39,288 Microsoft.Extensions.FileSystemGlobbing.dll
01-01-1980  00:00            38,776 Microsoft.Extensions.Primitives.dll
09-11-2019  00:56           693,680 Newtonsoft.Json.dll
13-01-2020  00:59             8,214 RoadStatus.deps.json
13-01-2020  00:39            12,800 RoadStatus.dll
13-01-2020  00:39           169,984 RoadStatus.exe
13-01-2020  00:39             2,948 RoadStatus.pdb
13-01-2020  00:59               154 RoadStatus.runtimeconfig.json
              16 File(s)      1,138,607 bytes
               2 Dir(s)  421,534,547,968 bytes free

Step 7: 	update appsettings.json config file with appId and Appkey
  "AppId": "XXXXXX",
    "AppKey": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "AppUrl": https://api.tfl.gov.uk/    (no need to change)

Step 8: on command prompt run “RoadStatus.exe A2” to check result  example as shown below 
C:\Users\veere\source\repos\ TransportLondon\bin\Debug\netcoreapp3.1\publish> RoadStatus.exe A2

Desired output :

The status of the A2 is as follows
Road Status is Good
Road Status Description is No Exceptional Delays

