SOP: DVD Digitization for Archival

Version: v1.0 

Owner: Ryan Conley 

Last Updated: 2026-02-04 



Purpose \& Scope

Purpose: Standardize the conversion of physical DVD media into high-quality MP4 files for modern playback.

Trigger: Receipt of physical media and client digitization request.

End State: MP4s delivered on USB and temporary staging files purged.

Prerequisites

IT Technician: Verify local admin permissions.

IT Technician: Connect external USB DVD drive and ensure 10GB+ free SSD space.

Step-by-Step Procedure

IT Technician: Inspect the physical disc surface for scratches or debris.

IT Technician: Insert the DVD and Open VLC Media Player to verify playback.

IT Technician: Open Handbrake and Click 'Open Source' to load the disc.

IT Technician: Select the main movie title (usually the longest track) from the Title menu.

IT Technician: Apply the 'Fast 480p30' preset and Set the 'Container' to MP4.

IT Technician: Enable the 'Deinterlace' filter under the Filters tab.

IT Technician: Type the file name in the Save As field following the \[CLIENT\_NAME DVD\_##] format.

IT Technician: Drag and Drop the MP4 file from the \[LOCAL\_STAGING\_AREA] to the client USB drive.

IT Technician: Transfer the MP4 from the staging folder to the client USB drive.

IT Technician: Right-Click the USB drive icon and Select 'Eject' before returning the physical disc and USB to the client.

Exception Handling

Unreadable Disc: If VLC playback stutters, Clean the disc with a microfiber cloth and Retry.

File Size Limitation: If a file >4GB fails to transfer to the USB, Reformat the USB drive to exFAT.

Insufficient Storage: If Handbrake reports a "Disk Full" error, Purge previous temporary files in the staging area and Restart the encode.





Glossary / Data Dictionary

Transcoding: Converting video from DVD format to a compressed MP4 file.

Deinterlace: A filter that prevents "combing" artifacts on modern digital screens.

exFAT: A file system required for USB drives to support files larger than 4GB.



Change Log



Date

Version

Change

Why (Evidence)

Author

2026-02-04

v1.0

Added "IT Technician" to every step.

AI v0 draft had ambiguous actors; corrected for rubric compliance.

Ryan Conley

2026-02-04

v1.0

Added specific screen cues like "Filters tab."

Self-test showed a new hire wouldn't know where to find deinterlace settings.

Ryan Conley

2026-02-04

v1.0

Added "Insufficient Storage" exception.

Identified as a common failure mode during a recent client job.

Ryan Conley





Prompt Log



Prompt 1: "Based on the SOP v1 assignment page, give me a breakdown of how to hit those 'Full Marks' criteria."



Prompt 2: "Review my DVD Digitization steps. Identify any ambiguous pronouns and ensure every instruction starts with a concrete action verb like 'Click', 'Select', or 'Open'." 



Validation Decision: I accepted the AI's suggestion for adding screen-level cues (like 'Filters tab') to help new hires, but I rejected a suggestion to use "Auto" settings for transcoding to ensure quality control remains high.



