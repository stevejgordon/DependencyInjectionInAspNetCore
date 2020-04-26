# Prerequisites

- .NET Core SDK 2.1+
- Visual Studio 2019 or alternative editor

# Configuration Steps Required to Run Sample

1: Open the TennisBookings.sln in Visual Studio.

*If prompted with a security warning, deselect "Ask me for ever project in this solution" and click "OK".*

![Security Warning](images/image-01.png)

2: Set multiple startup projects...

- Right click on the solution and choose "Set Startup Projects".

![Startup Projects](images/image-02.png)

- Choose "Multiple startup projects"

Set `WeatherService.Api` as "Start without debugging" and `TennisBookings.Web` as "Start".

- Ensure `WeatherService.Api` is moved to the top of the list.

![Startup Projects](images/image-03.png)

- Click "OK" to close the solution properties window.

3: Expand the `WeatherService.Api` project and open the "launchSettings.json" file.

![Startup Projects](images/image-04.png)

4: Copy the auto-generated iisExpress application URL from the file.

![Startup Projects](images/image-05.png)

5: Open the appSettings.json file inside the `TennisBookings.Web` application.

![Startup Projects](images/image-06.png)

6: Paste the copied URL as the value for the "WeatherApiUrl" under "ExternalServices"

![Startup Projects](images/image-07.png)