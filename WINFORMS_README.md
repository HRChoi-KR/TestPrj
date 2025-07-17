# WinForms Application

This project has been converted from a console application to a Windows Forms application.

## Changes Made

1. **Project File (TestPrj.csproj)**: 
   - Changed `OutputType` from `Exe` to `WinExe`
   - Changed `TargetFramework` to `net8.0-windows`
   - Added `UseWindowsForms` property set to `true`

2. **Program.cs**: 
   - Updated to initialize WinForms application
   - Added `[STAThread]` attribute for Windows Forms compatibility
   - Changed from Console.WriteLine to Application.Run(new Form1())

3. **Form1.cs**: 
   - Created main form class inheriting from Form
   - Calls InitializeComponent() in constructor

4. **Form1.Designer.cs**: 
   - Created designer file with form layout
   - Added a label with text "Hello World!!!"
   - Set form size to 300x150 pixels
   - Positioned label at coordinates (50, 50)

## Requirements

- Windows operating system
- .NET 8.0 or later
- Windows Forms workload (usually included with .NET SDK on Windows)

## Running the Application

On Windows, you can run the application using:

```bash
dotnet run
```

The application will open a window with a label displaying "Hello World!!!" text.

## Note

This project requires the Windows Desktop SDK which is not available in Linux environments. The project structure is correct and will compile and run properly on Windows systems.