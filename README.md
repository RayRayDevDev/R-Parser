# R-Parser
EXIF Data Processor with Initial MOV/MP4 Support!

This is a simple C# app which takes the current file name of a JPEG/JPG, PNG, HEIC, or MOV/MP4 file and, upon checking its metadata for a date created or earliest access date (whichever comes first), renames the file to that date, with a preference for the date created. This allows for easy sorting of photos and videos in most gallery apps and, indeed, in most file systems when sorting by "name", which is what I was having trouble with. 

As a relatively new developer, there are no doubt bugs and/or features one may wish to request--feel free to create a pull request and/or report an issue and I will look into it!

I plan on supporting more file formats and Mac/Linux enviornments as well. Learning about said enviornments is probably helpful before I start trying to write software for it, though.

You may (I dunno why you would want to, but I digress) make use of this repository under the GNU v3 terms as specified in the license. All external libraries used retain their original licenses, so be sure to review those if you have a specific use in mind.

Attribution is always welcome too!

## How to Run

**Requirements:** [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or newer.

```bash
git clone https://github.com/RayRayDevDev/R-Parser.git
cd R-Parser
dotnet run
```

`dotnet run` restores the NuGet dependencies, builds, and launches the console app. From the menu:

1. **Rename files based on Exif date** — enter the path to a folder; the app scans it (and subfolders) for `.jpg`/`.jpeg`/`.png`/`.tiff`, `.mp4`/`.mov`/`.avi`/`.mkv`, and `.heic` files and renames each to its captured/created date (`yyyy-MM-dd HH_mm_ss`). Answer `y` to the recheck prompt to reprocess files that already match the naming scheme, or `n` to skip them.
2. **Undo renaming** — reverts the most recent rename operation back to the original file names (only available for the files renamed in the current session).
3. **Exit** — closes the app.

To build a standalone executable instead:

```bash
dotnet build -c Release
```

Thanks for visiting! 

All the best! 

--Rä.
