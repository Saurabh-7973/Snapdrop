<a>
<img src="assets/svg_asset/snapdrop_logo.svg" height="100" width="100"> 
<h1> Snapdrop </h1>

## Snapdrop - Effortless Image Transfer for UI/UX Designers

### 1. Features:

* Direct phone to Figma image transfer
* Secure QR code connection
* Seamless Figma plugin integration
* Review & integrate images in Figma

### 2. Useful For:

* UI/UX designers
* Anyone transferring images between phone and Figma

### 3. Core Structure:

* Mobile app: image selection & QR Scanning
* Figma plugin: QR code Generation & image import

### 4. Resources & Inspirations:

* Solves common designer image transfer pain point
* Streamlines workflow & improves design efficiency

### 5. Future Scope:

* Send more than 10 images at once or Send files larger than 5 mb.
* Able to see all the transfer history.

### 6. Screenshots:
<table>
  <tr>
    <td>
      <img src="assets/app_screenshots/splashscreen.jpeg" alt="Splashscreen" width="300">
    </td>
        <td>
      <img src="assets/app_screenshots/void_error.jpeg" alt="HomeScreen" width="300">
    </td>
        <td>
      <img src="assets/app_screenshots/home_screen.jpeg" alt="HomeScreen"  width="300">
    </td>
  </tr>
   <tr>
    <td>
      <img src="assets/app_screenshots/multiple_selection.jpeg" alt="Splashscreen" width="300">
    </td>
    <td>
      <img src="assets/app_screenshots/qr_screen.jpeg" alt="HomeScreen" width="300">
    </td>
      <td>
      <img src="assets/app_screenshots/review_images_2.jpeg" alt="Splashscreen" width="300">
    </td>
  </tr>
     <tr>
  </tr>
</table>



### File Structure

A High-level overview of the project structure:
```

lib/                     # Root Package
|
├─ Constant/                             # Constant files to use across the app
│  ├─ global_showcase_key/               # global key used for showcase view
│  ├─ theme_constant/                    # theme file
│
├─ Screen/                               # Contain all the main screens of the app
│  ├─ home_screen/                       # home screen for the app
│  ├─ intent_sharing_screen/             # Images send directly from other app
│  ├─ onboard_screen/                    # Onboarding user for the first time
│  ├─ qr_screen/                         # QR Screen
│  ├─ send_file_screen/                  # Review selected images screen
|
├─ Services/                             # Services used for the app
│  ├─ check_internet_connectivity/       # to check internet connectivity before sending the images
│  ├─ file_image/                        # used to identify the size of the image
│  ├─ first_time_login/                  # check first time login to display showcase view and onboarding screen
│  ├─ media_provider/                    # this class provides app with the album list and the images that are present in the album
│  ├─ permission_provider/               # To ask user to grant permission for storage and camera for picking images and scanning qr code
│  ├─ socket_service/                    # To transfer all the images from phone to your figma design file
|
├─ Widgets/                              # Widgets used multiple times throught the application is present here
│  ├─ app_bar_widget/                    # app bar for the app
│  ├─ connect/                           # connect to connecting to socket and sending images from phone to figma
│  ├─ dropdown_view/                     # dropdown used to display all the albums present with in the application and the images in a gridview
│  ├─ figma_display_helper/              # for displaing figma info
│  ├─ hero_text/                         # To display info throughtout every screen
│  ├─ intent_file_diplayer/              # Display images which is shared from other apps to Snapdrop
│  ├─ intro_widget/                      # used in the intro screen to display info
│  ├─ qr_scanner/                        # actual qr scanning code
│  ├─ room_displayer/                    # to display the room id when connected to figma
│  ├─ selected_images/                   # review images displayer
|
├─ main/                # Main class

```


</a>

