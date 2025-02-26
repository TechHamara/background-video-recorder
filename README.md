# background-video-recorder
An Extension To Record Background Video Without Open Camera App

<div align="center">
<h1><kbd>🧩 BackgroundVideoRecorder</kbd></h1>
An extension for MIT App Inventor 2.<br>
Developed by th using Fast. An Extension To Record Background Video Without Open Camera App, with Inclued video quality with including dynamic orientation rotation for cinematic effects.
</div>

## 📝 Specifications
* **
💾 **Size:** 12.24 KB<br>
⚙️ **Version:** 1.0<br>
📱 **Minimum API Level:** 7<br>
📅 **Updated On:** [date=2025-02-25 timezone="Asia/Calcutta"]<br>
💻 **Built & documented using:** [FAST-CLI](https://community.appinventor.mit.edu/t/fast-an-efficient-way-to-build-extensions/129103?u=jewel)<br><br>

## <kbd>Events:</kbd>
**BackgroundVideoRecorder** has total 9 events.

![FrontCameraSelectedBlock](https://github.com/user-attachments/assets/4c42574f-2902-452e-a824-6185a04f68ab)
### 💛 FrontCameraSelected
Event triggered when front camera is selected.

![BackCameraSelectedBlock](https://github.com/user-attachments/assets/3d83000e-ab6b-4215-96c7-d31abded4cd6)
### 💛 BackCameraSelected
Event triggered when back camera is selected.


![VideoRecordingPausedBlock](https://github.com/user-attachments/assets/2ed5e490-42c8-4c70-942b-4bfaff7cc0cd)
### 💛 VideoRecordingPaused
Event triggered when video recording has been paused.

![VideoRecordingResumedBlock](https://github.com/user-attachments/assets/afbc5e39-e198-4ce3-a497-50851e0d34a3)
### 💛 VideoRecordingResumed
Event triggered when video recording has been resumed.

![PhotoCapturedBlock](https://github.com/user-attachments/assets/cb05c6c7-a1a3-4df2-954b-66ad8aa38b1d)
### 💛 PhotoCaptured
Event triggered when a photo has been captured successfully.

| Parameter | Type
| - | - |
| filePath | text

![PhotoCaptureErrorBlock](https://github.com/user-attachments/assets/e687b4e6-1708-418f-b11c-20421999ab25)
### 💛 PhotoCaptureError
Event triggered when an error occurs during photo capture.

| Parameter | Type
| - | - |
| message | text


![VideoRecordingStartedBlock](https://github.com/user-attachments/assets/1f29e74c-3018-47d3-8977-2fffb5cc748b)
### 💛 VideoRecordingStarted
Event triggered when video recording has successfully started.

![VideoRecordingStoppedBlock](https://github.com/user-attachments/assets/6ebaf2ba-ef30-4e7b-9b70-c615f8bf6457)
### 💛 VideoRecordingStopped
Event triggered when video recording has been stopped. and filePath The file path where the video was saved

| Parameter | Type
| - | - |
| filePath | text

![VideoRecordingErrorBlock](https://github.com/user-attachments/assets/a2da05e6-b850-460e-80b3-e7c9597ea1ae)
### 💛 VideoRecordingError
Event triggered when an error occurs during video recording. and message A message describing the error.

| Parameter | Type
| - | - |
| message | text

## <kbd>Methods:</kbd>
**BackgroundVideoRecorder** has total 13 methods.

![StartRecordingBlock](https://github.com/user-attachments/assets/1a79209b-d404-492c-b7a1-2659a1641d46)
### 💜 StartRecording
Starts video recording in the background with custom parameters and enhanced quality.
* height - The height (in pixels) of the video.
* width - The width (in pixels) of the video.
* orientation - The display orientation (e.g., 90 or 180).
* frameRate - The frame rate (e.g., 30 or 60).
* bitRate - The video bit rate (e.g., 2000000 (2mb lower bit rate) to 12000000 (12mb higher bit rate)).
* audioBitRate - The audio bit rate (e.g., 64000 (64kbps) to 320000 (320kbps)).
* filePath - The full path (including file name) where the recorded video will be saved.

| Parameter | Type
| - | - |
| width | number
| height | number
| orientation | number
| frameRate | number
| filePath | text

![StopRecordingBlock](https://github.com/user-attachments/assets/f7acd3b2-f391-47a7-bc7d-d7dce83a701c)
### 💜 StopRecording
Stops background video recording.

![FrontCameraBlock](https://github.com/user-attachments/assets/70bcf276-b5f9-45de-8568-b8e9ff265426)
### 💜 FrontCamera
Sets the camera to use the front-facing camera if available.

![BackCameraBlock](https://github.com/user-attachments/assets/6669d318-e233-4eed-b38c-eeeb4b782627)
### 💜 BackCamera
Sets the camera to use the back-facing camera if available.

![IsFrontCameraBlock](https://github.com/user-attachments/assets/d40e2484-713e-4ee2-9e34-c00c8c17d1fc)
### 💜 IsFrontCamera
Returns true if the front camera is currently selected.


![StartRecordingFHD1080PBlock](https://github.com/user-attachments/assets/c344f83a-38e6-4385-b997-2289ab1fec3e)
### 💜 StartRecordingFHD1080P
Starts high quality background video recording with preset parameters (1920x1080, 60 fps, 6Mbps video bitrate, 128Kbps audio bitrate).
* filePath - The full path (including file name) where the recorded video will be saved.

| Parameter | Type
| - | - |
| filePath | text

![PauseRecordingBlock](https://github.com/user-attachments/assets/8c802792-ddc7-4519-9c84-f6c074bbbe6f)
### 💜 PauseRecording
Pauses video recording if supported (API level 24 and above).

![ResumeRecordingBlock](https://github.com/user-attachments/assets/009ec2cb-0129-408a-a196-4736713962df)
### 💜 ResumeRecording
Resumes video recording if supported (API level 24 and above).

![IsRecordingBlock](https://github.com/user-attachments/assets/1b99da9c-bd0b-4e95-a095-5afd2017702f)
### 💜 IsRecording
Returns true if video recording is active, false otherwise.

![RecordedFilePathBlock](https://github.com/user-attachments/assets/198ffb89-a6af-4aae-b2d2-88ae56d54582)
### 💜 RecordedFilePath
Returns the file path of the last recorded video.

![CancelRecordingBlock](https://github.com/user-attachments/assets/c8170de1-9762-4eef-9bc6-ea6067939f98)
### 💜 CancelRecording
Cancels the current recording and cleans up resources.

![CapturePhotoBlock](https://github.com/user-attachments/assets/5309321a-d4cd-452f-b155-33935981286a)
### 💜 CapturePhoto
Captures a photo and saves it to the provided file path.

| Parameter | Type
| - | - |
| photoFilePath | text

![LastCapturedPhotoFilePathBlock](https://github.com/user-attachments/assets/788450e3-f644-4366-a59c-8d0b73caf788)
### 💜 LastCapturedPhotoFilePath
Returns the file path of the last captured photo.

### Thanks
    TechHamara

